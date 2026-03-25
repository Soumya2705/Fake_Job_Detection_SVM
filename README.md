# 🚀 Fake Job Detection using SVM

## 📌 Project Overview

This project focuses on detecting fraudulent job postings using Support Vector Machine (SVM) and Natural Language Processing (NLP) techniques.

With the increasing number of online job scams, this project aims to classify job listings as **real or fake** based on textual and categorical features.

The project demonstrates a complete machine learning workflow including **data preprocessing, feature engineering, handling imbalanced data, model training, and evaluation**.

---

## 📂 Dataset

The dataset used is the **Fake Job Postings Dataset from Kaggle**, which contains job descriptions, company details, and labels indicating whether a job is fraudulent.

---

## 🛠️ Tools & Libraries Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* SciPy
* Jupyter Notebook

---

## 🧹 Data Preprocessing

* Handled missing values
* Combined multiple text columns (title, description, requirements)
* Removed unnecessary columns
* Encoded categorical variables
* Prepared dataset for machine learning models

---

## 🔤 Feature Engineering

* Applied **TF-IDF Vectorization** to convert text into numerical features
* Used **n-grams (unigram + bigram)** to capture meaningful phrases
* Combined text features with categorical features

---

## ⚖️ Handling Imbalanced Data

The dataset was highly imbalanced (very few fraudulent jobs compared to real jobs).

Techniques used:

* Class Weighting (`class_weight='balanced'`)
* Undersampling (reducing majority class)

Different approaches were compared to understand their impact on model performance.

---

## 📈 Models Implemented

### 1️⃣ SVM (Baseline)

* Linear Support Vector Machine applied on TF-IDF features

### 2️⃣ SVM with Class Weight

* Handled class imbalance without losing data
* Improved recall for fraudulent jobs

### 3️⃣ Undersampled SVM

* Balanced dataset by reducing majority class
* Achieved highest recall for fraud detection

---

## 🔍 Model Evaluation

Models were evaluated using:

* Precision
* Recall
* F1-score
* Accuracy

Special focus was given to **recall for fraudulent jobs**, since missing fraud cases is critical.

---

## 🏆 Results Summary

* Highest Recall: ~90% (Undersampling)
* Best Practical Model: Class-weighted SVM
* Demonstrated trade-off between **accuracy and recall**

---

## 🚀 How to Run

1. Clone the repository
2. Download dataset (if not included)
3. Open the notebook (`svm_fake_job_detection.ipynb`)
4. Run all cells step-by-step

---

## 🔮 Future Scope

* Deploy model using Streamlit
* Try advanced models (XGBoost, Deep Learning)
* Improve feature engineering with embeddings (Word2Vec, BERT)
* Build real-time job fraud detection system

---

## 📌 Conclusion

This project highlights how SVM can be effectively used for text classification problems and demonstrates practical techniques to handle imbalanced datasets in real-world scenarios.

---

## 📌 License

This project is created for educational and learning purposes.
