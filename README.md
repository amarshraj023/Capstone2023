# An Intelligent Modular Real-Time Vision-Based System for Environment Perception

A significant portion of driving hazards is caused by human error and disregard for local driving regulations; consequently, an intelligent assistance system can be beneficial. Hence, we propose a vision-based modular package to ensure drivers’ safety by perceiving the environment. Each module is designed based on accuracy and inference time to deliver real-time performance. As a result, the proposed system can be implemented on a wide range of vehicles with minimum hardware requirements. Our modular package comprises four main sections: lane detection, object detection, segmentation, and monocular depth estimation. Each section is accompanied by novel techniques to improve the accuracy of others along with the entire system. Furthermore, a GUI is developed to display perceived information to the driver. 

![overall_diagram](https://user-images.githubusercontent.com/61879630/199366037-69f5a025-73d5-428b-a2de-5742532946d3.jpg)

## Inference
To run the program, first install the requirements using the code below:
```
$ pip install -r requirements.txt
```
Then create a folder named 'weights' in the main directory and download all the weights in [this](https://drive.google.com/uc?export=download&id=1X1uKaGENEBZamF6tOfx9eKLTIQLsBN5h) shared google drive folder.

Then, place your video in the main folder of this repo and then run the following command.
```
$ python main.py --video yourvideoname.mp4 [--save] [--noshow] [--output-name myoutputvideo.mp4] [--fps]
```
--save argument will save the output video.

--noshow will not show you a preview of the output.

--output-name will determine the name you want for your output video

--fps will plot the fps results on the output frames

"yourvideoname.mp4" is the name of your video file added to the main folder.
"myoutputvideo.mp4" is the name you want for your output video.

Afterwards, the program starts running and the output video will be saved in the specified directory. To view the output while running, do not use '--no-show' argument.

There you have it.





## Datasets

### Test Videos:
Please download from [here](https://drive.google.com/uc?export=download&id=1-bRFhDt5EZULnQaKO35U3oX-p6yZwteB).

### Sign Datasets:
1. Traffic-Sign Detection and Classification in the Wild [Link](https://cg.cs.tsinghua.edu.cn/traffic-sign/)
2. DFG Traffic Sign Data Set [Link](https://www.vicos.si/Downloads/DFGTSD#:~:text=Dataset%20consists%20of%20200%20traffic,around%207000%20high%2Dresolution%20images.&text=The%20images%20have%20been%20anonymized,with%20the%20EU%20GDPR%20legislation.)



