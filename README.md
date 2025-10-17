# ROOTFS_EPICS_TCF
这是一个依据Debian8、Ubuntu 16.04.6提供的根文件系统更改的后的文件系统仓库，支持正点原子zynq最小系统板、alinx 7020b开发板。

## Debian8_ROOTfs下载连接：

通过网盘分享的文件：rootfs.tar.gz
链接: https://pan.baidu.com/s/1xQed2h5ADK5Xz-X_60zdvg 提取码: k913

## Ubuntu_ROOTfs下载连接：
通过网盘分享的文件：ubuntu_rootfs_16_04_6.tar.gz
链接: https://pan.baidu.com/s/1W0YsG4fOfj4gRWM9fA2GxA 提取码: ytqm

## 安装方法

查看设备：lsblk

# 在LINUX下挂载系统镜像文件
sudo mkdir /mnt/rootfs_img

sudo mount -o loop rootfs.img /mnt/rootfs_img

# 解压根文件系统到EXT4分区
sudo tar -xvpf rootfs.tar.gz -C /mnt/rootfs_img
