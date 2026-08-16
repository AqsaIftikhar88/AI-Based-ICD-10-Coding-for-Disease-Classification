# Enhancing Healthcare Efficiency: AI-Based ICD-10 Coding for Disease Classification

## 📌 Project Overview

This project presents an AI-based approach for automating the classification of diseases into ICD-10 codes based on patient-reported symptoms.

ICD-10 (International Classification of Diseases, 10th Revision) is widely used for disease classification, diagnosis documentation, healthcare management, and medical billing.

The proposed system uses Deep Learning, Natural Language Processing (NLP), and Machine Learning techniques to analyze symptom descriptions and predict the most relevant ICD-10 disease code.

---

## 🎯 Objectives

The main objectives of this project are:

- Automate the ICD-10 code classification process using Deep Learning.
- Predict disease codes based on patient symptoms.
- Compare the performance of Deep Learning and traditional Machine Learning models.
- Support multilingual symptom input through automatic translation.
- Provide an intuitive solution that can assist healthcare professionals in decision-making.

---

## 🔬 Methodology

The system follows the following workflow:

1. **Symptom Input**
   - The user provides a description of their symptoms.

2. **Text Preprocessing**
   - The input text is cleaned and preprocessed.
   - Stopwords are removed and the text is converted into a suitable format for classification.

3. **Tokenization & Sequence Processing**
   - Symptoms are converted into numerical sequences using a tokenizer.
   - Padding is applied to maintain a fixed input length.

4. **Deep Learning Classification**
   - A Recurrent Neural Network (RNN) based model is used for text classification.
   - The model predicts the most probable ICD-10 disease code.

5. **Machine Learning Comparison**
   - Traditional Machine Learning algorithms are also evaluated and compared with the Deep Learning approach.

6. **Multilingual Translation**
   - User symptoms can be entered in different languages.
   - The `googletrans` library automatically detects and translates the input into English before classification.

7. **Prediction & Confidence**
   - The system returns the predicted disease code along with its probability/confidence score.

---

## 🤖 Models Used

The project evaluates both Deep Learning and Machine Learning approaches.

### Deep Learning
- Recurrent Neural Network (RNN)

### Machine Learning
- Random Forest
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Naive Bayes

The models are evaluated using classification metrics and confusion matrices.

---

## 🌍 Multilingual Symptom Classification

To improve accessibility, the system includes a multilingual translation feature.

The `googletrans` library is used for automatic language detection and translation. User-submitted symptoms are translated into English before being passed to the disease classification model.

This feature supports input across multiple languages and improves usability for users who may not provide symptoms in English.

---

## 📊 Results

The developed model provides:

- Predicted ICD-10 disease code
- Confidence/probability score
- Probability levels for the available disease classes
- Comparison between Deep Learning and Machine Learning models
- Accuracy and loss analysis
- Confusion matrix evaluation

The RNN-based approach provides a list of possible diagnoses with probability scores, allowing the predicted results to be used as an assistance tool for healthcare decision-making.

---

## 💡 Project Strengths

- AI-based automation of ICD-10 disease classification.
- Symptom-based disease code prediction.
- Deep Learning based text classification.
- Comparison with traditional Machine Learning algorithms.
- Multilingual symptom translation.
- Probability-based prediction results.
- Potential to reduce manual ICD-10 code entry.
- Designed as a decision-support/assistance system for healthcare professionals.

---

## ⚠️ Limitations

The current system has limited ICD-10 code coverage.

The model was trained on a selected subset of **24 ICD-10 codes** due to the availability and quality of labeled data. This is only a small fraction of the complete ICD-10 code system.

Expanding the system to cover a broader range of ICD-10 codes would require a significantly larger and more diverse labeled medical dataset.

---

## 🚀 Future Work

Future improvements include:

- Expanding the dataset with more medical records and ICD-10 codes.
- Increasing the number of supported disease categories.
- Improving model accuracy with larger and better-quality datasets.
- Exploring advanced NLP architectures such as **BERT (Bidirectional Encoder Representations from Transformers)**.
- Integrating the system more deeply into healthcare applications.
- Improving multilingual medical-text understanding.

---

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Googletrans
- Jupyter Notebook

---

## 📁 Project Structure

```text
Enhancing-Healthcare-Efficiency-AI-Based-ICD-10-Coding-for-Disease-Classification/
│
├── dataset/
│   └── Symptom2Disease_50-checkpoint.csv
│
├── notebook/
│   └── Deep Learning.ipynb
│
├── requirements.txt
├── .gitignore
└── README.md
