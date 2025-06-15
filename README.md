# 🧠 Brain Tumor Segmentation using U-Net
This project implements U-Net with ResNet50, VGG16, MobileNetV2, and EfficientNetB0 encoders to segment brain tumors from MRI images. It compares their accuracy, Dice scores, and efficiency, with ResNet50 achieving the best overall segmentation performance.

This project focuses on automated brain tumor segmentation from MRI scans using deep learning. It implements and compares four U-Net models with different encoder backbones: **ResNet50**, **MobileNetV2**, **VGG16**, and **EfficientNetB0**.

---

## 📌 Objective

- Segment brain tumor regions from MRI images.
- Compare performance of different pre-trained encoder backbones in U-Net.
- Evaluate using clinically relevant metrics.

---

## 🧪 Dataset

- **Source**: Custom 2D slices prepared from BRATS-style MRI datasets.
- **Structure**:
  - Images: `image_dataset/images/`
  - Masks: `image_dataset/masks/`
- **Size**: 128×128 pixels
- **Preprocessing**:
  - Normalization to [0, 1]
  - Augmentation: flips, rotations, noise

---

## 🏗️ Architecture

- **Base Model**: U-Net (encoder-decoder with skip connections)
- **Encoders**: 
  - ResNet50 🥇 (best accuracy & Dice)
  - VGG16
  - MobileNetV2 (lightweight)
  - EfficientNetB0 (balanced)

---

## ⚙️ Tech Stack

- TensorFlow 2.10.0
- Keras
- Python 3.8
- NumPy, Pandas, Matplotlib
- GPU: NVIDIA RTX 3070 Ti

---

## 🧮 Metrics

- **Accuracy**
- **Dice Coefficient**
- **Precision**
- **Recall**
- **Mean IoU**

---

## 🖼️ Visualizations

Prediction results are saved in the `segmentation_predictions/` directory:
- Input image
- Ground truth mask
- Predicted mask
