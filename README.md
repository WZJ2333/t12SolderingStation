# T12焊台

### 参考网址

原作者easyEda：[https://easyeda.com/wagiminator/z-solderingstation-smd-v2](https://easyeda.com/wagiminator/z-solderingstation-smd-v2)

github原项目地址：[https://github.com/wagiminator/ATmega-Soldering-Station](https://github.com/wagiminator/ATmega-Soldering-Station)

中文固件开发者：[https://github.com/createskyblue/ATmega-Soldering-Station](https://github.com/createskyblue/ATmega-Soldering-Station)

用Arduino烧录bootloader和固件教程：

[http://blog.sina.com.cn/s/blog_6f72ff900102xktj.html](http://blog.sina.com.cn/s/blog_6f72ff900102xktj.html)

[https://www.bilibili.com/video/BV1Sf4y167eS](https://www.bilibili.com/video/BV1Sf4y167eS)

[https://www.arduino.cn/forum.php？mod=viewthread&tid=100378&page=1&extra=#pid573426](https://www.arduino.cn/forum.php?mod=viewthread&tid=100378&page=1&extra=#pid573426)

[https://www.bilibili.com/video/BV1mt4y1i7GE](https://www.bilibili.com/video/BV1mt4y1i7GE)

[https://www.bilibili.com/video/BV1fy4y1y78x/](https://www.bilibili.com/video/BV1fy4y1y78x/)

b站参考视频：

[https://www.bilibili.com/video/BV1RD4y127BJ](https://www.bilibili.com/video/BV1RD4y127BJ)

[https://www.bilibili.com/video/BV1hU4y1h7u2](https://www.bilibili.com/video/BV1hU4y1h7u2)

[https://www.bilibili.com/video/BV1w7411W75V](https://www.bilibili.com/video/BV1w7411W75V)

[https://www.bilibili.com/video/BV1iE41137xJ](https://www.bilibili.com/video/BV1iE41137xJ)

### 需要额外购买的零件(BOM除外)

- 手柄套件
- 3D打印盒子
- 航空插 (GX12  4芯)
- DC 电源插座 (5.5 * 2.1 mm)
- DC电源适配器 (15V)
- 两脚开关 (KCD1 15 * 10 mm)（焊接开关的时候开关一定要处于断开状态，不然开关会被烫坏）
- 线 (截面积0.75m㎡)
- 4 个螺丝 (1.7 * 12 )
- OLED屏幕 (128x64    4个引脚,引脚要GND开头)
- 贴片编码器

### 硬件

手柄部分：

<img src="images/IMG_1139.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/IMG_1139.jpg" style="zoom: 50%;" />

<img src="images/IMG_1140.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/IMG_1140.jpg" style="zoom:50%;" />

<img src="images/IMG_1143.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/IMG_1143.jpg" style="zoom:50%;" />

<img src="images/IMG_1144.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/IMG_1144.jpg" style="zoom:50%;" />

<img src="images/IMG_1146.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/IMG_1146.jpg" style="zoom:50%;" />

<img src="images/IMG_1147.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/IMG_1147.jpg" style="zoom: 50%;" />

<img src="images/IMG_1148.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/IMG_1148.jpg" style="zoom:50%;" />

<img src="images/IMG_1149.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/IMG_1149.jpg" style="zoom:50%;" />

另外一种手柄的接法

<img src="images/74B851DB3E9C71AA91827E64F0BAFCEF.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/74B851DB3E9C71AA91827E64F0BAFCEF.jpg" style="zoom:50%;" />

<img src="images/F1E923BB9D348203B23AE3DA6A15FB74.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/F1E923BB9D348203B23AE3DA6A15FB74.jpg" style="zoom: 25%;" />





<img src="images/A903B9BE08AE4BF19E2100107DF49E19.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/A903B9BE08AE4BF19E2100107DF49E19.jpg" style="zoom:25%;" />

白色的线接金色引脚

<img src="images/05F9DCCB4003B5E63045A18BF5F77F9B.jpg" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/05F9DCCB4003B5E63045A18BF5F77F9B.jpg" style="zoom:25%;" />

焊台部分：

<img src="images/Snipaste_2021-07-10_11-06-27.png" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/Snipaste_2021-07-10_11-06-27.png" style="zoom: 25%;" />

### 固件

1、Arduino的IDE安装u8glib库和PID_v1等其他需要的库(可以直接在IDE中下载导入，也可以直接把库文件拖进ArduinoIDE的libraries文件夹中)

<img src="images/Snipaste_2021-07-10_21-03-04.png" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/Snipaste_2021-07-10_21-03-04.png" style="zoom: 33%;" />

<img src="images/Snipaste_2021-08-02_20-12-19.png" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/Snipaste_2021-08-02_20-12-19.png" style="zoom:33%;" />

2、连接(ArduinoUNO连上 电脑 和 T12控制板的ICSP)

<img src="images/Snipaste_2021-07-10_15-21-55.png" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/Snipaste_2021-07-10_15-21-55.png" style="zoom: 25%;" />

3、新建ArduinoISP项目

<img src="images/Snipaste_2021-08-03_09-21-34.png" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/Snipaste_2021-08-03_09-21-34.png" style="zoom:25%;" />

先编译然后上传

<img src="images/Snipaste_2021-08-03_09-23-52.png" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/Snipaste_2021-08-03_09-23-52.png" style="zoom:25%;" />

4、点击烧录引导程序(bootloader)，到T12的主控(ATMEGA328P)中，成功之后关掉这个项目

<img src="images/Snipaste_2021-08-03_09-25-25.png" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/Snipaste_2021-08-03_09-25-25.png" style="zoom:25%;" />

5、烧录固件

打开T12的源码，先点击编译，然后点击使用编程器上传，成功之后T12焊台的屏幕会被点亮

<img src="images/Snipaste_2021-08-03_09-27-36.png" alt="T12%E7%84%8A%E5%8F%B0%20b157d01f9ea6403abac089e03313d03d/Snipaste_2021-08-03_09-27-36.png" style="zoom:25%;" />