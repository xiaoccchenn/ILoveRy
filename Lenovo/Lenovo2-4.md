>## 联想篇2-3
>
>### 关于TB-X605M双系统数据分区的实现
>
>> 理论上来说，双系统的实现将破解之后的隐蔽性拉满
>
>> 一个**system**使用少年派上课，另一个**system**进行学习和娱乐
>
>>优点:隐蔽性拉满   
>
>>缺点:分割后的两个data分区各自的容量太少,在使用时内存消耗率太高
>
>>但以上都不是我们停止探索步伐的理由
>
>>我们马上开始
>
>### 实现一:刷入双系统
>
>#### **需要准备的工具**
>
><details markdown='1'><summary>展开/收起</summary>
>
>- [ ] Win10操作系统的PC一台
>
>- [x] **QPST_2.7.496--QFIL**
>
>- [x] Adb集成工具
>
>- [x] **Double_OS.img(bin)**
>
>- [ ] 一根数据线
>
>- [ ] **prog_emmc_firehose_8953_ddr.mbn**
>
>- [x] [点击下载所有内容](https://wwd.lanzoui.com/b02cky3ah)/[**Double_OS.img(bin)**](https://pan.baidu.com/s/1JiApvGrE3YdLGVcTFv6TGQ)
>
></details>
>
>>首先在电脑解压并打开 ***"QPST_2.7.496"*** ,点击第一个文件夹 ***"Driver"*** ，执行 ***.exe*** 文件以安装高通驱动。
>
>>驱动安装完成后重启电脑，并执行 ***"QPST.2.7.496.1.exe"*** ，等待安装完成
>
>>开启平板的 ***USB调试*** ，使用数据线连接你的电脑，传输方式选择 ***MTP*** 
>
>>电脑解压并打开 ***TOOLS_BY_CZ_V6.14.rar*** ,执行 ***CZ's Utility Tools V6.14.exe***
>
>>此时平板会询问：***“是否允许进行USB调试*** (若没有弹出，请确保平板已开启 ***USB*** 调试)，点击允许
>
>>若命令窗口显示 ***你的序列号+device*** 则表示你已经成功连接电脑，如图：
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-29e1bac2d3267ea8.png)
>
>>关闭该窗口，依次点击 ***线刷专区*** , ***EDL(9008)*** ，进入***9008***模式，如图
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/bed0c6af910fe98.png)
>
>>进入后，打开 ***QFIL***，如图:
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/134416464364.png)
>
>>最上面一栏中，选择 ***Tools*** ， ***Partition Manager***，点击打开分区表，找到名为**system**的分区
>
>> 右键该分区，点击第二个**Manage as Mixed...**,如图:
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/1.png)
>
>> 在**Number of LBAs**处输入**11715600**，并点击一下**Start..**的方框(即输入值为**0**)，如图:
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/2.png)
>
>> 点击**Load image**，找到并打开**img**文件，然后等待
>
>> 若出现**Finish send image**时，如图:
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/3.png)
>
>> 则说明双系统已经成功刷入了你的平板，最后一路**close** ,直到平板震动，拔掉数据线
>
>> 长按音量下加电源键，等待平板震动松开即可
>
>> 大功告成!!
>
>### 实现二:双系统的切换
>
>>当你再次进入**9008**打开分区表，发现出现了**systema**和**systemb**时，则说明你已经成功刷入了**双系统**
>
>>刚刚刷完后，系统开机时，**默认**进入的是**systemb**，那么我们该如何在两个分割开的系统切换呢(老实说，你是不是想到了**8848钛金手机**))))
>
>>我们马上开始
>
>#### 法一:使用终端模拟器
>
>>此方法建立在你已经**Root**的基础上，若你还未**Root**，则请前往[法二](#法二)或者[Root](联想篇2-1)
>
><details markdown='1'><summary>展开/收起</summary>
>
>- [ ] **MT管理器**
>
></details>
>
>>打开MT管理器，它会请求获取超级管理权限，选择允许
>
>> 等待终端初始化完毕，确保显示如图：
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-67a7e3d8d287c19b.jpg)
>
>> 然后输入 **su**，回车，右边的 **"箭头"** 会变成 **"#"**，如图:
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/4438c08e853492a4.jpg)
>
>> 然后输入：
>
>```java
>    switchslot a//在systemb时 | switchslot b//在systema时
>```
>
>>切换成功后，输入
>
>```java
>    reboot
>```
>
>>此时重启后便会进入另一个**system**
>
>>大功告成!1
>
>#### 法二:使用第三方REC
>
>>此方法建立在你已经刷入**M_Twrp.img**，若你还没有刷入，请前往[Twrp](#联想篇2-2)
>
>#### 需要准备的工具
>
><details markdown='1'><summary>展开/收起</summary>
>
>- [ ]一台已经刷入**Twrp**的平板
>
></details>
>
>>关机状态下，长按三键，震动那一下，立刻松开按键
>
>>若屏幕出现大大的**TeamWin**，则说明你已经成功进入了第三方**REC**
>
>>点击**Mount**，挂载**system**和**vender**分区
>
>>点击**Terminal**，输入:
>
>```java
>    switchslot a(b)
>```
>
>>成功后退出，点击**reboot**，**reboot system**重启至另一个系统
>
>>大功告成!!