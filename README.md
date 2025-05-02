# lablk
Just a setting of lsblk using certain columns

# Install
- just copy `lablk` file in a folder inside your $PATH
```sh
sudo cp ./lablk /usr/local/bin
```

# Usage
- just execute `lablk`

# Example 
```
user@linux:~$ lablk 
NAME        PTTYPE   SIZE FSUSE% TYPE  FSTYPE            LABEL         PARTLABEL                    MOUNTPOINTS      UUID
sda         gpt    931,5G        disk                                                                                
└─sda1      gpt    931,5G        part  linux_raid_member debian-main:1 raid-part                                     bdc1d24d-c16e-4b05-91c9-5950a49c5231
  └─md1            931,4G    74% raid1 ext4                                                         /raid            6941c587-95ff-47fd-aacd-96307b8b9ff0
sdb         gpt    931,5G        disk                                                                                
├─sdb1      gpt       16M        part  ext4              wd-2.5-hdd    Microsoft reserved partition                  9c6c991d-f83e-426a-99c1-1a79271e52f6
├─sdb2      gpt    190,3G        part  ntfs                            Basic data partition                          9EE28C3EE28C1CA1
└─sdb3      gpt    541,2G        part  ext4              sata-ssd-main tmp                                           e6240e1c-8d00-47b9-84b7-851ae2228cb1
sdc         gpt    931,5G        disk                                                                                
└─sdc1      gpt    931,5G        part  linux_raid_member debian-main:1 raid-part                                     bdc1d24d-c16e-4b05-91c9-5950a49c5231
  └─md1            931,4G    74% raid1 ext4                                                         /raid            6941c587-95ff-47fd-aacd-96307b8b9ff0
sdd         dos        1M        disk                                                                                
└─sdd1      dos        1M        part  vfat              CIRCUITPY                                                   E40C-3A49
nvme0n1     gpt      1,8T        disk                                                                                
├─nvme0n1p1 gpt      600M     1% part  vfat              EFI                                        /boot/efi        9621-A4F1
├─nvme0n1p2 gpt      100G    54% part  ext4              root                                       /                8561679f-eea3-454d-8415-4a3db0acbbb3
└─nvme0n1p3 gpt      1,7T    44% part  ext4              home                                       /home            2a89e7d8-4b3a-437c-afdf-1136e68c3907
nvme1n1     gpt    931,5G        disk                                                                                
└─nvme1n1p2 gpt    931,5G    74% part  ext4              nvme-p3-main  root                         /nvme/crucial-p3 b456b5d8-368b-4c96-9fd6-c0d1dff6f873
```
