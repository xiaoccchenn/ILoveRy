## 番外篇1

### How to **INSTALL** applications when you were unlocked in **TB-X605M** 

> 经过探索，也算是解决了这令人头疼的问题

> 即使觉得这个方法有点点笨拙，但还是要拿出来分享给大家

> 话不多说，我们马上开始

### **需要准备的工具**

<details markdown='1'><summary>展开/收起</summary>
- [x] [**Myipad_Plugin.apk**](https://github.com/Shelterforyou/ILoveRy/raw/main/Applications/MyiPad%20Plugin_0.2.apk)


- [x] [**Lsposed.apk**](https://github.com/Shelterforyou/ILoveRy/raw/main/Applications/LSPosed_v1.5.2.apk)

- [x] [**Magisk_23.0.apk**](https://github.com/Shelterforyou/ILoveRy/raw/main/Applications/Magisk_23.0.apk)

- [x] [**Riru-v26.1.3.r513.8e95115fd4(513).zip**](https://github.com/Shelterforyou/ILoveRy/raw/main/Zips/%20riru-v26.1.3.r513.8e95115fd4(513).zip)

- [x] [**Riru_-_LSPosed-v1.6.2_(6152)(6152).zip**](https://github.com/Shelterforyou/ILoveRy/raw/main/Zips/%20riru_-_lsposed-v1.6.2_(6152)(6152).zip)

- [ ] **VMOS.apk(酷安)**

</details>

> 首先将平板刷入**lsp**，并在**lsp**激活**应用管理.apk**模块和**Plugin.apk**(激活后需要重启)，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/11111.png)

> 然后打开**应用管理.apk**，依次点击"**进阶**"，"**移花接木**"，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/22222.png)

> 右下角添加，依次输入如图所示的内容:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/33333.png)

> 保存后打开少年派(打开之前请务必确认已经刷入**Plugin**模块)

> 输入密码进入少年派主界面后，依次点击"**台灯**"， "**高级**"， "**壁纸**"， 进入**少年派内置终端**，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/44444.png)

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/55555.png)

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/66666.png)

> 然后在终端输入:

```java
X605M:/ $ su
```

> Magisk会请求允许获取超级管理权限，允许后返回:

```JAVA
X605M:/ # 
```

> 准备工作已经完成

> 那么我们如何在锁了之后，继续安装想要下载的应用呢?

> 通过上述所及方式进入少年派的终端，使用**Root**身份输入:

```java
X605M:/ # pm enable com.xxx.xxx //此处输入VMOS的包名即可(lazy author...)
```

> 当返回:

```java
X605M:/ # .... state : enable 
```

> 你已经成功恢复!!!

> 然后我们就可以随心所欲地安装应用啦

> 大功告成!!
