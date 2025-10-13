# Predicting Student Success Using Supervised Machine Learning

**Evidence from the Open University Learning Analytics Dataset**


## Website
https://anianlotte919.github.io/ou-student-outcome-prediction/ 

## Project Overview

This project uses machine learning to predict student outcomes (Pass, Fail, Withdrawn, Distinction) in online courses using the Open University Learning Analytics Dataset (OULAD). The analysis combines demographic information, course enrollment data, VLE engagement metrics, and assessment performance to build predictive models that can support early intervention systems.

## Author

**Yun Xia**
Email: yuxi8959@colorado.edu
Course: Introduction to Machine Learning: Supervised Learning
Date: October 2025

## Key Results

- **Best Model**: Random Forest Classifier
- **Performance**: 67.42% accuracy, 0.6614 weighted F1, 0.8836 ROC-AUC
- **Strong Predictions**: 86% recall for Pass, 71% recall for Withdrawn
- **Challenge Areas**: 38% recall for Fail (30% misclassified as Pass)

## Dataset

**Open University Learning Analytics Dataset (OULAD)**
- Source: Kaggle mirror of official OULAD release
- Link: https://www.kaggle.com/datasets/anlgrbz/student-demographics-online-education-dataoulad
- Citation: Kuzilek, J., Hlosta, M., & Zdrahal, Z. (2017). Open university learning analytics dataset. Scientific data, 4(1), 1-8.
- DOI: https://doi.org/10.1038/sdata.2017.171

## Requirements

- Python 3.11+
- scikit-learn ≥ 1.3
- pandas
- numpy
- matplotlib

## Usage

1. Download the OULAD dataset and place it in `./dataset/` directory
2. Run the analysis

## Models Compared

- Logistic Regression (baseline)
- K-Nearest Neighbors (KNN)
- AdaBoost
- Random Forest (best performer)
- Support Vector Machine (SVM) - optional

## Key Features

**Behavioral metrics:**
- VLE engagement (sum_click)
- Assessment scores (weighted average)

**Demographic variables:**
- Age band, gender, disability status
- Socioeconomic status (IMD band)
- Education level, region

**Course information:**
- Module code, presentation semester
- Registration timing, credits studied
- Previous attempts

## Contact

For questions or collaboration:
- Email: yuxi8959@colorado.edu

