## 三星篇2-1 
>
> 恭喜你成功翻越了破解三星这一座高山，来到了进阶玩法
> 与联想不同的是，想要获得**Root**权限，你首先得将**TWRP**刷入你的平板，事不宜迟，让我们开始吧
>
>### **需要准备的工具**
>
><details markdown='1'><summary>展开/收起</summary>
>
>
>- [ ] Win10操作系统的PC一台
>
>- [ ] 一根数据线
>
>- [x] [**Odin3&Drive-for-Samsang**](https://github.com/Shelterforyou/ILoveRy/raw/main/Zips/%20%E4%B8%89%E6%98%9Fusb%E9%A9%B1%E5%8A%A8%E5%8F%8Aodin3.1.zip)
>
>- [x] [**TWRP_3.1.1-1.tar**](https://github.com/Shelterforyou/ILoveRy/raw/main/Zips/%20twrp_3.1.1-1.zip)
>
>- [x] [**Magisk_22.0.zip**](https://github.com/Shelterforyou/ILoveRy/raw/main/Zips/%20magisk-v22.0.zip)
>
>- [x] [**TOOLS_BY_CZ_V6.14.rar**](https://github.com/Shelterforyou/ILoveRy/raw/main/Zips/%20tools_by_cz_v6.14.rar)
>
></details>
>
>>下面开始我们的第一步，解压并打开**驱动和Odin**所在的文件夹，继续解压两个压缩文件
>
>>执行**Samsung_USB_Drivers_for_Mobile_Phones_1.5.9.0.exe**，如图：
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/4f45d477ff3fcab7.jpg)
>
>>驱动安装完成后，打开**Odin3**所在的文件夹，并执行**Odin3 v3.12.5.exe**，打开**Odin3**，如图：
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/7dffcc2a53b3b0c5.jpg)
>
>>开启平板的 ***USB调试*** ，使用数据线连接你的电脑，传输方式选择 ***MTP*** 
>
>>电脑解压并打开 ***TOOLS_BY_CZ_V6.14.rar*** ,执行 ***CZ's Utility Tools V6.14.exe***
>
>>此时平板会询问：**“是否允许进行USB调试** (若没有弹出，请确保平板已开启 ***USB*** 调试)，点击允许
>
>>若命令窗口显示 **你的序列号+device** 则表示你已经成功连接电脑，如图：
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-29e1bac2d3267ea8.png)
>
>>关闭该窗口，依次点击 _**线刷专区**_ , _**Fastboot(BL)**_ ，进入_**Download**_模式，(没错就是这么神奇)，如图：
>
>![]()
>
>>此时你已经进入了**Download**刷机模式，根据平板上的提示，短摁**音量上**
>
>>再次用数据线连接平板与电脑，**Odin**便会出现**Added**的成功提示，如图：
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-664f53d24e3f890b.jpg)
>
>>解压并打开**TWRP_3.1.1-1.zip**，你会得到一个名叫**TWRP_3.1.1-1.tar**文件
>
>>单击**Odin**上的**AP**按钮，找到并打开刚刚的**TWRP_3.1.1-1.tar**文件，如图：
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/-c9b752a7490efb7.png)
>
>>点击**Odin**里的**Options**，取消选中**Nand Erase**和**Auto reboot**，如图：
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/3a6ce3a70b69b1be.jpg)
>
>>此时点击**start**开始刷入，等待一会后，若出现**Pass**的字样，如图，则说明你已经成功刷入了**SM-P350**的**TWRP**了，恭喜！！
>
>![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/2e2402ffcbc5980.jpg)
>
>>大功告成!!
