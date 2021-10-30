# ILoveRy
---

> 少年派速通教程，通，都能速通 

> 如有任何疑问，请向我发Email:h.shelter@outlook.com 

>每一part需要用到的工具中，标记▲为有提供的，标记△的请自行准备，默认下载密码:***RYNB*** 。

---

# Project preview

## Unlock                                 
Versions|Hardware|Unlock|Quickly_reach
--|:--:|:--:|:--:
**5.2.2xxxxx**|SM-P350|✔|Method[1](#三星篇)|
**5.2.3xxxxx**|SM-P350|✔|?|
**5.2.352411**|TB-X605M|✔|?|
**5.2.3xxxxx**|TB-X605M|✔|Method[1](#联想篇1-2)、[2](#联想篇1-3)|

## Advantage_plays                              
Hardware|Rooted|Quickly_reach|Hide|Quickly_reach
--|:--:|:--:|:--:|:--:
**SM-P350**|✔|[Go](#Root-for-SM-P350)|?|?|
**TB-X605M**|✔|[Go](#Root-for-TB-X605M)|?|?|
**The-Third-Device**|✖️|✖️|?|?|

##  三星篇  

[(Back to top)](#ILoveRy) 
   
* ##### 5.2.2xxxxx
5.2.2开头的版本，目前网上已有许多教程，故不详细展开，只提供思路，思路如下：
 
利用fiddler等抓包工具，替换书包里面的应用为设备管理器.

详细教程请前往 [Wtrwx的Blog](https://wtrwx.github.io/20200206/snpcrack.html)

* ##### 5.2.3xxxxx
5.2.3开头的版本想必是大家最难找到方法的(除非你有RY的服务器证书和签名二维码的工具))) 

**下面便以5.2.352411版本为例(396以上版本通用)，为大家详细介绍))**

   **需要准备的工具**

- 一个智慧的大脑
> 
- 一点刷机的基础
> 
- 和机敏的判断力


  
首先，平板进入到安全模式(具体操作请自行探索)，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/54b836e2b2eba622.jpg)
  
进入后选择第一个选项 ***"重装少年派"***

点击后安装少年派，由于安卓5的特性)，安装速度极慢，所以点击安装后立刻进入 ***设置→锁定屏幕与安全→其他安全设定***

你会看到一个 ***加密设备*** 的选项，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/50b44710317830fd.jpg)
  
此时，在很短一段时间里 ***加密设备*** 是可以点击的(速度要快)
若无法点击则退出设置，重新安装少年派，重复上述过程。
进入 ***加密设备*** 后，你需要设置一种锁屏方式，随便设置一个密码后，点击 ***加密*** 即可。
如时间不够，可以先设置密码，再重复上述步骤再次进入进行加密。

>注意⚠️加密过程中，平板至少有 ***80%*** 的电量并且且平板外接电源，加密时不能重启平板或拔掉充电线，否则平板会变砖。

加密完成后打开平板，进入之前那个设置界面，此时会发现 ***加密设备*** 已变成了 ***解密设备*** ，点击 ***解密*** 
此时平板会重启，在重启过程中(提前准备好)同时按住音量—和电源键和HOME键15秒，强制重启以打断解密过程。
平板再次重启后就会进入另一个界面，届时会有一个 ***重置设备*** 按钮，点击即可将平板恢复出厂设置.

   #  联想篇1
   
   [(Back to top)](#ILoveRy) 
   
   相信大多数同学们的平板都是联想的TB—X605M，所以破解的需求面更为宽泛，其方法有三，且听我慢慢到来
   
   ## 联想篇1-1
   
   [(Back to top)](#ILoveRy)
   
* ##### 5.2.352411
   
>下面首先同样以5.2.352411版本为例(该方法仅适用于此版本)，展示一种独特的破解方法)))

  **需要准备的工具**
   
>△Win10操作系统的PC一台
>
>▲Fiddler抓包工具 
>
>▲DevicePolicyManager(ByShelter).apk
>
>△一台能开热点的手机
> 
>▲[点击下载所有内容](https://wws.lanzoui.com/b02ckj74f)
   
>事不宜迟，我们马上开始

>首先将 ***平板*** 和 ***电脑*** 连接到同一个网络下

>Win+R⇒键入"cmd"，回车⇒键入"ipconfig"，查看电脑的ipv4地址，如图(与下图有出入请忽略):

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-1deca77a9056d324.jpg)

>平板长按已连接的网络⇒修改网络⇒把代理改为手动⇒代理地址填上上一步获得的ip地址⇒端口填上**8888**⇒保存，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/6d4a7120a708f264.jpg)

>打开Fiddler⇒左上角tools⇒Options⇒弹出的六个选项全部勾上⇒切换到connection⇒四个选项全部勾上并确保端口为***8888***⇒点击OK⇒重启Fiddler

>准备工作已经就绪，下面开始抓包

>平板进入课堂实录，随便选择一个视频，点击

>此时Fiddler会弹出一些网址，选择网址左边是 ***绿色的下载*** 符号的网址右键⇒Copy⇒JustURL⇒点击复制

>进入Autorespond⇒点击Add Rule⇒此时会自动添加刚刚复制的url⇒点击第二栏最右边的▽⇒选择最后一个Searchfiles⇒自动索引打开文件资源管理器⇒找到并选择DevicePolicyManager.apk
  
>最后勾上 ***Enable rules*** 和 ***Allow all connects***

>平板点击 ***“下载当前视频”*** 此时将会下载DevicePolicyManager.apk

>等待进度条快速走完即可

>电脑关闭Fiddler，平板关闭代理

>接下来的操作全由平板进行

>随便点开自主学习的一个文件⇒批注⇒向左滑动 ***“其他”*** 一栏⇒选择 ***“视频”*** ⇒从文件选择⇒找到刚刚下载的视频，路径为(Andorid/data/com.netspace.myipad/cache)⇒滑动到最下面，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/58478c701bfe5bb5.jpg)

>⇒点击最下面的mp4文件

>添加视频后，点开视频，选择打开安装包程序，进行安装

>⚠️⚠️你所安装的DevicePolicyManager.apk的包名必须修改为你书包中任意一个应用，如维词等，且安装前，要将原书包应用卸载⚠️⚠️
  
>安装完成后打开⇒ ***“激活设备管理器”*** ⇒ ***“恢复出厂设置”***

>大功告成！

   ## 联想篇1-2
   
   [(Back to top)](#Contents)
   
* ##### 5.2.3xxxxx
   
>再次以5.2.352411版本为例(该方法适用于所有版本)，仍是一种独特的破解方法😀

  **需要准备的工具**
  
>▲DevicePolicyManager(ByShelter).apk
>
>△一个Outlook邮箱账号
>
>△一个网易邮箱账号
>
>△一台设置里有 ***电池*** 的平板
>
>▲[点击下载所有内容](https://wws.lanzoui.com/i4wwmvwlf2b)

>首先将少年派强行停止，然后找到设置⇒应用与通知⇒查看全部应用⇒右上角⇒显示系统进程⇒找到电子邮箱⇒电池⇒启动,如图所示:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-7e86494b79d8e812.jpg)

>下滑状态栏⇒截屏⇒分享⇒用电子邮件打开⇒使用Outlook邮箱账号登录(⚠️⚠️经过测试只能使用该邮箱)

>使用浏览器登录网易邮箱，选择发送附件到平板上登录的邮箱中

>接收后打开安装(同样注意包名问题)

>安装完成后打开⇒ ***“激活设备管理器”*** ⇒ ***“恢复出厂设置”*** ，如图所示:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-10d09111857b26d4.jpg)

>大功告成!



























