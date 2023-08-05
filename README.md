- **Based on the YOLOv7 framework, Pure for improving YOLOv7**

### 安装

在**Python>=3.7.0** 的环境中克隆版本仓并安装 requirements.txt，包括**PyTorch>=1.7**。

$ pip install -r requirements.txt  # 安装
```

### 训练

```bash
$ python train.py --data coco128.yaml --cfg configs/attention_v7/yolov7_CA.yaml #默认为yolo
```

### 推理

`detect.py` 在各种数据源上运行推理, 并将检测结果保存到 `runs/detect` 目录。

```bash
$ python detect.py --source 0  # 网络摄像头
                          img.jpg  # 图像
                          vid.mp4  # 视频
                          path/  # 文件夹
                          path/*.jpg  # glob
```

### 融合
如果您使用不同模型来推理数据集，则可以使用 wbf.py文件 通过加权框融合来集成结果。

您只需要在 wbf.py文件 中设置 img 路径和 txt 路径。
```bash
$ python wbf.py
```
_ExDark Dataset:[Link]：https://pan.baidu.com/s/1wfp4xJBSPKz-Qh2GLmDlrA [password]：83wo
Subdivide the low light conditions, such as whether it is twilight or nighttime, location (in or out), visibility of the light source, and type of light source (sun, artificial light)
12 categories: Bicycle, Boat, Bottom, Bus, Car, Cat, Chair, Cup, Dog, Motorbike, People, and Table
Data collection: online download, keywords (dark, low light, nighttime); Public datasets (PADCAL VOC, ImageNet, and COCO); Extracting from movies; Manual shooting
Annotations: manual annotations
_____________________________________________________________________


