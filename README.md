🧠 Customer Purchase Prediction (Random Forest)

This project builds a machine learning classification model to predict whether a customer will purchase a travel product based on demographic, behavioral, and interaction-related features.

The solution uses a Random Forest classifier and evaluates performance using multiple classification metrics.

📌 Problem Statement

Predict whether a customer will take a product offer (ProdTaken) using historical customer data collected during sales pitches.

This is formulated as a binary classification problem:

1 → Product taken

0 → Product not taken

📊 Dataset Description

Total records: 4,888

Total features: 20

Target variable: ProdTaken

The dataset includes:

Customer demographics (age, gender, income, marital status)

Interaction details (pitch duration, satisfaction score, follow-ups)

Travel preferences (number of trips, property star rating)

Socio-economic indicators (city tier, occupation, designation)

Missing values were handled during preprocessing before model training.

🛠️ Model Used

Algorithm: Random Forest Classifier

Framework: scikit-learn

Key Parameters:

n_estimators = 1000

max_features = 7

min_samples_split = 2

max_depth = None

Random Forest was chosen for its robustness, ability to handle mixed feature types, and resistance to overfitting.

📈 Model Performance (Test Set)
Metric	Score
Accuracy	93.15%
F1 Score	92.65%
Precision	96.97%
Recall	67.02%
ROC-AUC	83.25%
🔍 Interpretation

High precision indicates the model rarely predicts a purchase incorrectly.

Lower recall suggests some actual buyers are missed, which is acceptable in scenarios where false positives are costly.

ROC-AUC shows good overall class separability.

⚙️ Workflow

Data cleaning and preprocessing

Handling missing values

Feature encoding and splitting (train/test)

Model training using Random Forest

Evaluation using accuracy, precision, recall, F1, and ROC-AUC
