# YOLO 目标检测
## 概述
初步训练下，该模型具备对奶牛行为的检测能力。
## 检测对象

**奶牛的行为：'drinking', 'eating', 'resting', 'standing', 'walking'**

## 模型训练32轮后的结果

- mAP50:0.904
- mAP50-95:0.785

## 使用
```
yolo detect predict model=./datasets/runs/detect/train/weights/best.pt source=测试图片.png
```
### 检测结果位置：/runs/detect/train/predict-x

## 补充
1. 畜养环境不同，检测置信度差异较大，建议降低置信度
```
yolo detect predict model=./datasets/runs/detect/train/weights/best.pt source=测试图片.png conf=0.2 imgsz=1280
```
2. 针对不同畜养环境可将训练后的模型导出，根据不同环境制作对应的数据集进行训练
3. ~~数据集~~忽略







