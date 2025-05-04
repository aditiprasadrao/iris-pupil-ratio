# 👁️ Iris-Pupil Ratio Detection using U-Net

### 🎯 Real-Time Eye Segmentation and Ratio Measurement with Deep Learning

---

## 🌟 Overview

This project leverages the power of **deep learning** to accurately segment and measure the **iris** and **pupil** from eye images. Using a customized **U-Net** model, the system performs real-time **three-class segmentation** (iris, pupil, background), enabling precise **iris-to-pupil ratio** analysis — ideal for eye research, medical diagnostics, and smart vision systems.

---

## 🚀 Key Features

- 🔍 **Multi-Class Segmentation**: Accurately classifies pixels into **background**, **iris**, and **pupil**.
- 🧠 **Deep Learning Backbone**: Enhanced U-Net architecture with a ResNet backbone for robust feature extraction.
- 🖼️ **Image Input Flexibility**: Accepts inputs from webcam, mobile phone images, or file paths.
- 📊 **Results Dashboard**:
  - Left and right eye original images
  - Corresponding segmented images
  - Calculated **iris-to-pupil ratio** for both eyes

---

## 🧾 Dataset

We use a curated dataset of annotated eye images. Each sample includes a ground truth mask with three labeled regions:
- `0` - Background  
- `1` - Iris  
- `2` - Pupil

This structured format allows the model to learn fine distinctions between eye components.

---

## 🧠 Model Architecture

| Component        | Description                      |
|------------------|----------------------------------|
| **Base Model**   | U-Net                             |
| **Backbone**     | ResNet (e.g., ResNet-34/50)       |
| **Segmentation** | 3-class (background, iris, pupil) |
| **Loss Function**| Categorical Cross-Entropy         |

> ✅ Optimized for pixel-wise classification and multi-class segmentation tasks.

---

## ⚙️ Installation & Setup

Clone the repository and install dependencies:

```bash
pip install -r requirements.txt
