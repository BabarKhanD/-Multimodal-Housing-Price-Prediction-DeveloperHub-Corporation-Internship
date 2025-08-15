# Multimodal Housing Price Prediction — DeveloperHub Corporation Internship

## Objective
This project, developed as part of my internship with **DeveloperHub Corporation**, aims to predict housing prices by leveraging both **tabular data** (e.g., bedrooms, bathrooms, area, zipcode) and **real images** of houses.

The goal is to demonstrate **multimodal machine learning** by combining features extracted from house images via CNN with structured data for accurate regression modeling.

## Dataset
- **Source:** [Houses Dataset (Ahmed & Moustafa, 2016)](https://github.com/emanhamed/Houses-dataset)
- **Contents:**
  - 535 houses
  - 4 images per house (bedroom, bathroom, kitchen, front view)
  - Metadata: bedrooms, bathrooms, area, zipcode, price

## Methodology / Approach
1. **Data Loading & Cleaning**  
   - Load tabular metadata.
   - Load and preprocess images into 2×2 montages.
2. **Feature Engineering**  
   - **Image branch:** MobileNetV2 pretrained CNN → GlobalAveragePooling → feature vector.
   - **Tabular branch:** Numeric scaling + categorical one-hot encoding.
3. **Feature Fusion**  
   - Concatenate image and tabular features.
4. **Model Training**  
   - Fully connected regression head with dropout regularization.
5. **Evaluation**  
   - Metrics: MAE, RMSE.
   - Actual vs Predicted price plots.

## Skills Demonstrated
- Multimodal Machine Learning
- Convolutional Neural Networks
- Feature Fusion
- Regression Modeling
- Data Visualization

## Acknowledgements
Special thanks to **DeveloperHub Corporation** for providing this internship opportunity and guidance, and to the mentors and team members who supported the project.
Dataset courtesy of Ahmed & Moustafa (2016).
