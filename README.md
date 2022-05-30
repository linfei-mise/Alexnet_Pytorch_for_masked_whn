## 该文件夹是用来存放模式识别作业——alexnet模型文件的目录
### 下面将针对子文件夹及模型文件进行简单的介绍： 
* （1）文件夹
```
├── conv_feature_map_results（analyze_feature_map.py脚本生成的部分特征图）
├── conv_kernel_weight_results（analyze_kernel_weight.py脚本生成的部分权重、偏置等直方图）
├── plot_img（传入TensorBoard进行可视化的图片，以及predict.py脚本单次预测的图片路径）
├── Post_experimental_processing（存放生成混淆矩阵及模型指标的脚本及图片）
├── runs（传入TensorBoard进行可视化的参数文件，通过train.py脚本生成）
└── tensorboard_results（TensorBoard可视化得到的结果图）
```
* （2）文件
``` 
├── AlexNet.pth（alexnet模型训练得到的权重文件）  
├── analyze_feature_map.py（生成特征图所应用的脚本）  
├── analyze_kernel_weight.py（生成直方图所应用的脚本）
├── class_indices.json（生成的json文件用于TensorBoard和predict.py中类别可视化索引）
├── data_utils.py（构建TensorBoard可视化的脚本）
├── model.py（alexnet模型文件）
├── model_analyze.py（alexnet模型分析文件，更改了正向传播过程，用于生成特征图和直方图）
├── predict.py（模型的预测脚本）
├── README.md（文件类型解释）
└── train.py（模型训练脚本）
```
### 权重文件获取链接
* （1）alexnet网络训练得到权重文件：[AlexNet.pth](https://drive.google.com/file/d/1qyTeYHcE2Ybm5xCh3b5Zf4MxyHjknLC2/view?usp=sharing)
### 信息及维护时间：
```
作者：林飞
创建：2022-05-17
更新：2022-05-22
目的：使用alexnet网络对Masked-Face-Dataset数据集进行训练，完成图像分类任务（是否带帽子）。
```
