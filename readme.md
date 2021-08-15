# Lenovo_M920s_Hackintosh_Bigsur_OC

oc 版本 0.7.2

电脑配置

|   规格    |  详细信息  |
| :------  | :-------------- |
| 电脑型号  |  联想 ThinkCentre M920s-N000 台式电脑 |
|  处理器  |  英特尔 Core i5-8500 @ 3.00GHz 六核  |
|   内存   |  16 GB ( 三星 DDR4 2666MHz / 联想 DDR4 2400MHz ) |
|   主板   |  联想 3133（Q370 芯片组） |
|   硬盘   |  三星 MZVLB256HBHQ-000L7 ( 256 GB / 固态硬盘 ) |
|   显卡   |  英特尔 UHD Graphics 630 ( 128 MB / 联想 )  |
|   声卡   |  瑞昱 ALC662 @ 英特尔 High Definition Audio 控制器  |
|   网卡   |  英特尔 Ethernet Connection I219-LM / 联想 |
| BIOS版本 |  M1UKT45A |

bios 设置

|   禁用   |  启用  |
| :------ | :-------------- |
| Fast Boot	快速启动 |      VT-x     |
|  CFG Lock (MSR 0xE2 write protection)	CFG 锁 (MSR 0xE2 写入保护)  |      Above 4G decoding	大于 4G 地址空间解码 |
|   VT-d   |     Hyper Threading	处理器超线程 |
|   CSM	兼容性支持模块   |   Execute Disable Bit	执行禁止位  |
|   Intel SGX   |   EHCI/XHCI Hand-off	接手 EHCI/XHCI 控制    |
|      |    Legacy RTC Device	传统 RTC 设备     |
|      |    瑞昱 ALC662 @ 英特尔 High Definition Audio 控制器        |
|      |     英特尔 Ethernet Connection I219-LM / 联想         |
|      |            M1UKT45A                  |


安全菜单：
    安全启动 -> 关闭 (Disable Secure Boot)
设备：
    显示菜单
        选择有效显示：IGD
        预指派内存大小：64MB (DVMT pre-allocated memory)
        全部显示内存：最大
    ATA设备菜单：
        配置SATA为 -> AHCI
高级菜单
    Intel Manageability -> 关闭
    Intel SXG -> 关闭
    Intel SIPP 支持 -> 关闭
启动菜单
    兼容模块 -> 关闭
    启动方式 -> UEFI
