# alexnet‑mnist‑gui‑matlab
MATLAB基于简化AlexNet实现MNIST手写数字识别，附带手写GUI交互界面，输出Top‑3预测结果。

## 项目简介
本项目使用MATLAB深度学习工具箱搭建简化版AlexNet卷积神经网络，对MNIST手写数字数据集完成训练。
实现鼠标手绘数字GUI，对绘制图像做预处理，给出Top3识别结果与置信度，用于课程实验。

## 运行环境
- MATLAB R2025a
- Deep Learning Toolbox

## 文件说明
- `train_net.m`：网络训练脚本
- `digit_gui.m`：手写识别GUI程序
- `mycnn_model.mat`：训练完成保存的模型参数
- 实验报告、PPT：项目文档

## 使用步骤
1. 将全部代码放在同一文件夹
2. 在MATLAB加载训练模型：`load mycnn_model.mat`
3. 启动GUI界面：`digit_gui(net)`
4. 在画布鼠标手写数字，点击识别，查看Top‑3预测结果

## 注意
> 数据集文件较大，未上传至仓库，请自行准备MNIST子集数据集。
