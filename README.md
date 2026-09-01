# Geospatial Image Segmentation

A geospatial deep-learning image segmentation project implementing modern segmentation architectures (U-Net, LinkNet, DeepLabV3+) to process overhead/satellite imagery and extract land-cover and feature masks.

---

## Overview

This repository contains Jupyter notebooks and workflows for semantic segmentation of geospatial imagery. It includes:

- Custom architecture explorations and implementations: U-Net, LinkNet, and DeepLabV3+
- Data preprocessing and augmentation pipelines for remote sensing images and masks
- Training, evaluation, and inference workflows
- Metric computation (IoU, Dice Coefficient, Accuracy) and prediction mask visualization

---

## Features

- **Multiple Segmentation Architectures:** Support for U-Net, LinkNet, and DeepLabV3+ backbones.
- **End-to-End Pipeline:** Data loading -> Preprocessing & Augmentation -> Model Training -> Evaluation -> Mask Visualization.
- **Remote Sensing Applications:** Land-cover classification, urban feature extraction, and environmental monitoring workflows.
- **Evaluation Metrics:** Quantitative evaluation using Intersection over Union (IoU), Dice Score / F1, and Pixel Accuracy.
- **Visualization:** Side-by-side comparison of original satellite imagery, ground-truth masks, and predicted segmentations.

---

## Project Structure

```
Geospatial-Image-Segmentation/
├── .env.example                           # Template for environment variables and paths
├── .gitignore                             # Git ignore rules for data, models, and secrets
├── Custom_UNet_LinkNet_DeepLapv3+.ipynb    # Architecture exploration and custom model training
├── LinkNet and UNet Trained Model.ipynb   # Evaluation and inference with trained models
├── requirements.txt                       # Project dependencies
└── README.md                              # Project documentation
```

---

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook, JupyterLab, or Google Colab
- GPU support recommended for model training

### Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/Someshwar54/Geospatial-Image-Segmentation.git
   cd Geospatial-Image-Segmentation
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On macOS/Linux:
   source venv/bin/activate
   ```

3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Configure environment variables:
   Create your local `.env` file from the provided template and configure your dataset paths, model directories, and training parameters:
   ```bash
   # On macOS/Linux:
   cp .env.example .env
   # On Windows PowerShell:
   Copy-Item .env.example .env
   ```

---

## Usage

1. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

2. Open one of the notebooks:
   - `Custom_UNet_LinkNet_DeepLapv3+.ipynb` - Train and compare custom U-Net, LinkNet, and DeepLabV3+ models.
   - `LinkNet and UNet Trained Model.ipynb` - Load trained checkpoints for evaluation and prediction visualization.

3. Follow the notebook workflow:
   1. **Load Dataset** - Import satellite or aerial images along with their segmentation masks.
   2. **Preprocess & Augment** - Resize, normalize, and augment image-mask pairs.
   3. **Train Models** - Fit selected architectures on training partitions.
   4. **Evaluate Performance** - Compute validation metrics including IoU, Dice Score, and Accuracy.
   5. **Visualize Predictions** - Generate and display predicted masks over original images for qualitative analysis.

---

## License & Attribution

Maintained by Om Roy. Available for research, educational, and non-commercial development.


