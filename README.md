- **Based on the YOLOv7 framework, Pure for improving YOLOv7**

### Install

Clone the version library and install requirements. txt in an environment with * * Python>=3.7.0 * *, including * * PyTorch>=1.7 * *.
$pip install - r requirements. txt # Install
```
###Training
```Bash
$Python train.py -- data coco128. yaml -- cfg configs/attention_ V7/yolov7_ CA. yaml # defaults to yolo
```
###Inference
`Detect. py 'runs inference on various data sources and saves the detection results to the' runs/detect 'directory.
```Bash
$Python detect. py -- source 0 # Webcam
Img. jpg # Image
Vid.mp4 # Video
Path/# folder
Path/*. jpg # global
```
###Fusion
If you use different models to infer the dataset, you can use the wbf.py file to integrate the results through weighted box fusion.
You only need to set the img path and txt path in the wbf.py file.
```bash
$ python wbf.py
```
_ExDark Dataset:[Link]：https://pan.baidu.com/s/1wfp4xJBSPKz-Qh2GLmDlrA [password]：83wo
Subdivide the low light conditions, such as whether it is twilight or nighttime, location (in or out), visibility of the light source, and type of light source (sun, artificial light)
12 categories: Bicycle, Boat, Bottom, Bus, Car, Cat, Chair, Cup, Dog, Motorbike, People, and Table
Data collection: online download, keywords (dark, low light, nighttime); Public datasets (PADCAL VOC, ImageNet, and COCO); Extracting from movies; Manual shooting
Annotations: manual annotations
_____________________________________________________________________


