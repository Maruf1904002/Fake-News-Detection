# 📰 Fake News Detection using Machine Learning

This repository contains a **Fake News Classifier** built with machine learning techniques.  
The project uses the [Fake and Real News Dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset) from Kaggle to classify news articles as **REAL** or **FAKE**.

---

## 📊 Dataset
- **Source:** Kaggle — Fake and Real News Dataset  
- **Files:**
  - `Fake.csv` → 23,481 fake news articles  
  - `True.csv` → 21,417 real news articles  
- **Features used:** `title + text` (concatenated)  
- **Labels:**
  - `0` = FAKE news  
  - `1` = REAL news  

---

## 🛠️ Project Workflow
1. **Data Preprocessing**
   - Loaded and merged Fake & True datasets  
   - Created a `content` column (`title + text`)  
   - Handled missing values and shuffled the data  

2. **Data Splitting**
   - Train: 80% (~36k articles)  
   - Validation: 10% (~4.5k articles)  
   - Test: 10% (~4.5k articles)  

3. **Model**
   - `TF-IDF Vectorizer` → Convert text to numerical features  
   - `LinearSVC (Support Vector Machine)` → Classification  

4. **Evaluation Metrics**
   - Accuracy  
   - Precision, Recall, F1-score  
   - Confusion Matrix  

---

## 🚀 Results

- **Validation Accuracy:** ~99.4%  
- **Test Accuracy:** ~99.7%  

| Metric       | Fake (0) | Real (1) |
|--------------|----------|----------|
| Precision    | 0.997    | 0.997    |
| Recall       | 0.997    | 0.997    |
| F1-score     | 0.997    | 0.997    |

- **Confusion Matrix (Test Set):**

See Confusion Matrix png file

---

