# Deepfake Image Dataset (DID)

## About the Dataset

### Overview

The **Deepfake Image Dataset (DID)** is a curated collection of real and artificially generated facial images designed to support deepfake detection research. It is developed for binary classification (**Real vs. Fake**) and supports modern deep learning architectures, particularly YOLO-based models.

### Motivation

With the rapid advancement of deep learning and generative AI, deepfake media has become increasingly realistic and difficult to detect. This dataset aims to support the development of robust and efficient detection systems that identify manipulated facial content and help address risks related to misinformation, identity theft, and digital fraud.

## Dataset Composition

The dataset contains two primary classes:

- **Real Images:** Authentic, unaltered human facial images collected from personal and publicly available sources.
- **Fake Images:** AI-generated or manipulated facial images divided into three complexity levels:
  - **Easy Fake:** Basic manipulations with visible artifacts, such as lighting mismatches and distortions.
  - **Mid Fake:** Moderately complex images combining real and AI-generated elements.
  - **Hard Fake:** Fully AI-generated images with high realism and minimal detectable artifacts.

## Dataset Distribution

| Subset     | Percentage |
| ---------- | ---------- |
| Training   | 80%        |
| Validation | 10%        |
| Testing    | 10%        |

Each subset maintains a balanced ratio of real and fake images.

## Annotations and Format

- **Annotation Format:** YOLO
- **Annotation Type:** Bounding-box-based labeling
- **Classes:**
  - `0` – Fake
  - `1` – Real

Images are annotated using tools such as Roboflow.

## Preprocessing and Augmentation

**Preprocessing**

- Resized to 512 × 512 pixels
- Auto-orientation applied

**Augmentation**

- Rotation, flipping, zoom, and shear
- Brightness, contrast, hue, and saturation adjustments
- Noise injection and blur effects

These techniques help improve model generalization and robustness.

## Key Features

- Multi-level fake categorization: Easy, Mid, and Hard
- Balanced training, validation, and testing splits
- YOLO-format annotations
- Suitable for real-time deepfake detection research
- Supports YOLOv8, YOLOv9, YOLOv10, and YOLOv11

## Applications

- Deepfake detection and classification
- Digital media forensics
- Facial forgery analysis
- AI-based cybersecurity systems
- Real-time content authentication

## Dataset Download

The dataset is hosted on Kaggle.

[**Download Deepfake Image Dataset (DID)**](https://www.kaggle.com/datasets/abdullah122/deepfake-image-dataset-did)

You can download it directly using KaggleHub.

**Install KaggleHub:**

```
pip install kagglehub
```

**Download the dataset:**

```
import kagglehub

path = kagglehub.dataset_download(
    "abdullah122/deepfake-image-dataset-did"
)

print("Dataset location:", path)
```

Kaggle authentication may be required before downloading.

## Intended Use

This dataset is intended for academic, educational, and research purposes. It can be used to develop, train, and evaluate deep learning models for detecting AI-generated and manipulated facial images.

## Citation and Acknowledgment

If you use this dataset in your research, please acknowledge the **Deepfake Image Dataset (DID)** and include a link to its Kaggle page.

## Author

**Abdullah Al Noman**

Research Interests: Deep Learning, Computer Vision, Artificial Intelligence, Medical Imaging, and Cybersecurity.
