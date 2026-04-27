# Early Diagnosis of Health Risk via Retinal Image Analysis

This project focuses on early detection of health risks using non-invasive retinal fundus image analysis with deep learning techniques.

## Overview

The retina provides critical information about vascular and structural changes associated with diseases such as:
- Diabetic Retinopathy
- Hypertension
- Glaucoma
- Cataract
- Age-related Macular Degeneration
- Pathological Myopia

This system uses deep learning to automate disease detection from retinal images.

## Methodology

1. Data preprocessing (resizing, normalization, augmentation)
2. Model training using transfer learning
3. Multi-model comparison
4. Disease classification
5. Explainability using Grad-CAM
6. Deployment using Streamlit

## Models Used

- ResNet101
- ResNet152
- DenseNet201
- InceptionResNetV2
- ConvNeXt
- Xception

## Results

Xception achieved the highest accuracy (~96.88%).

## Features

- Multi-class disease classification
- Non-invasive screening
- Grad-CAM visualization for explainability
- Streamlit-based interface for real-time prediction

## Dataset

Dataset sourced from Kaggle (approx. 50,000 retinal images).

Dataset is not included due to size and privacy.

## Tech Stack

- Python
- TensorFlow / PyTorch
- NumPy, Pandas
- Streamlit

## Project Status

This project requires GPU for training and is not fully runnable in the current environment.

## Future Work

- Use larger datasets
- Improve model accuracy
- Deploy as mobile/web app
- Integrate clinical decision support systems
