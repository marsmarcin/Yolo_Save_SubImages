将Yolo检测到的目标单独保存成图像

#0
==

确保安装了vs2015和opencv（我用的是opencv3.2.0）

#1
==

下载压缩文件，解压

#2
==

去 https://pjreddie.com/media/files/yolov2.weights 下载权重文件
把它放在...\build\darknet\x64\中

#3
==

打开darknet_no_gpu.sln

#4
==

再次确定opencv的包含目录和库目录没有问题

#5
==

debug x64

#6
==

shift+右键  打开powershell
输入 cmd
再输入 darknet_no_gpu.exe detector test data/coco.data cfg/yolo.cfg yolov2.weights -i 0 -thresh 0.25 dog.jpg

在results文件夹中会看到结果。
