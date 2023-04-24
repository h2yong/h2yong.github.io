# 准备封装环境

## 用到的软件
- [VMware-workstation-16](https://www.ghxi.com/workstationlite.html)
- [优启通 v3.7.2023.0110](https://www.itsk.com/thread-428078-1-1.html)
- [Easy Sysprep 5S RS2](https://www.itsk.com/thread-428084-1-1.html)
- [万能驱动](https://www.itsk.com/thread-428855-1-1.html)
- [Dism-Multi-language](https://github.com/Chuyu-Team/Dism-Multi-language/releases)
- [软媒清理大师单文件版3.7.8.0](https://www.yrxitong.com/h-nd-122.html)
- [小鱼儿yr系统封装优化设置辅助工具](https://www.yrxitong.com/h-nd-100.html)
- [系统和Office激活工具_HEU KMS Activator](https://www.yrxitong.com/h-nd-759.html)

## 待封装集成的软件
- [GoRuntime_DirectX_9.0c运行库](https://www.itsk.com/thread-396895-1-1.html)
- [微软常用运行库合集](https://www.ghxi.com/yxkhj.html)
- [7zip](https://www.7-zip.org/)
- [Office2021](https://www.yrxitong.com/h-nd-1030.html)
- [PotPlayer](https://www.yrxitong.com/h-nd-287.html)
- [Chrome](https://www.ghxi.com/chrome.html)

## 制作一个用于封装的优启通PE镜像
下载官方最新版的优启通后打开`EasyU_v3.7.exe`，按照下图步骤制作ISO镜像。
![EasyU_v3.7.png](https://s2.loli.net/2023/04/24/SMlIZPfQNanh516.png)

## 安装[VMware-workstation-16](https://www.ghxi.com/workstationlite.html)
打开[VMware-workstation-16](https://www.ghxi.com/workstationlite.html)安装包，依次点击下一步即可完成安装。

## 创建一个适合封装WIN10 64位系统的虚拟机环境
![](https://img.itsk.com/itkdx/attachment/forum/202201/11/205813j9hlfc9ea51h1ffz.jpg)
![](https://img.itsk.com/itkdx/attachment/forum/202201/11/205654gcunkikiquuuci1d.jpg)

## 虚拟机BIOS设置
1. 如下图，点击三角形旁边的下拉三角形选择打开电源时进入固件进入虚拟机BIOS。
![](https://img.itsk.com/itkdx/attachment/forum/202201/11/211739aho1oomvm5oegg9t.jpg)
2. 进入BIOS设置，定位到Advanced的I/O设置。
![](https://img.itsk.com/itkdx/attachment/forum/202201/11/211741qjknxe31oke3m94m.jpg)
3. 全部改为Disabled关掉不必要的东西，减少不必要的影响。
![](https://img.itsk.com/itkdx/attachment/forum/202201/11/211741n3h0qq2qrkh1005z.jpg)
4. 按主Shift+“+”或者点“-”设置CD-ROM为第一启动项，Hard Drive为第二启动项。
![](https://img.itsk.com/itkdx/attachment/forum/202201/11/211742telclz3vocb0w9fl.jpg)
5. 设置完成后按F10保存退出。
![](https://img.itsk.com/itkdx/attachment/forum/202201/11/211743moisovogvng691vz.jpg)

## 精简[万能驱动](https://www.itsk.com/thread-428855-1-1.html)

## 复制软件至虚拟机D盘