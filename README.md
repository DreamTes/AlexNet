# AlexNet 图像分类项目

这是一个基于 PyTorch 实现的 AlexNet 网络，用于对 Fashion-MNIST 数据集进行分类任务。项目包含完整的训练、验证和评估流程。

## 项目特点

- 使用经典的 AlexNet 网络结构进行图像分类
- 支持 Fashion-MNIST 数据集的加载与自动划分
- 提供模型训练、验证及测试功能
- 可视化训练过程中的准确率和损失曲线

## 文件结构

- `dataset.py`: 数据集加载与划分
- `model.py`: AlexNet 网络结构定义
- `train.py`: 训练与验证流程实现
- `evaluate.py`: 模型评估模块
- `checkpoints/`: 模型保存目录
- `results/`: 训练结果图像输出目录

## 使用方法

### 1. 安装依赖

请确保已安装以下依赖库：

- PyTorch
- torchvision
- matplotlib

可通过以下命令安装：

```bash
pip install torch torchvision matplotlib
```

### 2. 训练模型

运行 `train.py` 文件以开始训练模型：

```bash
python train.py
```

训练过程中会自动划分训练集和验证集，并在训练完成后保存模型。

### 3. 评估模型

使用 `evaluate.py` 对模型进行评估：

```bash
python evaluate.py
```

### 4. 可视化训练结果

训练过程中会记录准确率和损失，使用 `train.py` 中的 `matplot_acc_loss` 函数可绘制训练曲线。

## 模型结构

本项目实现的是经典的 AlexNet 网络结构，适用于图像分类任务。默认输出类别数为 10，适用于 Fashion-MNIST 数据集。

## 数据集

项目使用 Fashion-MNIST 数据集，包含 10 个类别的服装图像，每个类别有 7000 张图像。数据集会自动下载并划分。

## 结果展示

训练完成后，准确率和损失曲线将保存在 `results/` 目录下，文件名格式为 `train_curves_YYYYMMDD_HHMMSS.png`。

## 贡献指南

欢迎提交 Pull Request 或提出 Issue。请确保代码风格一致，并提供清晰的提交信息。

## 许可证

本项目遵循 MIT 许可证。详情请查看仓库中的 LICENSE 文件。