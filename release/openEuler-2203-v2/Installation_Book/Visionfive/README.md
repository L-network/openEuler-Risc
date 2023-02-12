## 使用VisionFive开发板安装安装openEuler RISC-V 22.03 V2

注：

1. root用户密码`openEuler12#$`
2. openeuler用户密码`openEuler12#$`,默认用户

### 1. 准备硬件

1）visionfive开发板：由starfive获取得到开发板。

2）64G micro-sd卡及读卡器：SanDisk TF/MicroSD卡，容量64GB，速度U1，带读卡器。

3）Usb转uart串口通信模块：丢石头 PL2303，3.3/5V电平输出，type A接口，10PIN散头杜邦线。

4）电源适配器及type-c线。

5）连接visionfive开发板的40-Pin GPIO端和Usb转uart串口通信模块。

- GND连接6 GND
- RXD连接8 GPIO14(UART TX)
- TXD连接10 GPIO13(UART RX)

如下图：

![figure_1](./images/figure_1.png)

照片：

![figure_3](./images/figure_3.png)

### 2. 准备系统镜像

Visionfive的系统镜像下载连接地址如下： https://mirror.iscas.ac.cn/openeuler-sig-riscv/openEuler-RISC-V/preview/openEuler-22.03-V2-riscv64/Visionfive/

考虑到要安装验证Firefox浏览器，我们可以下载openEuler-22.03-V2-xfce-visionfive-preview.img.tar.zst，连接如下： https://mirror.iscas.ac.cn/openeuler-sig-riscv/openEuler-RISC-V/preview/openEuler-22.03-V2-riscv64/Visionfive/openEuler-22.03-V2-xfce-visionfive-preview.img.tar.zst

其他文件均无需下载。

```bash
wget  https://mirror.iscas.ac.cn/openeuler-sig-riscv/openEuler-RISC-V/preview/openEuler-22.03-V2-riscv64/Visionfive/openEuler-22.03-V2-xfce-visionfive-preview.img.tar.zst
```

### 3. 刷写镜像

以下步骤适用于Ubuntu20.04，如适用Windows操作系统，解压请下载[zstd](./zstd-v1.4.4-win32.zip)，`zstd.exe -d ./openEuler-22.03-V2-xfce-visionfive-preview.img.tar.zst`，之后将.img.tar解压为.img文件，刷写请下载[win32diskimager](./win32diskimager-1.0.0-install.exe)

1. 解压镜像文件

```bash
sudo apt install zstd -y
tar -I zstdmt -xvf ./openEuler-22.03-V2-xfce-visionfive-preview.img.tar.zst
```

2. 镜像刷写

将64G micro-sd卡装入读卡器后，插入笔记本电脑。笔记本电脑通常带一个硬盘，所以sd卡对应设备是/dev/sdb

```bash
sudo dd if=./openEuler-22.03-V2-xfce-visionfive-preview.img of=/dev/sdb bs=1M iflag=fullblock oflag=direct conv=fsync status=progress
```

### 4. 安装串口调试软件

1）将Usb转uart串口通信模块连接到电脑usb口。

2）检查设备管理器中的COM端口，例如COM4。

![figure_2](./images/figure_2.png)

3）使用Xmodem安装固件。

安装teraterm，https://mobaxterm.mobatek.net/download.html

    选择菜单setup->Serial port setup
    Speed设置为115200
    Data设置为8bit
    Paritv设置为none
    Stoo bits设置为1bit
    Flowcontrol设置为none

![figure_4](./images/figure_4.png)

### 5. 启动Visionfive

将64G micro-sd卡装入Visionfive sd卡槽，连接tpye-c电源启动，用户名：`root`，密码：`openEuler12#$`， 用户名：`openeuler`，密码：`openEuler12#$`

![figure_6](./images/figure_6.png)

openEuler RISC-V 22.03 V2 相对 V1 版本提升了Firefox的性能，为了获取性能提升，建议您安装镜像后进行软件升级，请打开一个终端，输入如下命令

```bash
dnf upgrade
```

备注：

**无线网络配置**

```
nmtui
```

### 6. 参考资料

<https://rvspace.org/en/Product/VisionFive/Technical_Documents/VisionFive_Software_Technical_Reference_Manual>

<https://wiki.rvspace.org/en/Product/VisionFive/Technical_Documents/VisionFive_Single_Board_Computer_Quick_Start_Guide>
