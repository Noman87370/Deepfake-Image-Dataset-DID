# Deepfake Image Dataset (DID)

<p align="center">
  <a href="https://link.springer.com/article/10.1007/s10791-026-10477-3">
    <img src="https://img.shields.io/badge/Springer%20Nature-Published-blue?style=for-the-badge" alt="Published in Springer Nature">
  </a>
  <a href="https://doi.org/10.1007/s10791-026-10477-3">
    <img src="https://img.shields.io/badge/DOI-10.1007%2Fs10791--026--10477--3-green?style=for-the-badge" alt="DOI">
  </a>
  <img src="https://img.shields.io/badge/Journal-Discover%20Computing-orange?style=for-the-badge" alt="Discover Computing">
</p>

<p align="center">
  <strong>A curated dataset for deepfake detection using deep learning and YOLO-based models.</strong>
</p>

---

## Research Publication

This dataset is associated with the following peer-reviewed research publication:

**Paper Title:** A YOLO Enhanced Deep Learning Model for Efficient and Scalable Deepfake Detection for Real-Time Facial Forgery Recognition in Digital Media

- **Journal:** Discover Computing
- **Publisher:** Springer Nature
- **Publication Year:** 2026
- **DOI:** [10.1007/s10791-026-10477-3](https://doi.org/10.1007/s10791-026-10477-3)

<p align="center">
  <a href="https://link.springer.com/article/10.1007/s10791-026-10477-3">
    <strong>Read the Published Research Paper →</strong>
  </a>
</p>

---

## About the Dataset

### Overview

The **Deepfake Image Dataset (DID)** is a structured and curated collection of real and artificially generated facial images designed to support deepfake detection research. It is developed for binary classification (**Real vs. Fake**) and supports modern deep learning architectures, particularly YOLO-based models.

### Motivation

With the rapid advancement of deep learning and generative AI, deepfake media has become increasingly realistic and difficult to detect. This dataset aims to support the development of robust, scalable, and efficient detection systems capable of identifying manipulated facial content and helping address risks related to misinformation, identity theft, and digital fraud.

## Dataset Composition

The dataset contains two primary classes:

- **Real Images:** Authentic, unaltered human facial images collected from personal and publicly available sources.
- **Fake Images:** AI-generated or manipulated facial images divided into three complexity levels:
  - **Easy Fake:** Basic manipulations with visible artifacts, such as lighting mismatches and distortions.
  - **Mid Fake:** Moderately complex images combining real and AI-generated elements.
  - **Hard Fake:** Fully AI-generated images with high realism and minimal detectable artifacts.

## Dataset Distribution

| Subset | Percentage |
|---|---:|
| Training | 80% |
| Validation | 10% |
| Testing | 10% |

Each subset maintains a balanced ratio of real and fake images to support unbiased model training and evaluation.

## Annotations and Format

- **Annotation Format:** YOLO
- **Annotation Type:** Bounding-box-based labeling
- **Classes:**
  - `0` – Fake
  - `1` – Real

Images are annotated using tools such as Roboflow for classification and localization.

## Preprocessing and Augmentation

### Preprocessing
- Resized to 512 × 512 pixels
- Auto-orientation applied

### Data Augmentation
- Rotation, flipping, zoom, and shear transformations
- Brightness, contrast, hue, and saturation adjustments
- Noise injection and blur effects

These techniques help improve model generalization and robustness across different deepfake patterns.

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

**[Download Deepfake Image Dataset (DID) on Kaggle](https://www.kaggle.com/datasets/abdullah122/deepfake-image-dataset-did)**

### Download Using KaggleHub

Install KaggleHub:

```bash
pip install kagglehub
```

Download the dataset:

```python
import kagglehub

path = kagglehub.dataset_download(
    "abdullah122/deepfake-image-dataset-did"
)

print("Dataset location:", path)
```

Kaggle authentication may be required before downloading.

## Intended Use

This dataset is intended for academic, educational, and research purposes. Researchers can use it to develop, train, and evaluate deep learning models for detecting AI-generated and manipulated facial images.

## Citation and Acknowledgment

If you use this dataset in your research, please acknowledge the **Deepfake Image Dataset (DID)** and cite the associated research publication.

**Research Paper DOI:**  
https://doi.org/10.1007/s10791-026-10477-3

**Dataset Link:**  
https://www.kaggle.com/datasets/abdullah122/deepfake-image-dataset-did

## Author

**Abdullah Al Noman**

Research Interests: Deep Learning, Computer Vision, Artificial Intelligence, Medical Imaging, and Cybersecurity.

---

<p align="center">
  <strong>Deepfake Image Dataset (DID) | Research • AI • Computer Vision</strong>
</p>
