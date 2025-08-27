# AlexNet Image Classification Project

This is a PyTorch-based implementation of the AlexNet network for classification tasks on the Fashion-MNIST dataset. The project includes complete training, validation, and evaluation workflows.

## Project Features

- Uses the classic AlexNet architecture for image classification
- Supports loading and automatic partitioning of the Fashion-MNIST dataset
- Provides model training, validation, and testing capabilities
- Visualizes accuracy and loss curves during training

## File Structure

- `dataset.py`: Dataset loading and partitioning
- `model.py`: Definition of the AlexNet architecture
- `train.py`: Implementation of training and validation workflow
- `evaluate.py`: Model evaluation module
- `checkpoints/`: Directory for saving models
- `results/`: Directory for outputting training result images

## Usage Instructions

### 1. Install Dependencies

Please ensure the following libraries are installed:

- PyTorch
- torchvision
- matplotlib

You can install them using the following command:

```bash
pip install torch torchvision matplotlib
```

### 2. Train the Model

Run the `train.py` file to start training:

```bash
python train.py
```

The training process will automatically partition the dataset into training and validation sets, and save the model upon completion.

### 3. Evaluate the Model

Use `evaluate.py` to evaluate the model:

```bash
python evaluate.py
```

### 4. Visualize Training Results

Training records accuracy and loss metrics. Use the `matplot_acc_loss` function in `train.py` to plot the training curves.

## Model Architecture

This project implements the classic AlexNet architecture suitable for image classification tasks. The default output class count is 10, appropriate for the Fashion-MNIST dataset.

## Dataset

The project uses the Fashion-MNIST dataset, which contains 7,000 images per category across 10 classes of clothing items. The dataset will be automatically downloaded and partitioned.

## Results

After training, the accuracy and loss curves will be saved in the `results/` directory, with filenames in the format `train_curves_YYYYMMDD_HHMMSS.png`.

## Contribution Guidelines

Pull requests and issue reports are welcome. Please maintain consistent coding style and provide clear commit messages.

## License

This project is licensed under the MIT License. For details, please refer to the LICENSE file in the repository.