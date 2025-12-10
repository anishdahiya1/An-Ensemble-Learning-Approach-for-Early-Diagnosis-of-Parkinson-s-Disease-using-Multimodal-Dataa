# An-Ensemble-Learning-Approach-for-Early-Diagnosis-of-Parkinson-s-Disease-using-Multimodal-Dataa

Parkinson’s Disease Prediction Using Machine Learning

I built a predictive machine learning model to identify early signs of Parkinson’s Disease using biomedical voice measurements. This project focuses on applying statistical feature analysis and supervised learning algorithms to classify whether a patient is likely to have Parkinson’s based on measurable vocal biomarkers.

🔍 Problem Background

Parkinson’s Disease affects motor function, and one of the earliest detectable symptoms appears in speech — specifically, changes in vocal frequency, jitter, shimmer, and amplitude.
The goal was to leverage these measurable acoustic biomarkers to build a model that could support early screening and assist medical evaluation.

🧠 Approach & Technical Workflow
1️⃣ Dataset & Features

The dataset contains biomedical voice measurements collected from both healthy individuals and Parkinson’s patients.
Key features include:

MDVP:Fo(Hz) — Average vocal fundamental frequency

Jitter, Jitter(%) — Variations in frequency

Shimmer, Shimmer(dB) — Variations in amplitude

NHR & HNR — Noise-to-harmonics ratios

RPDE, DFA — Nonlinear signal complexity measures

PPE — Fundamental frequency variation

These features are strong indicators of vocal impairment associated with Parkinson’s.

2️⃣ Data Preprocessing

I applied a structured preprocessing pipeline:

Handling missing data

Standardization of all numerical features

Correlation analysis and feature importance mapping

Splitting data into training & testing sets

This ensured stable model performance and reduced noise in predictions.

3️⃣ Model Training & Evaluation

I trained multiple ML models to compare performance:

Model	Accuracy	Remarks
Logistic Regression	~86–90%	Strong baseline, interpretable
SVM (RBF)	High	Robust for non-linear feature spaces
Random Forest	Good	Handles feature interactions well
KNN	Lower	Performance sensitive to scaling

The best-performing model in your implementation was:
🔹 Logistic Regression (≈ 86% accuracy)
It provided a good balance between interpretability and predictive power, making it suitable for medical decision support systems.

Evaluation included:

Confusion Matrix

Precision, Recall, F1-score

ROC-AUC analysis

📊 Insights Derived

Frequency-based features and jitter/shimmer variations were strong predictors.

Noise-to-harmonics ratio (NHR) had high influence on classification.

Linear models performed better due to the structured nature of biomedical voice features.
