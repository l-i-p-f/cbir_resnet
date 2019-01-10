# CBIR

## A simple implementation of deep learning based cbir system
(基于深度学习的图像检索系统的简易实现)
=========================================================================

<p align="center"> 
<img src="https://github.com/l-i-p-f/cbir_resnet/blob/master/cbir_system.jpg">
</p>

Steps:
 1. Pretrain a classfication model.
 2. Use the pretrained model to extract features and construct a feature database.
 3. Input target image into the network to get features and compute cosine similarity with images in the database.
 4. Visualize the results.

Tools:
 - Deep learning framework: pytorch 0.4
 - Model: resnet-101
 - Dataset: cifar-100
 	- use training set to build feature database
 	- test set as source of target images

=========================================================================

该项目是本学期一个课程的大作业，适合练手。

可以熟悉\掌握：
 - pytorch官方提供的常见数据集和模型
 - 数据读取接口dataset、dataloader的使用
 - 模型结构修改、训练、保存、加载
 - 特征提取
 - 可视化
 - 模型简单，可以多调参、调优化器
 - ……
 
__神经网络版本的CBIR确实比我实现的平均哈希、感知哈希传统方法效果要好非常多。__
