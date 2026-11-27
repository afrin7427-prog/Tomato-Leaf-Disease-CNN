
# 🍅 Tomato Leaf Disease Classification Using CNN

## 📌 Project Overview

This project focuses on developing a Convolutional Neural Network (CNN) model to classify tomato leaf images into six different categories, including healthy leaves and diseased leaves.

The model is developed using **PyTorch** and trained on a tomato leaf image dataset. The main objective is to identify tomato leaf diseases automatically using deep learning and image classification techniques.

**Project Status:** 🚧 Work in Progress

## 🎯 Objectives

- Develop a CNN-based tomato leaf disease classification model.
- Classify tomato leaves into six different categories.
- Apply image preprocessing and data augmentation.
- Improve model generalization using Dropout.
- Evaluate model performance using accuracy, loss, and confusion matrix.
- Explore further improvements and optimization techniques.

## 📂 Dataset Information

The dataset contains three separate subsets:

| Dataset | Number of Images |
|---|---:|
| Training | 4,586 |
| Validation | 981 |
| Testing | 990 |
| **Total** | **6,557** |

### Classification Categories

The model identifies the following six classes:

1. Tomato Bacterial Spot
2. Tomato Early Blight
3. Tomato Late Blight
4. Tomato Leaf Mold
5. Tomato Septoria Leaf Spot
6. Tomato Healthy

## 🛠️ Technologies & Libraries

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## 🧠 Model Architecture

A custom CNN architecture is implemented with three convolutional blocks and fully connected layers.

| Layer | Configuration |
|---|---|
| Input | 128 × 128 × 3 |
| Conv Layer 1 | 32 filters, 3 × 3 |
| Max Pooling 1 | 2 × 2 |
| Conv Layer 2 | 64 filters, 3 × 3 |
| Max Pooling 2 | 2 × 2 |
| Conv Layer 3 | 128 filters, 3 × 3 |
| Max Pooling 3 | 2 × 2 |
| Fully Connected 1 | 256 neurons |
| Dropout | 0.5 |
| Output Layer | 6 neurons |

**Total Trainable Parameters:** 6,517,574

## ⚙️ Data Preprocessing & Augmentation

The following preprocessing techniques are applied:

- Image resizing to 128 × 128 pixels.
- Random horizontal flipping.
- Random rotation (10 degrees).
- Conversion of images into PyTorch tensors.
- Image normalization using mean = 0.5 and standard deviation = 0.5.

Data augmentation is applied to the training dataset to increase image diversity and improve model generalization.

Validation and test images use resizing, tensor conversion, and normalization without random augmentation.

## ⚡ Training Configuration

| Parameter | Value |
|---|---|
| Optimizer | Adam |
| Learning Rate | 0.001 |
| Loss Function | CrossEntropyLoss |
| Batch Size | 32 |
| Epochs | 20 |
| Dropout Rate | 0.5 |
| Image Size | 128 × 128 |
| Hardware | Google Colab GPU (CUDA) |

## 📊 Preliminary Results

The following results were obtained during the current training experiment.

| Evaluation Metric | Result |
|---|---:|
| Best Validation Accuracy | 96.74% |
| Best Validation Loss | 0.0969 |
| Test Accuracy | 95.05% |
| Test Loss | 0.1602 |

*Note: These are preliminary experimental results and may change as the project is further improved.*

## 📈 Model Evaluation

The model is evaluated using:

- Training and validation accuracy curves.
- Training and validation loss curves.
- Test accuracy and test loss.
- Confusion matrix.
- Individual image prediction.

## 💾 Model Saving

The trained model weights are saved in PyTorch format:

`tomato_leaf_cnn.pth`

## 🚀 How to Run

1. Open the project notebook in Google Colab.
2. Upload the tomato leaf dataset ZIP file.
3. Run the dataset extraction and preprocessing cells.
4. Initialize the CNN architecture.
5. Train the model using the training dataset.
6. Evaluate the model using validation and test datasets.
7. Generate performance visualizations and save the trained model.

## 🔄 Future Improvements

This project is still under development. Planned improvements include:

- Further CNN architecture optimization.
- Experimenting with different regularization techniques.
- Hyperparameter tuning.
- Improving model generalization.
- More detailed classification performance analysis.
- Exploring explainable AI (XAI) techniques.
- Comparing performance with other deep learning architectures.

## 📌 Current Project Status

**Work in Progress 🚧**

The initial CNN model has been implemented and evaluated. Further experiments and improvements are ongoing.

---

**Note:** This repository will be updated as the project progresses.
