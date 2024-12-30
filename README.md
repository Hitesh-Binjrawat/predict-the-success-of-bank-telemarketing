# MLP Project: Direct Marketing Campaign Prediction

## Project Description
This project analyzes data from direct marketing campaigns conducted by a banking institution. The campaigns were based on phone calls, with multiple contacts to the same client often required to assess whether the product (a bank term deposit) would be subscribed (`'yes'`) or not (`'no'`).

The goal of this project is to build a predictive model using a GradientBoostingClassifier,DecisionTrees, AdaBoost to classify whether a client will subscribe to the product.

---

## Dataset Overview
The dataset contains the following information:
- **Features:** Various attributes related to the client and campaign, such as demographics, past campaign outcomes, and current campaign characteristics.
- **Target Variable:** Binary label (`'yes'` or `'no'`) indicating if the client subscribed to the product.

---

## Evaluation
The submissions are evaluated using the **F1 Score** with `average='macro'` between the predicted classes and the true target values.

### Why F1 Score (Macro)?
- The F1 Score (Macro) is used because it equally weights the performance of both classes (`'yes'` and `'no'`), ensuring balanced evaluation regardless of class imbalance.

---

## Submission Format
Participants are required to submit their predictions in the following format:
- A CSV file containing predictions for the test set.
- Columns:
  1. **ID:** Unique identifier for each sample in the test set.
  2. **Target:** Predicted class (`'yes'` or `'no'`).

### Example:
| ID  | Target |
|-----|--------|
| 1   | yes    |
| 2   | no     |
| 3   | yes    |

---

## Project Workflow
1. **Data Preprocessing:**
   - Handling missing values, outliers, and data scaling.
   - Encoding categorical variables.

2. **Model Training:**
   - Developing a Multi-Layer Perceptron (MLP) model.
   - Performing hyperparameter tuning for optimal performance.

3. **Evaluation:**
   - Validating the model on a holdout dataset.
   - Computing the F1 Score (Macro) to assess performance.

4. **Submission:**
   - Generating predictions for the test set.
   - Formatting and submitting the prediction file.

---

## Technologies Used
- **Programming Language:** Python
- **Libraries:**
  - Scikit-learn
  - NumPy
  - Pandas
- **Tools:**
  - Jupyter Notebook
  - Visualization libraries (e.g., Matplotlib, Seaborn)

---
