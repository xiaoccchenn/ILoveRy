   ## 联想篇1-1 

* ##### 5.2.352411

>下面首先同样以**5.2.352411**版本为例(该方法仅适用于此版本)，展示一种独特的破解方法)))

###  **需要准备的工具**

<details markdown='1'><summary>展开/收起</summary>


- [ ] Win10操作系统的PC一台

- [x] Fiddler抓包工具

- [x] **DevicePolicyManager(ByShelter).apk**

- [ ] 一台能开热点的手机

- [x] [点击下载所有内容](https://wws.lanzoui.com/b02ckj74f)


</details>

>事不宜迟，我们马上开始

>首先将 **平板** 和 **电脑** 连接到同一个网络下

>**Win+R**⇒键入**"cmd**"，回车⇒键入"**ipconfig**"，查看电脑的**ipv4**地址，如图(与下图有出入请忽略):

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-1deca77a9056d324.jpg)

>平板长按已连接的网络⇒修改网络⇒把代理改为手动⇒代理地址填上上一步获得的**ip**地址⇒端口填上**8888**⇒保存，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/6d4a7120a708f264.jpg)

>打开**Fiddler**⇒左上角**tools**⇒**Options**⇒弹出的六个选项全部勾上⇒切换到**connection**⇒四个选项全部勾上并确保端口为***8888***⇒点击**OK**⇒重启Fiddler

>准备工作已经就绪，下面开始抓包

>平板进入课堂实录，随便选择一个视频，点击

>此时**Fiddler**会弹出一些网址，选择网址左边是 ***绿色的下载*** 符号的网址右键⇒**Copy**⇒**Justurl**⇒点击复制

>进入**Autorespond**⇒点击Add Rule⇒此时会自动添加刚刚复制的**url**⇒点击第二栏最右边的**▽**⇒选择最后一个**Search files**⇒自动索引打开文件资源管理器⇒找到并打开**DevicePolicyManager.apk**

> 选中**Allow all connections**

>######  平板点击 ***“下载当前视频”*** 此时将会下载DevicePolicyManager.apk

>等待进度条快速走完即可

>电脑关闭**Fiddler**，平板关闭代理

>接下来的操作全由平板进行

>随便点开自主学习的一个文件⇒批注⇒向左滑动 **其他** 一栏⇒选择 **视频** ⇒从文件选择⇒找到刚刚下载的视频，路径为**(Andorid/data/com.netspace.myipad/cache)**⇒滑动到最下面，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/468464.png)

>⇒点击最下面的**mp4**文件

>添加视频后，点开视频，选择打开安装包程序，进行安装

>⚠️⚠️你所安装的**DevicePolicyManager.ap**k的**包名**必须修改为你书包中任意一个应用的包名，如维词等，且安装前，要将原书包应用卸载⚠️⚠️

>安装完成后打开⇒ **“激活设备管理器”** ⇒ **“恢复出厂设置”**

>大功告成！
