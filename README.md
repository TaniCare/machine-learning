# TaniCare: Plant Disease Classification

## Overview
TaniCare is a deep learning-based plant disease classification system that can identify various diseases in crops including Potato, Rice, Soybean, and Wheat. The project uses transfer learning with MobileNetV2 architectures to provide accurate disease detection and treatment recommendations.

## Features
- Multi-class disease classification for 4 major crops
- Disease detection and identification
- Treatment recommendations
- Comprehensive plant health maintenance guidelines
- Support for both English and Indonesian languages

## Supported Crops & Diseases
### Potato
- Early Blight (Alternaria solani)
- Late Blight (Phytophthora infestans)
- Healthy

### Rice
- Brown Spot (Bipolaris oryzae)
- Leaf Blast (Pyricularia oryzae)
- Neck Blast
- Healthy

### Soybean
- Caterpillar damage (Spodoptera litura)
- Leaf Beetle damage (Diabrotica speciosa)
- Healthy

### Wheat
- Brown Rust (Puccinia recondita)
- Yellow Rust (Puccinia striiformis)
- Healthy

## Technical Details

### Model Architecture
- Base Model: MobileNetV2/V3
- Input Size: 224x224x3
- Output Classes: 13

### Dataset
- Balanced dataset with ~900-1100 images per class
- Train/Validation/Test split: 60/20/20
- Data augmentation including:
  - Rotation
  - Width/Height shifts
  - Shear transformation
  - Zoom
  - Horizontal flip

### Performance
- Training accuracy: 0.8841
- Validation accuracy: 0.8884 
- Test accuracy: 0.8977

## Installation & Usage

1. Clone the repository:
bash
git clone https://github.com/[your-username]/TaniCare.git


2. Install dependencies:
bash
pip install -r requirements.txt


3. Run the notebook:
bash
jupyter notebook TaniCare_Final_Notebook.ipynb



## Model Training

The model was trained using transfer learning with the following steps:
1. Data preprocessing and augmentation
2. Class balancing
3. Transfer learning using MobileNetV2/V3
4. Fine-tuning with early stopping and learning rate reduction
5. Model evaluation and testing

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.


## Acknowledgments
- Dataset source: Kaggle Plant Disease Classification Dataset
- [Add any other acknowledgments]


---
Created as part of TaniCare Project