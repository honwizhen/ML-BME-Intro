# Classifying Biological Sex Using FreeSurfer Volumetric Features

This Jupyter Notebook demonstrates how to classify biological sex (male/female) using volumetric features extracted from FreeSurfer, a widely used tool for analyzing brain MRI data. The notebook employs a Random Forest classifier with hyperparameter tuning via Grid Search to achieve the classification task.

## Overview

The notebook covers the following steps:
1. **Data Loading and Preprocessing**: Load the dataset, clean column names, and encode the target variable (sex) as binary values (0 for female, 1 for male).
2. **Exploratory Data Analysis (EDA)**: Visualize the distribution of sex and age in the dataset.
3. **Feature Scaling**: Standardize the features using `StandardScaler`.
4. **Model Training**: Use a Random Forest classifier with Grid Search for hyperparameter tuning.
5. **Model Evaluation**: Evaluate the model using accuracy and a confusion matrix.

## Prerequisites

To run this notebook, you need the following:
- Python 3.x
- Jupyter Notebook or JupyterLab
- Required Python libraries:
  - `numpy`
  - `pandas`
  - `seaborn`
  - `matplotlib`
  - `scikit-learn`

You can install the required libraries using `pip`:

```bash
pip install numpy pandas seaborn matplotlib scikit-learn
```

## Dataset

The dataset used in this notebook is stored in an Excel file (`volumetry_cc359.xlsx`). It contains volumetric features extracted from brain MRI scans using FreeSurfer. The dataset includes features such as:

- Left and right hemisphere volumes (e.g., `Left_Lateral_Ventricle`, `Right_Lateral_Ventricle`).
- Subcortical gray matter volumes (e.g., `Left_Hippocampus`, `Right_Hippocampus`).
- Total gray matter and white matter volumes.
- Demographic information (e.g., age, sex).

## Notebook Structure

### 1. Data Loading and Preprocessing
- Load the dataset and clean column names.
- Encode the target variable (Sex) as binary values (0 for female, 1 for male).

### 2. Exploratory Data Analysis (EDA)
- Visualize the distribution of sex and age in the dataset.

### 3. Feature Scaling
- Standardize the features using `StandardScaler`.

### 4. Model Training
- Use a Random Forest classifier with Grid Search for hyperparameter tuning.
- The hyperparameters tuned include:
  - `bootstrap`
  - `max_depth`
  - `max_features`
  - `min_samples_leaf`
  - `min_samples_split`
  - `n_estimators`

### 5. Model Evaluation
- Evaluate the model using accuracy and a confusion matrix.

## Results

The model achieves an accuracy of approximately **76.33%** on the test set. The confusion matrix provides insights into the classification performance for male and female classes.

## Usage

Clone this repository (if applicable):

```bash
git clone https://github.com/your-repo/your-project.git
```

Navigate to the repository:

```bash
cd your-project
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook and run the cells to perform the classification task.

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to open an issue or submit a pull request.

## License

This project is not licensed

## Author

Honwi Zhen
GitHub: [honwizhen](https://github.com/honwizhen)
LinkedIn: (https://www.linkedin.com/in/honwi-zhen-feng/)

---
Feel free to explore the notebook and adapt it to your own projects! If you have any questions, please reach out.

### Notes:
- Replace `your-repo`, `your-project`, and `your-username` with the appropriate details.
- If the notebook is part of a larger repository, update the repository link and description accordingly.
- Add a `LICENSE` file if one doesn’t already exist in your repository.
