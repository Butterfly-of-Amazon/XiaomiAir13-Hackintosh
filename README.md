# XiaomiAir13-Hackintosh
适用于小米笔记本Air13的黑苹果EFI
1. 使用时，用OC目录下对应macOS版本的 Config-xxxx.list 改名替换掉 Config.list，用OC\Kexts 下的 AirportItlwm-xxxx.kext 改名替换掉 AirportItlwm.kext。
2. 对于 Catalina，系统安装好后，要安装 HeliPort.dmg 并设置为开机自动运行，才能使用 Wifi。
3. 我测试了Catalina、Big Sur、Montery、Ventura、Sonoma 等从10.15到14等各个版本的macOS，Wifi、蓝牙、声音、背光、触摸板、HDMI输出、睡眠、睿频等均正常；Sequoia（macOS15）不行。
4. 我的小米Air13配置为：Intel i7第八代CPU、RealTek235声卡、Intel Dual Band Wireless-AC 8265无线网卡、Intel UHD Graphics 620集成显卡。如果你的笔记本配置与我的一样，就可以直接用；如果配置接近，也可以试试，有可能会需要做些微调。
5. 相关文章：《小米Air13和联想Yoga311黑苹果EFI分享》（ https://mp.weixin.qq.com/s/SrdrzpuFetM0e_YbRC5kcQ ）

**注意：**
1. 由于苹果系统不支持小米Air13自带的三星硬盘（详见 https://dortania.github.io/OpenCore-Install-Guide/macos-limits.html#storage-support ），所以安装前需要把硬盘更换为西部数据等苹果支持的品牌，或者直接加装一个m2.sata硬盘（小米Air13除了m2.NVme，还富余一个m2.sata硬盘接口）。
