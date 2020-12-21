- [加群](#加群)
- [ubuntu知识点总结](#ubuntu知识点总结)

<a name="加群"></a>

来源：公众号|[3D视觉工坊](https://mp.weixin.qq.com/s/weShDMbGTf0amg1qu_t8cw)

![](imgs/公众号.jpg#center)

「3D视觉工坊」技术交流群已经成立，目前大约有12000人，方向主要涉及3D视觉、CV&深度学习、SLAM、三维重建、点云后处理、自动驾驶、CV入门、三维测量、VR/AR、3D人脸识别、医疗影像、缺陷检测、行人重识别、目标跟踪、视觉产品落地、视觉竞赛、车牌识别、硬件选型、学术交流、求职交流、ORB-SLAM系列源码交流、深度估计等。工坊致力于干货输出，不做搬运工，为计算机视觉领域贡献自己的力量！欢迎大家一起交流成长~

添加小助手微信：CV_LAB，备注学校/公司+姓名+研究方向即可加入工坊一起学习进步。

<img src="imgs/微信.jpg#" style="zoom:50%;" />

QQ群「3D视觉研习社」，群号：574432628

<img src="imgs/QQ群.jpg#" style="zoom:50%;" />

<a name="ubuntu知识点总结"></a>

#### ubuntu常用命令技巧

- $gnome-system-monitor    #系统监视器打开（类似任务管理器）

  

- $free -m #查看系统内存

  

- tar.gz文件压缩与解压

  - $tar -zxvf FileName.tar.gz  #解压

  - $tar -C DesDirName -zxvf FileName.tar.gz #解压到目标路径

  - $tar -zcvf FileName.tar.gz DirName  #将DirName和其下所有文件（夹）压缩

    

- md5sum #特点：md5sum校验，与文件名无关，仅与内容有关

  用法：#***表示文件

  $md5sum ***               

  ​            

- adb线的使用：

  - $lsusb  #查看usb端口

  - 如何利用adb线与电脑端进行文件传输？方法如下：

    文件打包完成后，回到PC的终端上，可以在任何你想存储数据的文件夹里新开一个终端：

     $adb pull  ***  #写清楚你要拖的东西在机器上的路径

  - 如何想在机器上拖电脑端的文件进行?

    $add push *** #在电脑端的文件路径

    $sync

     

- OpenCV的imshow()如何可以查看图片的像素值？

  编译OpenCV时，命令行终端：

  $cmake -DWITH_QT=ON ..



- 如果出现程序死机，该如何做？

  方法一：$ps aux|grep *** #程序名关键字

  ​                $kill -9 pid #代表程序的pid号

  方法二：$gnome-system-monitor #打开控制面板

- $sudo aptitude install *** #这里的aptitude比apt的优点是：可以解决一些依赖问题，但容易把系统搞崩。

  

- 如何快速地将终端文件输出到文本？

  方法一：exe ->log.txt 

   在当前位置打开终端，输入命令：$tail -f log.txt #可以动态查看log.txt的文件内容变化

  

- 如何将编译信息输出到文本？

  $make 2>&1|tee log.txt 

更新于2020年12月21日,后续持续完善。

备注：

1、[3D视觉招聘信息汇总](https://github.com/qxiaofan/awesome-Computer-Vision-Algorithm-Jobs)

2、[一个超干货的3D视觉学习社区](https://mp.weixin.qq.com/s/weShDMbGTf0amg1qu_t8cw)






