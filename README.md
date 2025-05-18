# Depression Risk Predictor

This repository contains the code and resources for the **Depression Risk Predictor** project. The main analysis and machine learning workflow are implemented in the `projet.ipynb` notebook.

## Project Overview

Depression is a significant public health concern worldwide. This project leverages machine learning to predict the risk of depression based on individual data. The primary workflow, including data preparation, modeling, and experiment tracking, is provided in `projet.ipynb`.

## Notebook: projet.ipynb — Step-by-step Guide

1. **Import Libraries**
   - Load all necessary Python libraries (e.g., pandas, numpy, matplotlib, seaborn, scikit-learn).
   - Import and initialize [Weights & Biases (wandb)](https://wandb.ai/) for experiment tracking and pipeline management.

2. **Load the Dataset**
   - Load the data file (CSV or similar) into a pandas DataFrame.
   - Display the first few rows to understand the structure and variables.

3. **Data Cleaning**
   - Check for and handle missing values (e.g., drop, fill, or impute).
   - Convert categorical variables to numerical (using encoding if needed).
   - Rename columns for clarity if necessary.

4. **Exploratory Data Analysis (EDA)**
   - Visualize distributions of key features (histograms, boxplots, etc.).
   - Use correlation matrices or pairplots to examine relationships.
   - Summarize key statistics about the dataset (mean, std, counts).

5. **Feature Engineering**
   - Select relevant features for prediction.
   - Create new composite features if useful.
   - Scale or normalize features if appropriate.

6. **Data Splitting**
   - Divide the data into training and test sets (e.g., 70% train, 30% test).
   - Ensure reproducibility using a fixed random state.

7. **Model Pipeline with wandb Integration**
   - Define and build a machine learning pipeline for the task.
   - Use wandb to:
     - Track experiments and metrics.
     - Log hyperparameters, artifacts, and model outputs.
     - Visualize and compare model performances directly on the wandb dashboard.
   - Train, validate, and optimize different models (e.g., Logistic Regression, Random Forest, etc.) using the pipeline.

8. **Model Evaluation**
   - Make predictions on the test set.
   - Evaluate performance: accuracy, precision, recall, F1-score, ROC-AUC.
   - Display confusion matrices and ROC curves for the best model.
   - Log evaluation results to wandb for easy tracking and visualization.

9. **Model Interpretation**
   - Identify and visualize the most important features.
   - Discuss what these features might mean in the context of depression risk.

10. **Conclusions and Insights**
    - Summarize the main findings.
    - List the best-performing model and its metrics.
    - Discuss any limitations or considerations for real-world use.

11. **Next Steps / Recommendations**
    - Suggest further work, such as collecting more data, trying advanced models, or deploying the model.

---

## How to Use

1. **Clone the Repository**
   ```bash
   git clone https://github.com/andrebrandaopro/DepressionRiskPredictor.git
   cd DepressionRiskPredictor
   ```

2. **Create and Activate the Conda Environment**
   ```bash
   conda env create -f environment.yml
   conda activate depression-risk-predictor
   ```

3. **Set Up wandb**
   - Sign up at [wandb.ai](https://wandb.ai/) if you don’t have an account.
   - Run `wandb login` and paste your API key as instructed.

4. **Run the Notebook**
   - Start Jupyter Notebook:
     ```bash
     jupyter notebook
     ```
   - Open `projet.ipynb` and follow the steps from top to bottom, executing each cell in order.

## Dataset

- Place your dataset in the location specified in the notebook or update the notebook path as needed.
- If the dataset is not included, refer to the instructions in the notebook for how to obtain or simulate the data.

---

**Author:**  
[andrebrandaopro](https://github.com/andrebrandaopro)
