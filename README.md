# Credit Card Fraud Detection

This repository contains a machine learning project aimed at detecting fraudulent transactions in credit card data. The project follows a structured approach to understand the problem, prepare the data, and evaluate models.

## 1. Problem Understanding

**Task**: To classify credit card transactions as fraudulent or legitimate using machine learning models.

**Input**: A dataset of credit card transactions, including anonymized numerical features and transaction details.

**Output**: A binary classification indicating whether a transaction is fraudulent (1) or not (0).

**Type of Problem**: Binary Classification.

**Features**: Anonymized features labeled V1, V2, ..., V28, and additional attributes such as `Time` and `Amount`.

**Evaluation Metric**:
- Precision
- Recall
- F1-score
- Accuracy

## 2. Dataset

**Source**: [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

**Dataset Details**:
- Number of instances: 284,807
- Number of features: 30 (including `Class` for labels)
- Highly imbalanced dataset with ~0.17% fraudulent transactions.

## 3. Data Exploration

- **Input Structure**: Numerical features (V1 to V28), `Time`, and `Amount`.
- **Output Structure**: Binary labels indicating fraud or legitimate transactions.
- **Observations**:
  - Features are anonymized and scaled.
  - High class imbalance necessitates specific evaluation metrics (e.g., precision and recall).

## 4. Data Preparation

1. **Train-Test Split**: The dataset is split into training and testing sets.
2. **Handling Missing Values**: No missing values identified.
3. **Feature Scaling**: Applied to numerical features (`Amount` and `Time`).
4. **Imbalanced Data Handling**: Techniques like SMOTE or class weighting were explored.
5. **Pipeline**: Automated data preprocessing pipeline for consistency.

## 5. Model Selection, Training, and Evaluation

### Models Used
- **Baseline Model**: Logistic Regression
- **Advanced Model**: Neural Network with layers designed for binary classification.

### Training and Evaluation
- Models trained on the prepared training dataset.
- Performance evaluated on the test set using precision, recall, and F1-score.

### Results
- **Baseline Performance**: [Insert performance metrics]
- **Neural Network Performance**: [Insert performance metrics]
- Analysis: The neural network outperformed the baseline in [specific metrics].

## 6. Future Work

Based on the current results, future steps may include:
- Hyperparameter tuning of the neural network.
- Experimentation with ensemble models like Random Forest or Gradient Boosting.
- Feature engineering to derive more informative attributes.
- Further investigation into imbalanced data handling techniques.

## How to Run the Code

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook to reproduce results.

## Dataset License
The dataset is provided under the Database Contents License (DbCL 1.0). Please ensure compliance when using this dataset.

---

For any questions or suggestions, please feel free to open an issue or reach out!


