## 精粤 B760I SNOW DREAM 黑苹果 OpenCore EFI

![image](ScreenShot/JINGYUEB760M.jpg)

### [ENGLISH](README.EN.md)

### OpenCore

[OpenCore 0.9.9](https://github.com/acidanthera/OpenCorePkg)

### macOS

- macOS Monterey 12.x
- macOS Ventura    13.x
- macOS Sonoma   14.x

### 硬件

- 芯片组: B760
- Bios 版本: JYRPL003 04/13/2023
- 处理器: 英特尔12代 i9-12900 ES（QXQ3）
- 内存: 铭瑄白猎鹰16GBx2 DDR4 3200Mhz + 星驰星耀 16GBx2 DDR4 3200Mhz
- 硬盘: 三星 SSD 980 1TB MacOS
- 硬盘: 盈通 1TB Windows
- 硬盘: 东芝 DT01ACA100 1TB 机械硬盘
- 硬盘: 西数 WD30EZRX-19DCOB0 3TB 机械硬盘
- 核显: 英特尔超核心显卡770 (仅在Windows中可以使用)
- 独显: 华硕 Radeon RX 5700XT 8GB GDDR6
- 声卡: 瑞昱 ALC897
- 有线网卡:  瑞昱 RTL8125 Gaming 2.5GbE
- 无线网卡: 英特尔 AX200
- 处理器散热：利民 PA-120 白色
- 机箱:  爱国者 星璨·岚 白色
- 电源:  爱国者750瓦 金牌全模组

### BIOS设置

```
高级
     |-- CPU电源管理控制
        |-- CPU锁配置
	         |-- CFG锁定：关闭
	   |-- PCI总线驱动版本     
	       |-- Re-Size BAR Support：关闭
     |-- CSM配置
	      |-- CSM支持：关闭
		
启动
  |-- 安全启动
    |-- 安全启动：关闭
```

### 注意事项

 - 安装成功后必须使用 [OpenCore Configurator](https://mackie100projects.altervista.org/opencore-configurator/) 或者 [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools) 生成你自己的 SMBIOS
 - 如需使用没有小核心的CPU，必须取消勾选配置文件中Kernel--ProvideCurrentCpuinfo选项
 - 此EFI中的英特尔无线网卡驱动[AirportItlwm.kext](https://github.com/OpenIntelWireless/itlwm/releases)仅适用于 MacOS 14.3.1 Sonoma,安装其它版本请自行下载替换此驱动
 - 英特尔无线网卡无法使用隔空投送等功能

### 参考内容

[1.黑苹果安装过程演示](https://hackintosh.club/d/10000060)

[2.英特尔无线网卡WiFi驱动](https://hackintosh.club/d/10000015)

[3.英特尔无线网卡蓝牙驱动](https://hackintosh.club/d/10000017)

[4.我的B站黑苹果教程](https://space.bilibili.com/244390800/video)

[6.黑果之家](https://hackintosh.club)


### 联系我们

QQ群: 23304408

![image](ScreenShot/QRCode.png)



### 常用工具

- [Hackintool](https://github.com/headkaze/Hackintool)
- [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools) 简称 `OCAT`.
- [OpenCore Configurator](https://mackie100projects.altervista.org/opencore-configurator/) 简称 `OCC`.
- [gibMacOS](https://github.com/corpnewt/gibMacOS) 创建 MacOS 镜像 .
- [ProperTree](https://github.com/corpnewt/ProperTree) Plist 编辑器 .