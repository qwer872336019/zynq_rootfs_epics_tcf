# ROOTFS_EPICS_TCF
这是一个依据Debian8、Ubuntu 16.04.6提供的根文件系统更改的后的文件系统仓库，支持正点原子zynq最小系统板、alinx 7020b开发板。

## Debian8_ROOTfs下载连接：

通过网盘分享的文件：rootfs.tar.gz
链接: https://pan.baidu.com/s/1xQed2h5ADK5Xz-X_60zdvg 提取码: k913

## Ubuntu_ROOTfs下载连接：
通过网盘分享的文件：ubuntu_rootfs_16_04_6.tar.gz
链接: https://pan.baidu.com/s/1W0YsG4fOfj4gRWM9fA2GxA 提取码: ytqm

## 安装方法
# 1. 查看设备：
lsblk

# 2. 格式化
mkfs.vfat /dev/sdX1

mkfs.ext4 /dev/sdX2

# 3. 解压 rootfs
sudo mount /dev/sdX2 /mnt

sudo tar -xzvpf rootfsV2.tar.gz -C /mnt

# 4. 拷贝 boot

# 5. 执行同步命令，比较久
sync
