# Medical Insurance Cost Prediction using Regression Models

This repository contains multiple Jupyter Notebooks that implement and compare various regression models to predict medical insurance costs based on user features such as age, BMI, number of children, smoking habits, and region.

## 📊 Dataset

We use the **U.S. Health Insurance Dataset** from Kaggle:  
🔗 [Kaggle Dataset Link](https://www.kaggle.com/datasets/teertha/ushealthinsurancedataset)

## 📁 Notebooks Included

Each notebook implements one regression model:

- `insurance_multiple_regression.ipynb`: Multiple Linear Regression
- `insurance_polynomial_regression.ipynb`: Polynomial Regression
- `insurance_decision_tree_regression.ipynb`: Decision Tree Regression
- `insurance_random_forest_regression.ipynb`: Random Forest Regression
- `insurance_svr.ipynb`: Support Vector Regression (SVR)

## 📈 Visualizations

All notebooks include:
- Predicted vs Actual cost plots
- Residual plots (where applicable)
- Evaluation metrics such as MAE, MSE, RMSE, and R²

These visualizations help compare model performance and understand how well each model fits the data.

## ⚠️ Important: Setup Instructions for Running the Notebooks

In order to download the dataset directly from Kaggle and run these notebooks:

1. **Get your Kaggle API key**:
   - Go to your Kaggle account settings.
   - Click on “Create New API Token”.
   - A file named `kaggle.json` will be downloaded.

2. **Upload the API key in Colab (or locally)**:
   Uncomment and run the following code block in a new cell **at the beginning** of each notebook if you're using Google Colab:

   ```python
   from google.colab import files
   files.upload()  # Upload kaggle.json file here

   !mkdir ~/.kaggle
   !cp kaggle.json ~/.kaggle/
   !chmod 600 ~/.kaggle/kaggle.json
   ```

3. **Download the dataset with:**
   ```python
   !kaggle datasets download -d teertha/ushealthinsurancedataset
   !unzip ushealthinsurancedataset.zip
   ```

## 🧠 Objective

The aim is to understand which regression model performs best for predicting medical insurance costs and to explore how model complexity and interpretability vary across methods.

---

### 📌 Notes

- Sensitive API keys have been **removed** from the notebooks for security.
- Graphs are kept intact to visually compare model performance.
- Make sure to upload your own `kaggle.json` for the notebooks to work.

---

## 💡 Author

Mathiyazhagan A — 2025  
This project is part of a regression model comparison study.
