# 个 人 简 历

## 个人资料
```
姓  名：黄 李 全                       籍  贯：广东湛江
出  生：1992-11-06
政治面貌：团 员                         民  族：汉  族                          学  历：本 科
毕业院校：太原工业学院        专  业：自动化
邮  箱：846863428@qq.com      手  机：15220187476
工作经验：6年+
```

## 大学教育

|开始时间|结束时间|学校名称|
|------|:-----:|------:|
|2012.09|2016.07|太原工业学院|


## 工作经历

|开始时间|结束时间|公司名称|
|------|:-----:|------:|
|2021.05|2022.12|深圳乐动机器人股份有限公司|
|2017.08|2021.05|广州极飞科技有限公司|
|2016.07|2017.07|骏晨科技有限公司|

## 职业技能

* 嵌入式操作系统 linux(openwrt,buildroot,yocto)、freertos；
* 编程语言 c/c++、python、rust、汇编、html、node.js；
* 应用软件  libusb、live555、frp、ffmpeg、protocbuf、openssl、VPN等;
* 硬件相关 arm(ti am335x, nxp imx6ull/imx8mm/imx8mp, 全志v3s/f1c200s/H3/H5/R328, amlogic A311D, SigmaStar ssd222d, qca ipq40xx)、mips/mipsel(mtk 7688/7628, Atheros 9432/9531)、mcu（stm/51/esp32)、risc-v(全志 D1/D1s)。

## 项目经验

### 乐动机器人
深圳乐动机器人有限公司是一家做机器人的公司，尤其擅长扫地机器人领域

#### 运用技术
c++、python3、zmq、protobuf3、共享内存、多进程管理、多地图管理，涂鸦IOT SDK、阿里IOT SDK, 华为hilink SDK

#### 负责工作
1. 扫地机器人应用逻辑，任务调度，交互子系统，定时子系统，上位机调试等系统设计

该工作主要设计机器人的系统设计，感知系统，调度算法等知识。

2. 搭建机器人交互系统

包括按键输入系统，灯光交互系统，语音交互，tft显示屏等。

3. 处理iot接口以及app数据

包括阿里，涂鸦，华为hilink等iot平台。对各家iot有一定的了解，包括IOT SDK移植，SDK接入的方式方法，数据上下行格式，以及如何给设备授权，后台如何进行调试等。

4. python解析

处理一些机器人模型配置解析。构建机器人系统，会接入平台，需要python对机器人模型进行解析

5. 网络子系统开发

一个支持多家IOT切换的子系统开发，将设备层和IOT或调试上位机接口隔离，也就是适配器模式，以更加方便各种IOT接入或上位机调试，虽然没有达到“机器人开发SDK”级别，但通过此项目的支撑，极大方便了新人或对接人员的开发效率。

6. 无线通讯接口开发

主要有wifi,蓝牙，433等无线通讯模块接口开发，以达成基站与机器人通讯，app获取机器人无线网路状态等接口

7. 可定制的机器人平台搭建

由于面向的客户多且杂，一对一的对接客户的做法效率较低，需要通过一系列的抽象接口，将机器人拆解成各个部件，统一的逻辑由代码控制，对于差异化客户定制，每个部件对外提供参数配置，用户可以在机器人后台按照自己的想法去构建一类机器人，以达到更灵活的定制目的，自去年立项到今日，已量产多款机型，性能稳定

8. 数据埋点功能开发

通过埋点数据，记录设备的各种操作，以分析用户行为，进而根据用户的喜好，定向优化体验

* 工作心得
在乐动一年多的职业生涯里，对C++，python有更深入的理解，面向对象编程的概念也更深入，了解各种设计模式，养成在开发前的系统设计习惯。工作工程中参与了机器人架构设计。对机器人的各种边界有更深入的了解，机器人的感知系统，让机器可以感知环境变化，slam建图，让机器记录环境，以便于下次执行任务，能够快速决策，提前规划高效作业路线，应激系统，机器人的基础反射，系统调度，机器人作业的各个阶段，需要处理的问题具体化，制定相对策略。

### 广州极飞科技有限公司

极飞科技是一家农业无人机生产及研发公司，通过研究无人机、物联网、云计算和人工智能技术，不断为人类简化生产方式让农业变得更智能、更高效、更环保。

#### 运用技术
openwrt-18.06机型适配 + RGMII/MII驱动移植 + AR934X高速串口驱动开发 + 无线射频校准软件移植(nart) + wifi图传方案 + 网络应用(mesh下的网络设备管理)；

#### 负责工作
1. 针对AR9342的openwrt移植，适配软硬件

主要是增加新的机型，并驱动相关外设，具体内容后面展开。

2. AR9342的u-boot移植及开发

摒弃高通的lsdk u-boot软件，基于pepe2k的开源代码（github地址https://github.com/pepe2k/u-boot_mod.git）开发一个可以通过web来升级AR934X的u-boot,并做了适配AR8035 phy芯片驱动。

3. 开发AR9342的高速串口驱动

AR934x高速串口相关的资料并不多，应该是用的人不太多，非路由行业必需。所有根据芯片手册，通过用户态驱动的方式摸清楚高通的高速驱动原理，最终在内核文件里面找到一份不起眼的驱动代码，适配串口到PIN，最终完成驱动的注册。

4. RGMII/MII驱动

这个部分有点复杂，移植了高通LSDK的相关驱动代码，但linux内核的更新导致很多老的接口要重新做适配，通过一段时间查找内核补丁的方式，将lsdk的上古代码艰难的移植到openwrt-18.06,后面再做相应的优化工作，终于可以稳定的在openwrt-18.06上运行，可以驱动AR8035芯片（可以适配更多的phy,但只用了AR8035）,并且可以跟STM32F407通过MII-MII通信，不需要phy芯片参与。

5. 尝试性的开发AR9342的usb device驱动

AR934x的usb比较奇特，可以做host,也可以做device,但不是otg。Host驱动openwrt自带，但device驱动没有，也没什么人在用。在lsdk中找到相应代码并移植到openwrt-18.06,但不是项目必须也就没继续研究。

6. 移植OpenWRT下的ART驱动程序

无线芯片最重要的部分就是无线信号质量，每个无线芯片的rf都有差异，这就需要进行无线校准，这个是决定无线通讯质量的关键。首先移植art驱动的内核模块，移植过art2_ver_2_28,art2_ver_4_9_844,这些驱动都有些问题，新旧接口不通用，需要修改相应的接口来适配新的内核。第二部分就是校准程序nart的移植，这个部分代码量庞大，软件架构比较混乱不好维护。在openwrt的chaos_calmer下编译。可以正常运行校准，但是在openwrt-18.06后的版本，会出现一个芯片ID不识别的问题，导致校准程序不能运行，怀疑是把uclibc换成musl库的问题，openwrt-18.06不支持uclibc库，应该是两个C库在某个方面做了不同的处理，导致获取ID接口的结果不一致。解决的办法是在nart程序这边强制把芯片ID设置成0x31(AR9342 ID),校准程序可以正确运行。

7. 视频直播服务搭建

利用AR9342的usb,接入相机，9342 将相机识别成uvc设备，相机把压缩编码的码流通过uvc传进来，放入rtsp服务器。Rtsp服务基于live555开发，架构比较完善，功能比较齐全，但有个缺陷是编译固件占用了500KB左右的空间，对于16Mflash的wifi来说压力有点大，但视频服务正常，可稳定运行，支持多客户端接入。

8. wifi模拟软件无线电

利用wifi芯片，通过monitor模式，将数据通过fec编码直接将数据包发到空中，对端接收解码，可以可靠的收发文件，但缺点是AR9342的fec编解码效率低，做不了很深入的应用。

9. 高通ipq40xx平台开发

适配外设接口rgmii,sdio,i2c,spi nor/nand,wifi驱动ath10k适配等接口。4核cortex-a7性能比较强，做通讯的同时，可以做一些复杂算法的工作，特别适合开发软件无线电，处理一下复杂逻辑等工作，但是40nm的制程，让芯片发热比较严重。为了开发ipq平台，也编译过高铁官方SDK，QSDK5.3。

10. openwrt 适配 TI am335x

在通讯系统中包含了一块am3352的A8处理器作为系统的大脑，为了软件开发的统一，C库的兼容，决定将ti统一整合到我们的软件系统里面，我负责ti的软件移植工作，包括硬件适配，接口定义，bootloader补丁等工作，目前该平台已测试已经稳定，交付其他同事维护。

#### 架构师之路
2020 - 2021 嵌入式系统架构师

#### 运用技术
网络通讯，软件管理，云通讯网络，编程架构等

#### 工作目标
设计一套类似人脑一样的系统架构，让设备可以跟人一样思考，具有决策能力，执行能力等。其实是一种抽象化的系统，该系统为产品服务。需要调动研发部们所有智慧，为这样一个大脑服务。这个大脑包含部分有收集APP交互端，云服务器云通讯，机器人控制器大脑（业务开发的linux）+ 平衡设备的小脑（飞控）。设备通讯技术，无线局域网（mesh网络）+ 4G通讯，软件管理。统筹各个业务软件的开发，目前已经有十几个应用在跑。

#### 主要工作如下
对接芯片供应商，将SDK转话成自己的系统构建框架，实际上是一套基于buildroot的变形,加上自研的进程管理，网络通讯等接口，作为自主操作系统1.0版本，实际上1.0大多是linux应用，并没有太多自己的设计，年初开始规划2.0版本，但是由于公司的原因，很难推进，打算用于自己创造

引入go python等开发语言，属于公司嵌入式开发历史上的首次尝试，大获成功，地图开发相关人员由java转go，开发出高质量应用，目前装机稳定运行

配合我们的4G + wifi双向通路，进行终端无差别访问linux端的服务应用，应用无需知晓通讯细节，只认为自己是服务端应用，服务器和嵌入式很好的融为一体，可以兼容大多数互联网应用
跟进产品从设计到工厂生产的一整套流程，参与到一个产品从构思阶段，到发展成熟阶段，以及最终量产，客户问题跟进的每一个环节

设计并牵头实现多应用管理架构，在我们的操作系统里面，引入一个进程监控的应用，它可以监控系统硬件资源，软件健康状态，应用调试和升级等功能，是一个系统保姆的角色

带领一个还没毕业的小伙子，从接手项目到实际输出，用时1个半月，基于我们主导的系统框架，将A311D从底层到上层业务，工厂流程全部打通，对于使用原厂SDK的前人开发经验，基本算是降维打击，用时至少，质量之高。

以下是配合实现的内容，涉及部门间协作

飞控单片机通讯，将异构的串口通讯，转换成socket可以访问的接口

linux通讯，配合我们的云端通讯SDK，将网络通讯抽象化。

APP交互，对接通讯接口设计，定义通讯协议和事件类型。

参与云服务通讯框架设计，打造适合新设计的产品的通讯接口，保证多设备通讯稳定

参与固件升级服务框架设计，设计并实现新架构下的应用升级流程，方式和实现。

使用go语言建立地图服务，帮助java技术栈员工使用go语言，重构地图服务应用。

#### 经验总结
架构决定一切，一个复杂的系统一定不简单，一个人的能力肯定不够，需要一群志同道合的人一起，进行任务的分解，充分发挥各自的长处。身为架构师，一定不能只看到自己的专业领域这一小范围，一定要有足够广阔的视野，不管是技术层面，还是人事层面，或者社会层面。别人愿意跟着你干，一定是可以从你身上看到希望，或者可以学到知识，或者认为你能给他提供帮助。

### 深圳骏晨科技有限公司
方案公司。主要业务是芯片代理，wifi模块代理，提供无线视频传输方案，以及车联网方案

#### 运用技术
rtsp, socket, rtmp, http, openwrt, wifi, GPS差分定位;

#### 负责工作
1. 嵌入式系统软件的移植和开发，底层接口的调整；
2. 通过uvc接口，拉取USB摄像头输出的音视频，alsa接口拉取音频流，并使用faac将输出的PCM音频压缩成aac；
3. 解决音视频通过无线传输的同步及花屏卡顿问题；
4. 使用http协议，设备通过4G网络来和服务器进行交互，上传设备信息及下载资源；
5. 调用千寻提供的第三方SDK，把GPS数据推送到差分定位服务器，以获取差分定位数据。

#### 工作心得
1. 跨出象牙塔，对嵌入式系统开始有新的认识，充分了解arm处理器；
2. 调试wifi过程中了解到wifi的工作原理，性能参数，使用环境干扰，以及丢包和延时的检测方法；
3. 了解网络视频传输上面的一些难题，比如网络上传带宽的限制，必须提高视频压缩率，降低码流来解决；
4.	接触到之前没有使用过的操作系统openwrt,并对这个精简版本的linux操作系统产生浓厚兴趣，精简化的设计可以去除冗余，可以用它来制作精简，高效率的软件；
5.	掌握Linux系统下的文本编辑器VSC的使用，相对于主流的souce Insight来说更适合linux用户，也大大提高了代码开发效率。

### 擅长技能
* buildroot 深度定制
* openwrt 深度定制
* C/C++ 应用开发

### 社交
个人博客：http://blog.csdn.net/u013908686

github：https://github.com/MagicPrince666

### 求职意向
linux系统架构师

c/c++开发
