# alexnet‑mnist‑gui‑matlab
MATLAB基于简化AlexNet实现MNIST手写数字识别，附带手写GUI交互界面，输出Top‑3预测结果。

## 项目简介
本项目使用MATLAB深度学习工具箱搭建简化版AlexNet卷积神经网络，在MNIST手写数字子集数据集上完成模型训练。
实现鼠标手绘数字GUI程序，对手绘图像做裁剪、居中预处理，输出Top‑3识别结果与对应置信度，为本课程实验项目。

## 运行环境
- MATLAB R2025a
- Deep Learning Toolbox

## 文件说明
- `cnn.m`：网络训练脚本，用于训练卷积神经网络模型
- `digit_gui.m`：手写数字识别GUI交互程序
- `mycnn_model.mat`：训练完成后导出保存的网络模型文件

## 使用步骤
1. 将全部代码放置在MATLAB同一工作文件夹
2. 准备MNIST子集数据集，修改`cnn.m`内数据集路径
3. 运行脚本 `cnn.m`，开始训练卷积网络
4. 训练结束保存模型，脚本末尾添加保存代码：
```matlab
% 将训练完成的网络net保存到本地
命令行运行save("mycnn_model.mat","net");
