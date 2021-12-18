##  联想篇2-1

>接下来进入联想***TB-X605M***的***Root***环节。实际上，对于联想来说，破解绝非难事，反而如何获取超级管理权限是大家一直苦思的问题，但有了 ***9008*** 这一利器，这一切都显得轻而易举，让我们开始吧！

###  **需要准备的工具**

<details markdown='1'><summary>展开/收起</summary>


- [ ] Win10操作系统的PC一台

- [ ] **QPST_2.7.496--QFIL**

- [x] [**Adb**集成工具](https://github.com/Shelterforyou/ILoveRy/raw/main/Zips/%20tools_by_cz_v6.14.rar)

- [x] [**Magisk_23.0.apk**](https://github.com/Shelterforyou/ILoveRy/raw/main/Applications/Magisk_23.0.apk)

- [ ] 一根数据线

- [ ] **prog_emmc_firehose_8953_ddr.mbn**

</details>

>首先在电脑解压并打开 ***"QPST_2.7.496"*** ,点击第一个文件夹 ***"Driver"*** ，执行 ***.exe*** 文件以安装高通驱动。

>驱动安装完成后重启电脑，并执行 ***"QPST.2.7.496.1.exe"*** ，等待安装完成

>开启平板的 ***USB调试*** ，使用数据线连接你的电脑，传输方式选择 ***MTP*** 

>电脑解压并打开 ***TOOLS_BY_CZ_V6.14.rar*** ,执行 ***CZ's Utility Tools V6.14.exe***

>此时平板会询问：***“是否允许进行USB调试*** (若没有弹出，请确保平板已开启 ***USB*** 调试)，点击允许

>若命令窗口显示 ***你的序列号+device*** 则表示你已经成功连接电脑，如图：

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-29e1bac2d3267ea8.png)

>关闭该窗口，依次点击 ***线刷专区*** , ***EDL(9008)*** ，进入***9008***模式，如图

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/bed0c6af910fe98.png)

>进入后，打开 ***QFIL***，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/134416464364.png)

>最上面一栏中，选择 ***Tools*** ， ***Partition Manager***，点击打开分区表，找到名为 ***boot*** 的分区

>右键该分区，选择第一个 ***Manage partition*** ，再点击第二个 ***Read Data...***，如图：

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/f1cb897feb86966.png)

>等待一会后，若QFIL出现下图所示内容，则表明你已经成功读取***boot***分区的***img***文件

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-525022aad077396e.png)

>接下来便是找到存放该***img***的文件夹，根据QFIL的信息寻找即可，值得注意的是，一般情况下，***Appdata***文件夹是被隐藏了的，需要你手动开启查看隐藏文件夹才能看到

>将读取的**img**文件传输到手机

>此时手机安装并打开**Magisk_23.0**,首页点击第一个***安装***，下一步，在**方式**一栏里，选择**选择并修补一个文件**，如图：

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/63ced23e96605293.jpg)

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/4e923f9f823c89f7.jpg)

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/26fb9a23900439ac.jpg)

>找到并打开刚刚读取的**img**文件，等待修补完成，根据提示的生成路径找到修补后是**img**文件，并将其发送至电脑

>电脑接受完毕后，点击**Load Image**，找到并打开刚刚所接收的文件，并进行等待

>直到QFIL显示**Finish send image**时，点击**Close**

>滑动分区表至最后一个名叫 **userdata** 的分区

>右键该分区，选择第一个 **Manage partition** ，再点击第一个 **Erase**，等待一会后，若8888显示 **Finish...**，则表示已清除数据分区

>最后一路**Close**，，最后一个窗口点**ok**或者X都没有问题，等待平板震动后即可拔掉数据线，若平板长时间无反应，则长按 **电源键** 和 **音量下键** 直至震动

>一会后若平板出现彩色的圈圈，下方出现 **正在清空** 的字眼时，则表示你已经成功了**Root**

>大功告成！
