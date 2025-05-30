# User Purchase Prediction using SVM

This project implements a Support Vector Machine (SVM) algorithm to predict whether a user will purchase a product based on their age and estimated salary. The dataset contains user demographic information and purchase behavior, and the goal is to build a classifier that can accurately predict purchase intent.

## Table of Contents

- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Building](#model-building)
- [Evaluation](#evaluation)
- [Results](#results)
- [Visualizations](#visualizations)
- [Dependencies](#dependencies)
- [How to Run](#how-to-run)
- [License](#license)

---

## Dataset

The dataset used is [`data/userdata.csv`](data/userdata.csv), which contains the following columns:

- **User ID**: Unique identifier for each user
- **Gender**: Gender of the user
- **Age**: Age of the user
- **EstimatedSalary**: Estimated salary of the user
- **Purchased**: Target variable (0 = Not Purchased, 1 = Purchased)

## Project Workflow

1. **Data Import & Cleaning**
   - Load the dataset using pandas.
   - Check for missing and duplicate values.

2. **Feature Selection & Scaling**
   - Select `Age` and `EstimatedSalary` as features.
   - Scale features using `StandardScaler`.

3. **Exploratory Data Analysis**
   - Visualize distributions and relationships in the data.

4. **Model Training**
   - Split data into training and test sets.
   - Train two SVM models: one with a linear kernel and one with an RBF (non-linear) kernel.

5. **Evaluation**
   - Predict on the test set.
   - Evaluate using accuracy, F1 score, recall, precision, and confusion matrix.

6. **Visualization**
   - Plot decision boundaries and confusion matrices.

## Exploratory Data Analysis

- Distribution plots for Age and Estimated Salary.
- Count plot for purchase distribution.
- Scatter plot of Age vs. Estimated Salary colored by purchase status.

## Model Building

- **Linear SVM**: Uses a linear kernel to find a straight-line decision boundary.
- **Non-linear SVM**: Uses an RBF kernel to capture more complex relationships.

## Evaluation

- **Accuracy**
- **F1 Score**
- **Recall**
- **Precision**
- **Confusion Matrix**

## Results

- The non-linear SVM (RBF kernel) outperformed the linear SVM on this dataset.
- Example metrics (may vary depending on random state and data split):

## For Linear SVM Model: 
- Accuracy : 0.90 
- Fl Score : 0.83 
- Recall : 0.75 
- Precision: 0.92
## For Non Linear SVM Model: 
- Accuracy : 0.93 
- Fl Score : 0.89 
- Recall : 0.91 
- Precision: 0.88


## Visualizations

- Decision boundary plots for both linear and non-linear SVMs.
- Confusion matrices for both models.
- Distribution and scatter plots for data exploration.

## Dependencies

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
- mlxtend

Install all dependencies using:

```sh
pip install numpy pandas matplotlib seaborn scikit-learn mlxtend
```
## License
- This project is licensed under the MIT License.
