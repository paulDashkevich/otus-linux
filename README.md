Домашка №2
Создать бокс со скриптом, который создаёт массив 10 из 5 дисков.
 vagrant up
Bringing machine 'otuslinux' up with 'virtualbox' provider...
==> otuslinux: Box 'centos/7' could not be found. Attempting to find and install...
    otuslinux: Box Provider: virtualbox
    otuslinux: Box Version: >= 0
==> otuslinux: Loading metadata for box 'centos/7'
    otuslinux: URL: https://vagrantcloud.com/centos/7
==> otuslinux: Adding box 'centos/7' (v1905.1) for provider: virtualbox
    otuslinux: Downloading: https://vagrantcloud.com/centos/boxes/7/versions/1905.1/providers/virtualbox.box
Download redirected to host: cloud.centos.org
==> otuslinux: Successfully added box 'centos/7' (v1905.1) for 'virtualbox'!
==> otuslinux: Importing base box 'centos/7'...
==> otuslinux: Matching MAC address for NAT networking...
==> otuslinux: Checking if box 'centos/7' version '1905.1' is up to date...
==> otuslinux: Setting the name of the VM: otus-linux_otuslinux_1589279218695_41389
==> otuslinux: Clearing any previously set network interfaces...
==> otuslinux: Preparing network interfaces based on configuration...
    otuslinux: Adapter 1: nat
    otuslinux: Adapter 2: hostonly
==> otuslinux: Forwarding ports...
    otuslinux: 22 (guest) => 2222 (host) (adapter 1)
==> otuslinux: Running 'pre-boot' VM customizations...
==> otuslinux: Booting VM...
==> otuslinux: Waiting for machine to boot. This may take a few minutes...
    otuslinux: SSH address: 127.0.0.1:2222
    otuslinux: SSH username: vagrant
    otuslinux: SSH auth method: private key
    otuslinux:
    otuslinux: Vagrant insecure key detected. Vagrant will automatically replace
    otuslinux: this with a newly generated keypair for better security.
    otuslinux:
    otuslinux: Inserting generated public key within guest...
    otuslinux: Removing insecure key from the guest if it's present...
    otuslinux: Key inserted! Disconnecting and reconnecting using new SSH key...
==> otuslinux: Machine booted and ready!
==> otuslinux: Checking for guest additions in VM...
    otuslinux: No guest additions were detected on the base box for this VM! Guest
    otuslinux: additions are required for forwarded ports, shared folders, host only
    otuslinux: networking, and more. If SSH fails on this machine, please install
    otuslinux: the guest additions and repackage the box to continue.
    otuslinux:
    otuslinux: This is not an error message; everything may continue to work properly,
    otuslinux: in which case you may ignore this message.
==> otuslinux: Setting hostname...
==> otuslinux: Configuring and enabling network interfaces...
==> otuslinux: Rsyncing folder: /home/paul/otus-linux/ => /vagrant
==> otuslinux: Running provisioner: shell...
    otuslinux: Running: inline script
    otuslinux: Loaded plugins: fastestmirror
    otuslinux: Determining fastest mirrors
    otuslinux:  * base: mirror.datacenter.by
    otuslinux:  * extras: mirror.datacenter.by
    otuslinux:  * updates: mirror.datacenter.by
    otuslinux: Resolving Dependencies
    otuslinux: --> Running transaction check
    otuslinux: ---> Package gdisk.x86_64 0:0.8.10-3.el7 will be installed
    otuslinux: ---> Package hdparm.x86_64 0:9.43-5.el7 will be installed
    otuslinux: ---> Package mdadm.x86_64 0:4.1-4.el7 will be installed
    otuslinux: --> Processing Dependency: libreport-filesystem for package: mdadm-4.1-4.el7.x86_64
    otuslinux: ---> Package smartmontools.x86_64 1:7.0-2.el7 will be installed
    otuslinux: --> Processing Dependency: mailx for package: 1:smartmontools-7.0-2.el7.x86_64
    otuslinux: --> Running transaction check
    otuslinux: ---> Package libreport-filesystem.x86_64 0:2.1.11-53.el7.centos will be installed
    otuslinux: ---> Package mailx.x86_64 0:12.5-19.el7 will be installed
    otuslinux: --> Finished Dependency Resolution
    otuslinux:
    otuslinux: Dependencies Resolved
    otuslinux:
    otuslinux: ================================================================================
    otuslinux:  Package                  Arch       Version                     Repository
    otuslinux:                                                                            Size
    otuslinux: ================================================================================
    otuslinux: Installing:
    otuslinux:  gdisk                    x86_64     0.8.10-3.el7                base     190 k
    otuslinux:  hdparm                   x86_64     9.43-5.el7                  base      83 k
    otuslinux:  mdadm                    x86_64     4.1-4.el7                   base     439 k
    otuslinux:  smartmontools            x86_64     1:7.0-2.el7                 base     546 k
    otuslinux: Installing for dependencies:
    otuslinux:  libreport-filesystem     x86_64     2.1.11-53.el7.centos        base      41 k
    otuslinux:  mailx                    x86_64     12.5-19.el7                 base     245 k
    otuslinux:
    otuslinux: Transaction Summary
    otuslinux: ================================================================================
    otuslinux: Install  4 Packages (+2 Dependent packages)
    otuslinux:
    otuslinux: Total download size: 1.5 M
    otuslinux: Installed size: 4.3 M
    otuslinux: Downloading packages:
    otuslinux: Public key for hdparm-9.43-5.el7.x86_64.rpm is not installed
    otuslinux: warning: /var/cache/yum/x86_64/7/base/packages/hdparm-9.43-5.el7.x86_64.rpm: Header V3 RSA/SHA256 Signature, key ID f4a80eb5: NOKEY
    otuslinux: --------------------------------------------------------------------------------
    otuslinux: Total                                              3.1 MB/s | 1.5 MB  00:00
    otuslinux: Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
    otuslinux: Importing GPG key 0xF4A80EB5:
    otuslinux:  Userid     : "CentOS-7 Key (CentOS 7 Official Signing Key) <security@centos.org>"
    otuslinux:  Fingerprint: 6341 ab27 53d7 8a78 a7c2 7bb1 24c6 a8a7 f4a8 0eb5
    otuslinux:  Package    : centos-release-7-6.1810.2.el7.centos.x86_64 (@anaconda)
    otuslinux:  From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
    otuslinux: Running transaction check
    otuslinux: Running transaction test
    otuslinux: Transaction test succeeded
    otuslinux: Running transaction
    otuslinux:   Installing : libreport-filesystem-2.1.11-53.el7.centos.x86_64             1/6
    otuslinux:
    otuslinux:   Installing : mailx-12.5-19.el7.x86_64                                     2/6
    otuslinux:
    otuslinux:   Installing : 1:smartmontools-7.0-2.el7.x86_64                             3/6
    otuslinux:
    otuslinux:   Installing : mdadm-4.1-4.el7.x86_64                                       4/6
    otuslinux:
    otuslinux:   Installing : hdparm-9.43-5.el7.x86_64                                     5/6
    otuslinux:
    otuslinux:   Installing : gdisk-0.8.10-3.el7.x86_64                                    6/6
    otuslinux:
    otuslinux:   Verifying  : 1:smartmontools-7.0-2.el7.x86_64                             1/6
    otuslinux:
    otuslinux:   Verifying  : gdisk-0.8.10-3.el7.x86_64                                    2/6
    otuslinux:
    otuslinux:   Verifying  : mailx-12.5-19.el7.x86_64                                     3/6
    otuslinux:
    otuslinux:   Verifying  : hdparm-9.43-5.el7.x86_64                                     4/6
    otuslinux:
    otuslinux:   Verifying  : mdadm-4.1-4.el7.x86_64                                       5/6
    otuslinux:
    otuslinux:   Verifying  : libreport-filesystem-2.1.11-53.el7.centos.x86_64             6/6
    otuslinux:
    otuslinux:
    otuslinux: Installed:
    otuslinux:   gdisk.x86_64 0:0.8.10-3.el7          hdparm.x86_64 0:9.43-5.el7
    otuslinux:   mdadm.x86_64 0:4.1-4.el7             smartmontools.x86_64 1:7.0-2.el7
    otuslinux:
    otuslinux: Dependency Installed:
    otuslinux:   libreport-filesystem.x86_64 0:2.1.11-53.el7.centos mailx.x86_64 0:12.5-19.el7
    otuslinux:
    otuslinux: Complete!
    otuslinux: mdadm: Unrecognised md component device - /dev/sdb
    otuslinux: mdadm: Unrecognised md component device - /dev/sdc
    otuslinux: mdadm: Unrecognised md component device - /dev/sdd
    otuslinux: mdadm: Unrecognised md component device - /dev/sde
    otuslinux: mdadm: Unrecognised md component device - /dev/sdf
    otuslinux: mdadm: layout defaults to n2
    otuslinux: mdadm: layout defaults to n2
    otuslinux: mdadm: chunk size defaults to 512K
    otuslinux: mdadm: size set to 253952K
    otuslinux: mdadm: Defaulting to version 1.2 metadata
    otuslinux: mdadm: array /dev/md0 started.
    otuslinux: Personalities : [raid10]
    otuslinux: md0 : active raid10 sdf[4] sde[3] sdd[2] sdc[1] sdb[0]
    otuslinux:       634880 blocks super 1.2 512K chunks 2 near-copies [5/5] [UUUUU]
    otuslinux:       [>....................]  resync =  0.9% (6528/634880) finish=1.6min speed=6528K/sec
    otuslinux:
    otuslinux: unused devices: <none>
    otuslinux: Information: You may need to update /etc/fstab.

    otuslinux: Information: You may need to update /etc/fstab.

    otuslinux: Information: You may need to update /etc/fstab.

    otuslinux: Information: You may need to update /etc/fstab.

    otuslinux: Information: You may need to update /etc/fstab.

    otuslinux: mke2fs 1.42.9 (28-Dec-2013)
    otuslinux: Filesystem label=
    otuslinux: OS type: Linux
    otuslinux: Block size=1024 (log=0)
    otuslinux: Fragment size=1024 (log=0)
    otuslinux: Stride=512 blocks, Stripe width=2560 blocks
    otuslinux: 31360 inodes, 125440 blocks
    otuslinux: 6272 blocks (5.00%) reserved for the super user
    otuslinux: First data block=1
    otuslinux: Maximum filesystem blocks=33685504
    otuslinux: 16 block groups
    otuslinux: 8192 blocks per group, 8192 fragments per group
    otuslinux: 1960 inodes per group
    otuslinux: Superblock backups stored on blocks:
    otuslinux:  8193, 24577, 40961, 57345, 73729
    otuslinux:
    otuslinux: Allocating group tables: done
    otuslinux: Writing inode tables: done
    otuslinux: Creating journal (4096 blocks):
    otuslinux: done
    otuslinux: Writing superblocks and filesystem accounting information:
    otuslinux:  0/16
    otuslinux:
    otuslinux: done
    otuslinux: mke2fs 1.42.9 (28-Dec-2013)
    otuslinux: Filesystem label=
    otuslinux: OS type: Linux
    otuslinux: Block size=1024 (log=0)
    otuslinux: Fragment size=1024 (log=0)
    otuslinux: Stride=512 blocks, Stripe width=2560 blocks
    otuslinux: 31360 inodes, 125440 blocks
    otuslinux: 6272 blocks (5.00%) reserved for the super user
    otuslinux: First data block=1
    otuslinux: Maximum filesystem blocks=33685504
    otuslinux: 16 block groups
    otuslinux: 8192 blocks per group, 8192 fragments per group
    otuslinux: 1960 inodes per group
    otuslinux: Superblock backups stored on blocks:
    otuslinux:  8193, 24577, 40961, 57345, 73729
    otuslinux:
    otuslinux: Allocating group tables: done
    otuslinux: Writing inode tables: done
    otuslinux: Creating journal (4096 blocks):
    otuslinux: done
    otuslinux: Writing superblocks and filesystem accounting information:
    otuslinux:  0/16
    otuslinux:
    otuslinux: done
    otuslinux: mke2fs 1.42.9 (28-Dec-2013)
    otuslinux: Filesystem label=
    otuslinux: OS type: Linux
    otuslinux: Block size=1024 (log=0)
    otuslinux: Fragment size=1024 (log=0)
    otuslinux: Stride=512 blocks, Stripe width=2560 blocks
    otuslinux: 32000 inodes, 128000 blocks
    otuslinux: 6400 blocks (5.00%) reserved for the super user
    otuslinux: First data block=1
    otuslinux: Maximum filesystem blocks=33685504
    otuslinux: 16 block groups
    otuslinux: 8192 blocks per group, 8192 fragments per group
    otuslinux: 2000 inodes per group
    otuslinux: Superblock backups stored on blocks:
    otuslinux:  8193, 24577, 40961, 57345, 73729
    otuslinux:
    otuslinux: Allocating group tables: done
    otuslinux: Writing inode tables: done
    otuslinux: Creating journal (4096 blocks):
    otuslinux: done
    otuslinux: Writing superblocks and filesystem accounting information:
    otuslinux:  0/16
    otuslinux:
    otuslinux: done
    otuslinux: mke2fs 1.42.9 (28-Dec-2013)
    otuslinux: Filesystem label=
    otuslinux: OS type: Linux
    otuslinux: Block size=1024 (log=0)
    otuslinux: Fragment size=1024 (log=0)
    otuslinux: Stride=512 blocks, Stripe width=2560 blocks
    otuslinux: 31360 inodes, 125440 blocks
    otuslinux: 6272 blocks (5.00%) reserved for the super user
    otuslinux: First data block=1
    otuslinux: Maximum filesystem blocks=33685504
    otuslinux: 16 block groups
    otuslinux: 8192 blocks per group, 8192 fragments per group
    otuslinux: 1960 inodes per group
    otuslinux: Superblock backups stored on blocks:
    otuslinux:  8193, 24577, 40961, 57345, 73729
    otuslinux:
    otuslinux: Allocating group tables: done
    otuslinux: Writing inode tables: done
    otuslinux: Creating journal (4096 blocks):
    otuslinux: done
    otuslinux: Writing superblocks and filesystem accounting information:
    otuslinux:  0/16
    otuslinux:
    otuslinux: done
    otuslinux: mke2fs 1.42.9 (28-Dec-2013)
    otuslinux: Filesystem label=
    otuslinux: OS type: Linux
    otuslinux: Block size=1024 (log=0)
    otuslinux: Fragment size=1024 (log=0)
    otuslinux: Stride=512 blocks, Stripe width=2560 blocks
    otuslinux: 31360 inodes, 125440 blocks
    otuslinux: 6272 blocks (5.00%) reserved for the super user
    otuslinux: First data block=1
    otuslinux: Maximum filesystem blocks=33685504
    otuslinux: 16 block groups
    otuslinux: 8192 blocks per group, 8192 fragments per group
    otuslinux: 1960 inodes per group
    otuslinux: Superblock backups stored on blocks:
    otuslinux:  8193, 24577, 40961, 57345, 73729
    otuslinux:
    otuslinux: Allocating group tables: done
    otuslinux: Writing inode tables: done
    otuslinux: Creating journal (4096 blocks):
    otuslinux: done
    otuslinux: Writing superblocks and filesystem accounting information:
    otuslinux:  0/16
    otuslinux:
    otuslinux: done
[paul@localhost otus-linux]$ vagrant ssh
[vagrant@otuslinux ~]$ lsblk
NAME      MAJ:MIN RM   SIZE RO TYPE   MOUNTPOINT
sda         8:0    0    40G  0 disk
└─sda1      8:1    0    40G  0 part   /
sdb         8:16   0   250M  0 disk
└─md0       9:0    0   620M  0 raid10
  ├─md0p1 259:0    0 122.5M  0 md     /raid/part1
  ├─md0p2 259:1    0 122.5M  0 md     /raid/part2
  ├─md0p3 259:2    0   125M  0 md     /raid/part3
  ├─md0p4 259:3    0 122.5M  0 md     /raid/part4
  └─md0p5 259:4    0 122.5M  0 md     /raid/part5
sdc         8:32   0   250M  0 disk
└─md0       9:0    0   620M  0 raid10
  ├─md0p1 259:0    0 122.5M  0 md     /raid/part1
  ├─md0p2 259:1    0 122.5M  0 md     /raid/part2
  ├─md0p3 259:2    0   125M  0 md     /raid/part3
  ├─md0p4 259:3    0 122.5M  0 md     /raid/part4
  └─md0p5 259:4    0 122.5M  0 md     /raid/part5
sdd         8:48   0   250M  0 disk
└─md0       9:0    0   620M  0 raid10
  ├─md0p1 259:0    0 122.5M  0 md     /raid/part1
  ├─md0p2 259:1    0 122.5M  0 md     /raid/part2
  ├─md0p3 259:2    0   125M  0 md     /raid/part3
  ├─md0p4 259:3    0 122.5M  0 md     /raid/part4
  └─md0p5 259:4    0 122.5M  0 md     /raid/part5
sde         8:64   0   250M  0 disk
└─md0       9:0    0   620M  0 raid10
  ├─md0p1 259:0    0 122.5M  0 md     /raid/part1
  ├─md0p2 259:1    0 122.5M  0 md     /raid/part2
  ├─md0p3 259:2    0   125M  0 md     /raid/part3
  ├─md0p4 259:3    0 122.5M  0 md     /raid/part4
  └─md0p5 259:4    0 122.5M  0 md     /raid/part5
sdf         8:80   0   250M  0 disk
└─md0       9:0    0   620M  0 raid10
  ├─md0p1 259:0    0 122.5M  0 md     /raid/part1
  ├─md0p2 259:1    0 122.5M  0 md     /raid/part2
  ├─md0p3 259:2    0   125M  0 md     /raid/part3
  ├─md0p4 259:3    0 122.5M  0 md     /raid/part4
  └─md0p5 259:4    0 122.5M  0 md     /raid/part5
[vagrant@otuslinux ~]$ cat /etc/fstab

#
# /etc/fstab
# Created by anaconda on Sat Jun  1 17:13:31 2019
#
# Accessible filesystems, by reference, are maintained under '/dev/disk'
# See man pages fstab(5), findfs(8), mount(8) and/or blkid(8) for more info
#
UUID=8ac075e3-1124-4bb6-bef7-a6811bf8b870 /                       xfs     defaults        0 0
/swapfile none swap defaults 0 0
#NEW DEVICE
UUID="b6197dc4-1fe2-4cbc-97f2-7a323149dc53" /u01 ext4 defaults 0 0
UUID="b4cda336-cbb4-4b00-9f5e-089feef103dd" /u02 ext4 defaults 0 0
UUID="eb52e291-1aac-4f06-8263-3f0eb85d32d6" /u03 ext4 defaults 0 0
UUID="ee8b937f-4cc0-471a-9a01-5079f19a782c" /u04 ext4 defaults 0 0
UUID="d6fee457-a30f-40fc-8c86-ded910dfb8e6" /u05 ext4 defaults 0 0
[vagrant@otuslinux ~]$ cat /etc/mdadm
cat: /etc/mdadm: Is a directory
[vagrant@otuslinux ~]$ sudo mdadm -D -S
mdadm: No devices given.
[vagrant@otuslinux ~]$ sudo mdadm -D
mdadm: No devices given.
[vagrant@otuslinux ~]$ sudo mdadm -D /dev/md0
/dev/md0:
           Version : 1.2
     Creation Time : Tue May 12 10:28:21 2020
        Raid Level : raid10
        Array Size : 634880 (620.00 MiB 650.12 MB)
     Used Dev Size : 253952 (248.00 MiB 260.05 MB)
      Raid Devices : 5
     Total Devices : 5
       Persistence : Superblock is persistent

       Update Time : Tue May 12 10:28:57 2020
             State : clean
    Active Devices : 5
   Working Devices : 5
    Failed Devices : 0
     Spare Devices : 0

            Layout : near=2
        Chunk Size : 512K

Consistency Policy : resync

              Name : otuslinux:0  (local to host otuslinux)
              UUID : 9c77c9b7:7bec9c6f:3757a8b9:c4429fba
            Events : 21

    Number   Major   Minor   RaidDevice State
       0       8       16        0      active sync   /dev/sdb
       1       8       32        1      active sync   /dev/sdc
       2       8       48        2      active sync   /dev/sdd
       3       8       64        3      active sync   /dev/sde
       4       8       80        4      active sync   /dev/sdf
[vagrant@otuslinux ~]$ sudo mdadm -D --scan --verbose /dev/md0
ARRAY /dev/md0 level=raid10 num-devices=5 metadata=1.2 name=otuslinux:0 UUID=9c77c9b7:7bec9c6f:3757a8b9:c4429fba
   devices=/dev/sdb,/dev/sdc,/dev/sdd,/dev/sde,/dev/sdf

Из приведённого отображения выполнения скрипта в Vagrantfile видно
 Собрался массив 10, накатился GPT и разбилось на 5 частей. 
 Создан файл конфигурации массива при загрузке /etc/mdadm/mdadm.conf, соотвествующие записи вставлены в /etc/fstab

Ломаются массивы командой --fault с указанием диска, например mdadm --fault /dev/sdc
После этого диск удаляем --remove, добавляем в систему (используем вновь очищенный) диск wipefs -a /dev/новыйдиск

Смотрим за состоянием массива:
cat /proc/mdstat
Personalities : [raid10]
md0 : active raid10 sdf[4] sde[3] sdd[2] sdc[1] sdb[0]
      634880 blocks super 1.2 512K chunks 2 near-copies [5/5] [UUUUU]

