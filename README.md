# Yolo_Save_SubImages
Save the detected object images in a Yolo detection

#0
==

make sure you have installed visual studio 2015 and configuration opencv ( I use opencv3.2.0 and worked)

#1
==

download the zip file and unzip it.


#2
==

download the weights from https://pjreddie.com/media/files/yolov2.weights 

put it into ...\build\darknet\x64\


#3
==

in your...\build\darknet\
you will find a lot of sln files.
choose the "darknet_no_gpu.sln" open it with visual studio 2015

#4
==

check attributes for opencv

#5
==

debug or F5 

#6
==

in ...\build\darknet\x64\

open in powershell->cmd->darknet_no_gpu.exe detector test data/coco.data cfg/yolo.cfg yolov2.weights -i 0 -thresh 0.25 dog.jpg


it worked!

![Image text](https://github.com/marsmarcin/Yolo_Save_SubImages/blob/master/yolov3.gif)

