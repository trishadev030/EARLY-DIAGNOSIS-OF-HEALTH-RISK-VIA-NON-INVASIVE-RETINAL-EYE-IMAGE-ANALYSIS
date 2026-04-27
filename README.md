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
- Scikit-learn  
- Matplotlib  
- Streamlit  
- Jupyter Notebook  

## Screenshots
<img width="688" height="259" alt="Screenshot 2026-04-27 120833" src="https://github.com/user-attachments/assets/d4891813-c876-4cf7-8bf9-20417015e998" />

<img width="1365" height="732" alt="Screenshot 2026-02-23 131851" src="https://github.com/user-attachments/assets/8b26ad32-8d1d-4321-b274-e85c5f65b538" />

<img width="1365" height="545" alt="Screenshot 2026-02-23 131900" src="https://github.com/user-attachments/assets/61e623c8-0c6d-488c-9eb3-00ba3a26cc82" />


## Project Status

This project requires GPU for training and is not fully runnable in the current environment as it needs access to GPU enabled systems.

## Observations

Although the model achieves high accuracy (~96.88%), predictions are probabilistic in nature. 

In some cases, the model may assign small probabilities to multiple classes (e.g., slight probability for "normal" along with a disease class). This occurs due to similarities in retinal features across conditions and inherent uncertainty in medical image classification.

Such behavior reflects realistic model confidence distribution rather than a definitive error.

## Future Work

- Use larger datasets
- Improve model accuracy
- Deploy as mobile/web app
- Integrate clinical decision support systems

*The model outputs probability scores for all classes, enabling better interpretability and supporting clinical decision-making rather than providing rigid classifications.*
