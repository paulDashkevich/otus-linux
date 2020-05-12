Процес миграции системы с одного диска на raid1 (md0)

1. В системе есть единственный диск sda, у него разделы swap (sda1), /home (sda2)  и / (sda3)
2. В систему добавляется пустой новый диск sdb, диск sda через fdisk ставим тип fd.
3. Создаём на диске sdb массив mdadm --create --verbose /dev/md0 -l 1 -n 2 /dev/sda1 /dev/sdb1
4. Создаём своп mkswap /dev/md0
5. Корректируем fstab /dev/sda1/2/3 -> /dev/md0/1/2
6. Активация своп swapon -a
7. Размечаем второй диск под разметку первого, на котором сейчас система:
	mdadm --create --verbose /dev/md1 -l 1 -n 2 missin /dev/sdb2
	mdadm --create --verbose /dev/md1 -l 1 -n 2 missin /dev/sdb2
	mkfs.ext4 /dev/md1
	mkfs.ext4 /dev/md2
8. Обновляем конфиг mdadm --examine --scan >> /etc/mdadm/mdadm.conf
9. Обновляем инфу о массиве update-initramfs -u
10.Синхронизируем смонтированные партиции md[x]:
	mount /dev/md1 /mnt/ && [tmux|screen] rsync -axu / /mnt
	moune /dev/md2 /mnt/home && [tmux|screen] rsync -axu /home/ /mnt/home
11.После rsync монтируем сис.каталоги к новому корню:
	mount --bind /proc /mnt/proc 
	mount --bind /dev /mnt/dev
	mount --bind /var /mnt/var
	mount --bind /run /mnt/run
	mount --bind /sys /mnt/sys
12.В новой системе -> chroot /mnt
13.На оба диска ставим загрузчики: 
	grub-install --recheck /dev/sda
	grub-install --recheck /dev/sdb
14.Обновляем конфиг загрузчика: update-grub
15.Добавляем в массив два раздела первого диска:
	mdadm /dev/md1 --add /dev/sda2
	mdadm /dev/md2 --add /dev/sda3
16.Результат наблюдаем 
	cat /proc/mdstat
