# Iris-Pupil Ratio Detection using U-Net

## Overview

This project focuses on detecting and measuring the iris and pupil from an eye image using a deep learning-based U-Net model. The goal is to process images of eyes, accurately segment the iris and pupil, and compute their ratio. The model is designed for integration with live webcam feeds for real-time processing.

## Features

- **Deep Learning Model**: Utilizes a modified U-Net architecture for segmentation.
- **Three-Class Segmentation**: Background, Iris, and Pupil.
- **Input Compatibility**: Supports images from a webcam, phone, or file path.
- **Results Table**:
  - Right-side original image
  - Left-side original image
  - Right-side iris pupil detected image
  - Left-side iris pupil detected image
  - Ratio of iris to pupil for the right side
  - Ratio of iris to pupil for the left side

## Dataset

The project uses a pre-prepared dataset containing eye images for training and validation. The dataset includes masks with three classes: background, iris, and pupil.

## Model Architecture

- **Base Model**: U-Net with ResNet backbone
- **Modifications**: Changed from binary segmentation to multi-class segmentation (background, iris, and pupil)
- **Loss Function**: Suitable for multi-class segmentation (e.g., categorical cross-entropy)

## Installation & Requirements

To run this project, install the necessary dependencies:

```bash
pip install -r requirements.txt
```

Dependencies include TensorFlow, OpenCV, NumPy, and other necessary libraries.

## Usage

### Training the Model

1. Open the Jupyter Notebook and execute the training cells.

### Running Inference

To perform iris and pupil detection on an image:

```python
detect_iris_pupil('path_to_image.jpg')
```

### Live Webcam Integration

Future integration will allow real-time iris and pupil detection using a webcam.

## Output Example

- Original and segmented images will be displayed.
- The computed iris-to-pupil ratio will be outputted.

## Future Work

- Integrate with a live webcam feed
- Improve segmentation accuracy
- Optimize inference speed for real-time applications

## License

This project is open-source and available under the MIT License.
detect_iris_pupil('path_to_image.jpg')
pip install -r requirements.txt
