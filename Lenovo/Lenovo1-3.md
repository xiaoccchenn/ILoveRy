   ## 联想篇1-3

* ##### 5.2.3xxxxx/5.2.2xxxxx

>接下来是关于联想平板破解的终极方法，它不受版本的限制，不受系统的限制，只要它的型号是**TB-X605M**，便可以使用接下来的方法)))

###  **需要准备的工具**

<details markdown='1'><summary>展开/收起</summary>


- [ ] Win10操作系统的PC一台

- [x] **QPST_2.7.496**

- [ ] 一根数据线

- [ ] 一台拆了后盖的平板

- [ ] 一根拿来短接用的回形针

- [ ] **prog_emmc_firehose_8953_ddr.mbn**(引导文件为绝密级，故请自行寻找，一般在刷机包里面会有)

- [x] [点击下载所有内容](https://wws.lanzoui.com/b02ckrf5c)

</details>

>首先在电脑解压并打开 ***"QPST_2.7.496"*** ,点击第一个文件夹 ***"Driver"*** ，执行 ***.exe*** 文件以安装高通驱动。

>驱动安装完成后重启电脑，并执行 ***"QPST.2.7.496.1.exe"*** 

>安装完成后，右下角打开最近添加中的 ***QPST*** ，打开 ***QPST*** ,如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/134416464364.png)

>此时标题显示的是 ***"No Port Available***" ,如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/OJ6PUSCGWH%5D%60Z%7D3V784YI_H.png)

>接下来是最关键的一步，首先将平板关机(一定要确保关机，或者直接将电池拆下后再装上)，此时已经默认你已经将后盖拆好

>找到短接点，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/1464164131436.png)

>先将数据线的一端连接电脑，再利用刚刚准备的回形针 ***短接*** 所示点位

>确保回形针的两端已经短接点位后的一瞬间，将数据线另一端插上平板，建议事先凑近充电口，且将线插入后，不要立刻松开回形针

>当电脑上的 **QFIL** 显示 ***Please Select an Existing Port*** 时，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/YF10AQ4PZ%24%7BE%5DTFCK_IZEKC.png)

>恭喜你成功进入了 ***9008模式*** !! 此时选择对应的9008端口即可

>接下来的步骤就十分轻而易举了，左上角选择 ***Flat Build*** ，在第一框框里点击 ***Browser*** ，打开mbn文件，如图:

![](https://github.com/Shelterforyou/ILoveRy_Pics/blob/main/468464446.png)

>最上面一栏中，选择 ***Tools*** ， ***Partition Manager***，点击打开分区表，滑到最后一个名叫 ***userdata*** 的分区

>右键该分区，选择第一个 ***Manage partition data*** ，再点击第一个 ***Erase***，等待一会后，若QFIL显示 ***Finish...***，则表示已清除数据分区

>最后一路close，，最后一个窗口点OK或者X都没有问题，等待平板震动后即可拔掉数据线，若平板长时间无反应，则长按 **电源键** 和 **音量下键** 直至震动

>一会后若平板出现彩色的圈圈，下方出现 **正在清空** 的字眼时，则表示你已经成功了!!

>大功告成!!