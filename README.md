# Real-Time Crowd Density Estimation using Self-Distilled ResNet-50

## Overview

This project implements a deep learning-based crowd density estimation system using a **Self-Distilled ResNet-50** architecture. The model estimates crowd density maps and predicts the total number of people in an image while maintaining a lightweight architecture suitable for real-time applications.

The project is based on self-distillation using an Exponential Moving Average (EMA) teacher, eliminating the need for an external teacher network.

---

## Features

- Real-time crowd density estimation
- Self-distillation with EMA teacher
- ResNet-50 backbone
- Density map generation
- Crowd count prediction
- Works on both dense and sparse crowd scenes

---

## Dataset

This project uses the **ShanghaiTech Crowd Counting Dataset**.

- ShanghaiTech Part A
- ShanghaiTech Part B

> Dataset is not included due to its large size.

---

## Model Architecture

- Backbone: ResNet-50 (ImageNet Pretrained)
- Self-Distillation using EMA Teacher
- Density Map Regression
- Composite Loss:
  - Pixel-wise Density Loss
  - Count Loss
  - Self-Distillation Loss

---

## Results

| Dataset | MAE |
|---------|-----|
| ShanghaiTech Part A | 93.87 |
| ShanghaiTech Part B | 15.05 |

The proposed model achieves competitive performance while maintaining a simpler architecture compared to multi-column networks.

---

## Technologies Used

- Python
- PyTorch
- NumPy
- OpenCV
- Matplotlib
- Jupyter Notebook

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/crowd-density-estimation.git

cd crowd-density-estimation
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Usage

Open the notebook

```bash
jupyter notebook
```

Run

```
notebook.ipynb
```

---

## Repository Structure

```
Crowd-Density-Estimation/
│
├── notebook.ipynb
├── README.md
├── requirements.txt
├── images/
└── model/
```

---

## Future Improvements

- Video-based crowd counting
- Lightweight attention modules
- Model pruning and quantization
- Edge device deployment

---

## Author

Priyanka Channappa Badiger

Project developed as part of the Machine Learning & Deep Learning course.
