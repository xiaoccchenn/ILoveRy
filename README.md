# ILoveRy
---

> 少年派速通教程，通，都能速通 

> 如有任何疑问，请向我发Email:h.shelter@outlook.com 

>每一part需要用到的工具中，标记▲为有提供的，标记△的请自行准备，默认下载密码:***RYNB*** ，另因有较大文件，将使用百度网盘分享，请提前准备)

---

# Project preview

## Unlock      
### (Attention!you must have a pad /xyx)  
Versions|Hardware|Unlock|Quickly_reach
--|:--:|:--:|:--:
**5.2.2xxxxx**|SM-P350|✔|[Go](#三星篇1-1)|
**5.2.3xxxxx**|SM-P350|✔|[Go](#三星篇1-2)|
**5.2.352411**|TB-X605M|✔|[Go](#联想篇1-1)|
**5.2.3xxxxx**|TB-X605M|✔|[Go](#联想篇1-2)|
**5.2.3xxxxx**|TB-X605M|✔|[Go](#联想篇1-3)|
**5.2.3xxxxx**|HUAWEI-C5|✔|[Go](#华为篇1)|

## Advanced_plays  
### (Attention!you must crack your pad before doing the followings)                            
Hardware|Root&Twrp|Quickly_reach|Hide|Quickly_reach|Double_OS|Quickly_reach|Login|Quickly_reach
--|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:
**SM-P350**|✔|[Go](#Root-for-SM-P350)|✔|[Go](#Hide-for-SM-P350)|✖|◾|✖|◾|
**TB-X605M**|✔|[Go](#联想篇2-1)|✔|[Go](#Hide-for-TB-X605M)|✔|[Go](#Double-OS-for-TB-X605M)|✖|◾|
**The-Third-Device**|✖|◾|✖|◾|✖|◾|✔|[Go](#How-to-login-in-the-third-device)|

# Let's start our journey ------ **Unlock!!**
   #  三星篇

##  三星篇1-1  

[(Back to top)](#Project-preview) 

* ##### 5.2.2xxxxx
5.2.2开头的版本，目前网上已有许多教程，故不详细展开，只提供思路，思路如下：
 
利用fiddler等抓包工具，替换书包里面的应用为设备管理器.

详细教程请前往 [Wtrwx的Blog](https://wtrwx.github.io/20200206/snpcrack.html)

##  三星篇1-2 

 [(Back to top)](#Project-preview) 

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

   #  联想篇
   
  [(Back to top)](#Project-preview) 
  
   相信大多数同学们的平板都是联想的TB—X605M，所以破解的需求面更为宽泛，其方法有三，且听我慢慢到来
   
   ## 联想篇1-1
   
  [(Back to top)](#Project-preview) 
      
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

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/468464.png)

>⇒点击最下面的mp4文件

>添加视频后，点开视频，选择打开安装包程序，进行安装

>⚠️⚠️你所安装的DevicePolicyManager.apk的包名必须修改为你书包中任意一个应用，如维词等，且安装前，要将原书包应用卸载⚠️⚠️
  
>安装完成后打开⇒ ***“激活设备管理器”*** ⇒ ***“恢复出厂设置”***

>大功告成！

   ## 联想篇1-2
   
   [(Back to top)](#Project-preview) 
      
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

   ## 联想篇1-3
   
   [(Back to top)](#Project-preview) 
   
* ##### 5.2.3xxxxx/5.2.2xxxxx
   
>接下来是关于联想平板破解的终极方法，它不受版本的限制，不受系统的限制，只要它的型号叫做TB-X605M，便可以使用接下来的方法)))

  **需要准备的工具**
  
>△Win10操作系统的PC一台
>
>▲QPST_2.7.496
>
>△一根数据线
>
>△一台拆了后盖的平板
> 
>△一根拿来短接用的回形针
>
>△prog_emmc_firehose_8953_ddr.mbn(引导文件为绝密级，故请自行寻找，一般在刷机包里面会有)
>
>[点击下载所有内容](https://wws.lanzoui.com/b02ckrf5c)

>首先在电脑解压并打开 ***"QPST_2.7.496"*** ,点击第一个文件夹 ***"Driver"*** ，执行.exe文件以安装高通驱动。

>驱动安装完成后重启电脑，并执行 ***"QPST.2.7.496.1.exe"*** 

>安装完成后，右下角打开最近添加中的QPST，打开QPST,如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/134416464364.png)

>此时标题显示的是 ***"No Port Available***" ,如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/OJ6PUSCGWH%5D%60Z%7D3V784YI_H.png)

>接下来是最关键的一步，首先将平板关机(一定要确保)，此时已经默认你已经将后盖拆好

>找到短接点，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/1464164131436.png)

>先将数据线的一端连接电脑，再利用刚刚准备的回形针 ***短接*** 所示点位

>确保回形针的两端已经短接点位后的一瞬间，将数据线另一端插上平板，建议事先凑近充电口，且将线插入后，不要立刻松开回形针

>当电脑上的QFIL显示 ***Please Select an Existing Port*** 时，如图:
 
![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/YF10AQ4PZ%24%7BE%5DTFCK_IZEKC.png)

>恭喜你成功进入了 ***9008模式*** !! 此时选择对应的9008端口即可

>接下来的步骤就十分轻而易举了，左上角选择 ***Flat Build*** ，在第一框框里点击 ***Browser*** ，打开mbn文件，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/468464446.png)

>最上面一栏中，选择 ***Tools*** ， ***Partition Manager***，点击打开分区表，滑到最后一个名叫 ***userdata*** 的分区

>右键该分区，选择第一个 ***Manage partition*** ，再点击第一个 ***Erase***，等待一会后，若QFIL显示 ***Finish...***，则表示已清除数据分区

>最后一路close，，最后一个窗口点OK或者X都没有问题，等待平板震动后即可拔掉数据线，若平板长时间无反应，则长按 ***电源键*** 和 ***音量下键*** 直至震动

>一会后若平板出现彩色的圈圈，下方出现 ***正在清空*** 的字眼时，则表示你已经成功了!!

>大功告成!!























# Get ready for the next journey ------ **Advanced_plays!!**

    恭喜你，成功克服了破解这一难题，现在的你，已经完全有能力迎接接下来的挑战，尽情显示破解之后的进阶玩法吧！
    
#  三星篇

##  三星篇2-1---Root!!

[(Back to top)](#Project-preview) 


#  联想篇

##  联想篇2-1

[(Back to top)](#Project-preview)

>接下来进入联想***TB-X605M***的***Root***环节。实际上，对于联想来说，破解绝非难事，反而如何获取超级管理权限是大家一直苦思的问题，但有了 ***9008*** 这一利器，这一切都显得轻而易举，让我们开始吧！


**需要准备的工具**
  
>△Win10操作系统的PC一台
>
>▲QPST_2.7.496--QFIL
>
>▲Adb集成工具
>
>▲Magisk_23.0
> 
>△一根数据线
>
>△prog_emmc_firehose_8953_ddr.mbn
>
>▲[点击下载所有内容](https://wws.lanzoui.com/b02cky3ah)

>首先开启平板的 ***USB调试*** ，使用数据线连接你的电脑，传输方式选择 ***MYP*** 

>电脑解压并打开 ***TOOLS_BY_CZ_V6.14.rar*** ,执行 ***CZ's Utility Tools V6.14.exe***

>此时平板会询问：***“是否允许进行USB调试*** (若没有弹出，请确保平板已开启USB调试)，点击允许

>若命令窗口显示 ***你的序列号 +device*** 则表示你已经成功连接电脑，如图：

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-29e1bac2d3267ea8.png)

>关闭该窗口，依次点击 ***线刷专区*** , ***EDL(9008)*** ，进入***9008***模式，如图

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/bed0c6af910fe98.png)

>进入后，最上面一栏中，选择 ***Tools*** ， ***Partition Manager***，点击打开分区表，找到名为叫 ***boot*** 的分区

>右键该分区，选择第一个 ***Manage partition*** ，再点击第二个 ***Read Data...***，如图：

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/f1cb897feb86966.png)

>等待一会后，若QFIL出现下图所示内容，则表明你已经成功读取***boot***分区的***img***文件

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-525022aad077396e.png)

>接下来便是找到存放该***img***的文件夹，根据QFIL的信息寻找即可，值得注意的是，一般情况下，***Appdata***文件夹是被隐藏了的，需要你手动开启查看隐藏文件夹才能看到

>将读取的***img***文件传输到手机

>此时手机安装并打开***Magisk_23.0***,首页点击第一个***安装***，下一步，在***方式***一栏里，选择***选择并修补一个文件***，如图：

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/63ced23e96605293.jpg)

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/4e923f9f823c89f7.jpg)

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/26fb9a23900439ac.jpg)

>找到并打开刚刚读取的***img***文件，等待修补完成，根据提示的生成路径找到修补后是***img***文件，并将其发送至电脑

>电脑接受完毕后，点击***Load Image***，找到并打开刚刚所接收的文件，并进行等待

>直到QFIL显示***Finish send image***时，点击***Close***

>滑动分区表至最后一个名叫 ***userdata*** 的分区

>右键该分区，选择第一个 ***Manage partition*** ，再点击第一个 ***Erase***，等待一会后，若QFIL显示 ***Finish...***，则表示已清除数据分区

>最后一路***Close***，，最后一个窗口点OK或者X都没有问题，等待平板震动后即可拔掉数据线，若平板长时间无反应，则长按 ***电源键*** 和 ***音量下键*** 直至震动

>一会后若平板出现彩色的圈圈，下方出现 ***正在清空*** 的字眼时，则表示你已经成功了***Root***

>大功告成！














