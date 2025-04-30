# GDSC_PROJECT
Price Prediction using Machine Learning 🧠
Welcome to the House Price Prediction project! This project uses various machine learning algorithms to predict house prices based on a set of features.

📚 Table of Contents
Introduction
Dataset
Usage
Models Used
Evaluation
Contributing
License

🌟 Introduction
Estimating a home’s market value can be tricky. In this project, we build machine-learning models—trained on a wide range of property features—to deliver reliable house-price predictions.

📊 Dataset
The dataset contains 13 features including:

Id: Record identifier.
MSSubClass: Type of dwelling.
MSZoning: General zoning classification.
LotArea: Lot size in square feet.
LotConfig: Configuration of the lot.
BldgType: Type of dwelling.
OverallCond: Overall condition of the house.
YearBuilt: Original construction year.
YearRemodAdd: Remodel date.
Exterior1st: Exterior covering on house.
BsmtFinSF2: Type 2 finished square feet.
TotalBsmtSF: Total square feet of basement area.
SalePrice: Sale price of the house (target variable).
Dataset Overview

Usage/Procedure
1. Open the Colab Notebook

2. Go to Google Colab and upload or link the provided .ipynb.

3. Install Dependencies & Mount Drive

python
Copy
Edit
!pip install pandas openpyxl tensorflow scikit-learn pyyaml
from google.colab import drive
drive.mount('/content/drive')
4.Load & Preprocess Data
Update the path to your Excel file (either in your Drive or uploaded manually).

5. Run the “Data Loading & Cleaning” cell to drop irrelevant columns, impute missing values, and one-hot encode categoricals.
6. Configure & Build the Model
In the “Model Definition” cell, tweak layer sizes, activation functions, dropout rates, and learning rate.

7. Train
Execute the “Training” cell. Adjust epochs and batch_size to suit your GPU/CPU quota.
 
8. Evaluate & Visualize
Run the “Evaluation” cell to compute MAPE, RMSE, and R².
View training curves in the “Plot History” cell.
 Save Outputs

9. After training, save your model checkpoints and a CSV of predictions back to Drive for future use.
