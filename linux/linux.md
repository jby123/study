# [socat 安装](https://gitee.com/JBY8/doc/blob/socat/doc/README.md#)
# [parted分区](https://blog.csdn.net/cailirong123/article/details/130015943)
# [fdisk分区](https://blog.51cto.com/wang/4163156)
# 磁盘
## 分区
    fdisk -l
    parted /dev/sdb
    mklabel
    新的磁盘标签类型？ GPT
    mkpart
## 挂载
    mkfs.ext4 /dev/sdb1 #分区格式换
    mount /dev/sdb1 /demo #磁盘挂载到指定的目录
    df -hT
    vim /etc/fstab #开机自动挂载
    /dev/sdb1               /data             ext4    defaults        0 0 