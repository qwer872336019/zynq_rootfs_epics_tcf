# ALINX_Debian8_TCF
这是一个依据ALINX提供的根文件系统更改的后的文件系统仓库

ROOTfs下载连接：

通过网盘分享的文件：rootfs.tar.gz
链接: https://pan.baidu.com/s/1xQed2h5ADK5Xz-X_60zdvg 提取码: k913

## 安装方法

查看设备：lsblk

# 在LINUX下挂载系统镜像文件
sudo mkdir /mnt/rootfs_img

sudo mount -o loop rootfs.img /mnt/rootfs_img

# 解压根文件系统到EXT4分区
sudo tar -xvpf rootfs.tar.gz -C /mnt/rootfs_img
