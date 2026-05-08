# YOLO 目标检测
## 检测对象
**奶牛的行为：'drinking', 'eating', 'resting', 'standing', 'walking'**
## 模型训练32轮后的结果
- mAP50:0.904
- mAP50-95:0.785
## 使用
```powershell
yolo detect predict model=runs/detect/train/weights/best.pt source=测试图片.png
```

