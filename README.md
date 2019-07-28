# Hackintosh-DeskMini310

MacOS 10.14.x Mojave on ASRock DeskMini 310/com with UHD(4k), QQ 交流群: `580456695`

## 硬件配置

- `CPU`: Intel I7-8700Tes (`QN8J`)
- `内存`: 十栓 DDR4 2400 8Gx2
- `硬盘`: WD SN750 512G
- `显卡`: 集成显卡
- `网卡`: BCM94360CS2
- `显示器`: KOIOS K2718UD


## 黑苹果状态

黑苹果兼容所有 8 代 Intel CPU, 可随意更换 CPU. 网卡使用苹果官方拆机网卡+加转接板实现免驱. 所有 USB 端口已经做了补丁. 配合超低价 4K 显示器, 默认支持 Retina 模式. 显示完美.

- 睡眠完美
- 网络完美
- 声音自动切换耳机与喇叭完美
- 显示 DP 输出完美, HDMI 未测试, VGA 不支持
- USB完美


## BIOS 配置 版本： P4.1

BIOS 配置使用默认配置, 只需要对下面三个部分进行调整. 以 P4.1 版本的出厂 BIOS 为例:

- `USB Configuration` => `XHCI Hand-off` => `Enabled`
- `Onboard HD Audio` => `Enabled`
- `Security boot` => `Disabled`


## 网卡: `BCM94352z`

完美支持 `BCM94352z` 网卡, 需要添加额外三驱动文件:

- `AirportBrcmFixup.kext`
- `BrcmFirmwareData.kext`
- `BrcmPatchRAM2.kext`

> 将上述上个文件放置到 `/EFI/CLOVER/kexts/Other/` 目录下. 更换网卡, 重启即可.


## 使用方式

下载 CLOVER 目录, 替换自己硬盘 `EFI` 分区中的同名目录即可.


## 视频教程

全套视频教程可以网盘下载：

链接: [https://pan.baidu.com/s/1XC9T6pXPFoYHzk_v-OLoBg](https://pan.baidu.com/s/1XC9T6pXPFoYHzk_v-OLoBg) 提取码: `c64g`
