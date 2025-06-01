# Glaucoma Detection Using Fundus Images

## Overview
An AI-driven image processing pipeline developed for early-stage glaucoma detection from retinal fundus images. The system identifies the optic disc and cup regions, calculates the Cup-to-Disc Ratio (CDR), and flags potential glaucoma-positive cases.

## Key Techniques
- 📷 Fundus Image Preprocessing (grayscale, binarization, Otsu thresholding)
- 🔍 Optic Disc and Cup segmentation using morphological and edge detection techniques
- 📈 Cup-to-Disc Ratio (CDR) calculation for glaucoma risk classification
- 🤖 ResNet-50-based classification model for automated detection

## Pipeline
1. Load fundus image from dataset
2. Convert to grayscale and apply morphological preprocessing
3. Segment optic disc and cup using fuzzy edge logic
4. Calculate CDR and compare to threshold
5. If CDR > threshold → flag as suspected glaucoma

## Tools & Libraries
- OpenCV, NumPy, Matplotlib
- TensorFlow / Keras for ResNet model
- Custom Python scripts for pre-processing and segmentation

## Dataset
- Kaggle Glaucoma Detection Dataset
- Preprocessed using Otsu binarization and image resizing

## Output
- Binary classification: Glaucoma / Normal
- Visual overlays for optic disc/cup segmentation
- ROC curve and AUC for model performance evaluation

## Applications
Early glaucoma detection aids ophthalmologists in diagnosis and helps reduce vision loss by timely intervention.
