# Casting Product Quality Inspection

## Project Overview
This project focuses on automating the quality inspection process for casting products, specifically submersible pump impellers, using deep learning techniques. Manual inspection in the casting industry is time-consuming and prone to human error, which can result in significant financial losses. By leveraging state-of-the-art deep learning models, we aim to build an accurate and efficient defect detection system.

## Key Features
1. **Custom Implementation of ResNet:**
   - ResNet architecture variants were implemented from scratch using PyTorch in a modular manner, providing flexibility and scalability for future enhancements.

2. **Fine-tuned Pre-trained Models:**
   - Xception and DenseNet models were fine-tuned on the casting defect dataset to leverage the power of transfer learning and improve model performance.

3. **Dataset and Augmentation:**
   - The dataset consists of 7348 grayscale images of size 300x300. Images are categorized into two classes:
     - `def_front` (defective impellers)
     - `ok_front` (non-defective impellers)
   - Training data: 3758 defective and 2875 non-defective images.
   - Testing data: 453 defective and 262 non-defective images.

4. **Automation Goal:**
   - Develop a reliable classification system to distinguish between defective and non-defective products, minimizing human intervention and improving quality assurance.

## Dataset Details
### Context
Casting defects are undesired irregularities in the casting process that can lead to order rejections and financial losses. The goal is to automate the defect detection process for submersible pump impellers using machine learning.

### Dataset Structure
- **Training Dataset:**
  - `def_front`: 3758 images
  - `ok_front`: 2875 images
- **Testing Dataset:**
  - `def_front`: 453 images
  - `ok_front`: 262 images

### Data Characteristics
- Images are grayscale with a resolution of 512x512.
- Stable lighting conditions were ensured during image capture.
- Data augmentation was not applied to the provided dataset.

## Implementation
### Libraries and Tools
- **Framework:** PyTorch
- **Pre-trained Models:** Xception, DenseNet
- **Custom Implementation:** ResNet variants

### Methodology
1. Implemented ResNet architecture from scratch, ensuring modular design for flexibility.
2. Fine-tuned Xception and DenseNet models on the dataset to utilize pre-trained weights for better feature extraction.
3. Evaluated model performance using metrics such as accuracy, loss, precision, recall, and F1-score.

## Results
The models demonstrated robust performance in classifying defective and non-defective casting products, significantly improving over manual inspection accuracy.


