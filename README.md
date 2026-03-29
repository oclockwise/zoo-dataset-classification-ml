# Zoo Dataset ML Classification

## Overview
This project explores how different machine learning models can classify animals based on their physical and behavioural features using the Zoo dataset. The goal is to predict the correct animal category (e.g. mammal, bird, fish) from input features.

## Dataset
- 101 animals with 16 features  
- Features include: hair, feathers, eggs, milk, legs, etc.  
- Target variable: `class_type` (7 animal categories)

## Models Used
- k-Nearest Neighbors (k-NN)
- Naive Bayes
- Decision Tree  

Both custom implementations and scikit-learn models were used for comparison.

## Key Steps
- Removed non-predictive features (e.g. animal names)  
- Feature scaling using StandardScaler  
- Train-test split (70/30)  
- Stratified cross-validation (4-fold)  
- Hyperparameter tuning (Decision Tree)

## Results
- k-NN and Decision Tree achieved ~90% accuracy  
- Naive Bayes showed stable and consistent performance  
- Feature importance analysis showed key predictors like **milk, feathers, and fins**

## Insights
- Feature scaling improves performance for distance-based models  
- Model complexity affects overfitting and generalization  
- Some animal classes are harder to distinguish due to similar features  

## Tech Stack
- Python  
- pandas, numpy  
- scikit-learn  
- matplotlib  

## Run
```bash
pip install pandas numpy scikit-learn matplotlib
jupyter notebook
