# 🧠 Early Brain Stroke Detection using Pathological Voice Features and Machine Learning

## 📌 Overview
This project focuses on detecting early signs of neurological disorders (such as stroke) using speech analysis. Subtle changes in voice occur before visible symptoms due to impaired motor control of speech-related muscles.

The system extracts acoustic features from voice recordings and uses machine learning models to classify speech as healthy or pathological.

---

## 🎯 Problem Statement
Traditional neurological diagnosis often happens after noticeable symptoms appear. However, early-stage disorders affect speech production due to disrupted neural control of vocal mechanisms.

The goal of this project is to build a non-invasive and accessible early screening system using voice as a biomarker.

---

## 💡 Key Idea / Innovation
- Uses speech as a biomarker for neurological health  
- Detects subtle voice changes before clinical symptoms  
- Combines acoustic signal processing and machine learning  
- Uses explainable AI (SHAP) for model interpretation  

---

## 📂 Dataset
- Source: TORGO Dataset (Dysarthric Speech)
- Total samples processed: 17,632 audio files
- Classes:
  - Healthy speech
  - Dysarthric speech

Note: Dataset is not included due to size limitations.

---

## ⚙️ Feature Extraction

### Spectral Features
- MFCC (Mel Frequency Cepstral Coefficients)

### Pitch Features
- Fundamental frequency (F0)

### Perturbation Features
- Jitter (pitch variation)
- Shimmer (amplitude variation)
- HNR (harmonic-to-noise ratio)

### Time-Domain Features
- RMS Energy
- Zero Crossing Rate
- Duration

---

## 🧠 Machine Learning Models
- Logistic Regression
- Support Vector Machine (RBF Kernel)
- Random Forest
- XGBoost (Best performing model)

---

## 📊 Results

| Model | Accuracy | Precision | Recall | F1 Score |
|------|----------|----------|--------|----------|
| Logistic Regression | 84.04% | 82.24% | 73.20% | 77.46% |
| Random Forest | 96.02% | 97.32% | 91.91% | 94.54% |
| SVM (RBF) | 96.16% | 97.08% | 92.54% | 94.76% |
| XGBoost | 97.21% | 97.16% | 95.32% | 96.23% |

---

## 🔍 Model Explainability (SHAP)
- MFCC features contribute the most
- Low HNR indicates pathological speech
- Pitch instability reflects motor impairment
- Jitter and shimmer capture vocal irregularities

---

## 🧬 Neurophysiological Insight
Speech production is controlled by neural signals from the brain to vocal muscles. Neurological damage affects motor control, leading to unstable vocal fold vibration.

This results in:
- Increased jitter (irregular pitch)
- Increased shimmer (amplitude variation)
- Reduced HNR (noisy voice)

---

## 🏥 Clinical Relevance
- Enables early screening of neurological disorders
- Non-invasive (only voice required)
- Useful for telemedicine and remote diagnostics

---

## 🛠 Tech Stack
- Python
- Librosa
- Parselmouth
- Scikit-learn
- XGBoost
- SHAP
- NumPy, Pandas

---

## 📁 Project Structure
early-stroke-detection/
│── working_code.ipynb
│── features_debug.csv
│── best_threshold.txt
│── README.md

---

## 🚀 How to Run

Install dependencies:
pip install librosa scikit-learn xgboost shap pandas numpy

Run notebook:
jupyter notebook working_code.ipynb

---

## ⚠️ Limitations
- Dataset size can be improved
- Real-time deployment not implemented
- Requires clinical validation

---

## 🔮 Future Work
- Add deep learning models (CNN)
- Build real-time detection system
- Deploy as mobile/web application
- Expand dataset

---

## 👩‍💻 Authors
Alina Elizabeth Joji  
B.Tech Computer Science (AI)

Abek Abraham  
BCA Final Year

---

## 📌 Note
Dataset and trained models are not included due to GitHub size limitations. They can be shared upon request.

---

## ⭐
If you found this project useful, consider giving it a star.
