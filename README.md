# -
这是黑苹果系统安装的资料 本次感谢 给我安装的好友 

首先准备工作 最好买一块 独立的 固态磁盘专门做苹果系统 128|256|512 1T 看你经济而定 最好选择 512存储大一点 

准备16G的U盘拿来做苹果系统U盘

然后下载这个苹果系统 目前最新的版本是 10.15.6
点击下载最新的
https://mirrors.dtops.cc/iso/MacOS/daliansky_macos/

然后通过 TransMac 这个软件去把 Mac OSX系统烧录到的你的U盘
具体操作过程看教程 
Clover 安装
OpenCover 是新的引导的方式 OC

https://www.bilibili.com/video/BV1x54y1X7tS?from=search&seid=2960506841850373438

具体 引导文件 安装的方法 

请详细查询自己本机的机型

还有 远景论坛 黑果小兵使用 
	
我使用的是老版本的 Clover引导安装 

还可以使用 balenaEtcher写入到U盘

首先磁盘软件 使用的是 DiskGenius

寻找自己的 EFI 这一步最为关键

我的机型配置如下 

电脑型号	技嘉 B365 M AORUS ELITE 台式电脑  (扫描时间：2020年07月30日)
操作系统	Windows 10 专业版 64位 ( DirectX 12 )
	
处理器	英特尔 Core i5-9400F @ 2.90GHz 六核
主板	技嘉 B365 M AORUS ELITE-CF ( 300 Series 芯片组 Family (B365) )
内存	16 GB ( 金士顿 DDR4 2400MHz )
主硬盘	金士顿 SA400S37120G ( 120 GB / 固态硬盘 )
显卡	AMD Radeon RX 570 ( 8 GB / 蓝宝石 )
显示器	冠捷 AOC2491 2491W ( 23.5 英寸  )
声卡	瑞昱 ALC892 @ 英特尔 High Definition Audio 控制器
网卡	英特尔 Ethernet Connection  I219-V / 技嘉

我的EFI 已经保存下来了 需要的童鞋可以 私我

还要目前 比较通用的 EFI 也可以私我

我的显卡为 蓝宝石 Rx580 2048SP 需要降级到 Rx570 

降级显卡 如下 教程 

https://osx.cx/rx580-2048sp-shua-vbios-rx570.html

最后需要 进图入苹果 系统 利用 cmd的命令 输入 sudo spctl --master-disable 

双系统 windows时间显示不正确 需要 到 windows下的 
中命令 敲入 并开启 自动设置时间 自动 设置时区

cReg add HKLM\SYSTEM\CurrentControlSet\Control\TimeZoneInformation /v RealTimeIsUniversal /t REG_DWORD /d 1md
