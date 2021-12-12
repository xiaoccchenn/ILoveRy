##   联想篇2-2

> 接触过刷机的朋友们应该知道 **twrp**及其本身的魅力，作为一个主流第三方**REC**，他所拥有的强大的功能，为我们提供了许多便利

> 虽然官网只有**F**版本的**TWRP**，但在一位大佬@()的加工加点下，**TWRP-for-TB-X605M**终于成功问世

> 如何进入**REC**：平板关机后，三键同时按，屏幕亮后松开即可

> 下面为大家介绍两种刷入**TWRP**的方法

###  9008

> 首先同样还是**9008**的方法，这是你没有**Root**的前提下，所使用的方法，若你已经**Root**，则请移步[方法2](#dd命令)

###  **需要准备的工具**

<details markdown='1'><summary>展开/收起</summary>


- [ ] Win10操作系统的PC一台

- [x] **QPST_2.7.496--QFIL**

- [x] Adb集成工具

- [x] **M_twrp.img**

- [ ] 一根数据线

- [ ] **prog_emmc_firehose_8953_ddr.mbn**

- [x] [点击下载所有内容](https://wwd.lanzoui.com/b02cl58dc)

</details>

>首先在电脑解压并打开 ***"QPST_2.7.496"*** ,点击第一个文件夹 ***"Driver"*** ，执行 ***.exe*** 文件以安装高通驱动。

>驱动安装完成后重启电脑，并执行 ***"QPST.2.7.496.1.exe"*** ，等待安装完成

>开启平板的 ***USB调试*** ，使用数据线连接你的电脑，传输方式选择 ***MTP*** 

>电脑解压并打开 ***TOOLS_BY_CZ_V6.14.rar*** ,执行 ***CZ's Utility Tools V6.14.exe***

>此时平板会询问：***"是否允许进行USB调试"*** (若没有弹出，请确保平板已开启 ***USB*** 调试)，点击允许

>若命令窗口显示 ***你的序列号+device*** 则表示你已经成功连接电脑，如图：

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-29e1bac2d3267ea8.png)

>关闭该窗口，依次点击 ***线刷专区*** , ***EDL(9008)*** ，进入***9008***模式，如图

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/bed0c6af910fe98.png)

>进入后，打开 ***QFIL***，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/134416464364.png)

>最上面一栏中，选择 ***Tools*** ， ***Partition Manager***，点击打开分区表，找到名为 ***recovery*** 的分区

>右键该分区，选择第一个 ***Manage partition*** 

>点击***Load Image***，找到并打开**M_twrp.img**，并进行等待

>直到**QFIL**显示***Finish send image***时，一路点击***Close*** 和**OK**

>等到平板震动，拔开数据线，等待屏幕黑屏后，长按**电源键**和**音量下**，等到亮屏后松开即可

>大功告成!!

###  dd命令

> 相比于**9008**，使用终端命令就显得非常**easy**了，但前提是你已经获得了**Root**权限

###   需要准备的工具

<details markdown='1'><summary>展开/收起</summary>


- [x] MT管理器

- [x] **M_twrp.img**

- [x] [点击下载所有内容](https://wwd.lanzoui.com/b02cl58dc)

</details>

> 首先将**M_twrp.img**复制到**storage/emulated/0/Android**

> 然后打开MT管理器，它会请求获取超级管理权限，选择允许

> 然后进入到**storage/emulated/0/Android/**文件夹中，点击右上角的**•••**，点击 **打开终端**

> 等待终端初始化完毕，确保显示如图：

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-67a7e3d8d287c19b.jpg)

> 然后输入 **su**，回车，右边的 **"箭头"** 会变成 **"#"**，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/4438c08e853492a4.jpg)

> 然后输入：

```java
   dd if=M_twrp.img of=/dev/block/bootdevice/by-name/recovery
```

> 回车，然后等待一会即可

> 此时，你已经成功刷入了 **TB-X605M** 的 **TWRP**!!

> 大功告成!!