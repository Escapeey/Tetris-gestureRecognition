# 基于手势识别的俄罗斯方块

手势识别分类模型采用resnet18,类别为5类，分别代表向左、向右、加速下落、旋转、原速下落

### 项目使用步骤
1. 运行DataCollect文件下的collectdata.py收集手势图像作为训练数据集
2. 将训练数据集按类别保存在trainDateset文件下，按类别分文件夹进行保存，共5类
3. 调用trainNet.py训练手势识别网络，采用5折交叉验证
4. 调用demo.py进行测试
5. 运行game.py


### Requirements
torch >= 1.6  
opencv-python == 3.4.2  
pygame == 2.4.0

### Explain
本项目基于github项目改进，源项目地址 https://github.com/CVMilk/Tetris-gestureRecognition
