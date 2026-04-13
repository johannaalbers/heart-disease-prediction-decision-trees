# Heart Disease Prediction using Decision Trees

This project applies machine learning techniques to predict the presence of cardiovascular disease (CVD) using clinical patient data. The focus is on **decision trees**, a highly interpretable model often used in healthcare and precision medicine.

---

## Dataset

The dataset contains information from 918 patients and includes 11 clinical features such as:

- Age
- Sex
- Chest pain type
- Blood pressure
- Cholesterol levels
- Maximum heart rate
- Exercise-induced angina

Target variable:
- `HeartDisease` (1 = disease, 0 = healthy)

Source: Kaggle Heart Failure Prediction Dataset  
:contentReference[oaicite:0]{index=0}

---

## Project Pipeline

### 1. Data Preparation
- Train-test split (80/20)
- Handling categorical variables:
  - One-hot encoding (Sex)
  - Ordinal encoding (other categorical features)
- Feature scaling (MinMaxScaler)

### 2. Model
- Decision Tree Classifier
- Criterion: Entropy
- Max depth: 2

### 3. Evaluation
- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix
- ROC analysis

### 4. Interpretability
- Tree visualization (Graphviz)
- Feature importance analysis

---

## Results

- Accuracy: ~85%  
- Model successfully identifies patients at risk of heart disease  
- Most important features include:
  - ST_Slope
  - ChestPainType

---

## Key Learnings

- Decision trees are powerful and interpretable models for clinical data
- Proper preprocessing (encoding + scaling) is critical
- Feature importance helps understand medical relevance

---

## Tech Stack

- Python
- pandas
- scikit-learn
- matplotlib / seaborn
- graphviz
