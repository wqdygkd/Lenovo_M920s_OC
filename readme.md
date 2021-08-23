# Lenovo_M920s_OC

oc 版本 0.6.5

电脑配置

| 规格     | 详细信息                                          |
| :------- | :------------------------------------------------ |
| 电脑型号 | 联想 ThinkCentre M920s-N000 台式电脑              |
| 处理器   | 英特尔 Core i5-8500 @ 3.00GHz 六核                |
| 内存     | 16 GB ( 三星 DDR4 2666MHz / 联想 DDR4 2400MHz )   |
| 主板     | 联想 3133（Q370 芯片组）                          |
| 硬盘     | 三星 MZVLB256HBHQ-000L7 ( 256 GB / 固态硬盘 )     |
| 显卡     | 英特尔 UHD Graphics 630 ( 128 MB / 联想 )         |
| 声卡     | 瑞昱 ALC662 @ 英特尔 High Definition Audio 控制器 |
| 网卡     | 英特尔 Ethernet Connection I219-LM / 联想         |
| BIOS版本 | M1UKT45A                                          |


PM981硬盘不能直接安装MAC，需要打补丁

使用方法一：克隆法（一定成功）
安装mac系统到U盘/移动硬盘/其他型号的硬盘
克隆安装好的MAC分区到PM981硬盘
需要补丁/ACPI/SSDT-nvme.aml和/kexts/other/HackrNVMeFamily.kext 来启动正常使用

使用方法二：正常安装
使用补丁 /kexts/NVMeFix.kext 正常安装，

```
bios 设置

bios 中没有 CFG Lock 选项，需使用Tools中的CFGLock.efi进行CFGLock解锁操作：将值设置为 0

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
    CPU 菜单
        Intel Virtualization 技术  -> 开启   （VT-x）
        VT-d -> 关闭
    Intel Manageability -> 关闭
    Intel SXG -> 关闭
    Intel SIPP 支持 -> 关闭
启动菜单
    兼容模块 -> 关闭
    启动方式 -> UEFI
```
