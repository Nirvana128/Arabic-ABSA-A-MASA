# 🌟 Arabic Multi-Domain Aspect-Based Sentiment Analysis (ABSA)

## 📝 About The Project
This repository contains a comprehensive, multi-domain Aspect-Based Sentiment Analysis (ABSA) system designed specifically for the Arabic language[cite: 1]. The project tackles the critical challenge of class imbalance in sentiment analysis, particularly the severe under-representation of neutral sentiments[cite: 1].

📄 **Full Research Paper:** [Read the detailed paper here](./Arabic_ABSA_Paper.pdf)

## 🎯 Key Objectives & Contributions
* **Data Augmentation & Balancing:** Successfully reduced the class imbalance ratio from 12.2 to 2.36 by integrating 7,423 real hotel reviews and generating 3,200 synthetic neutral Arabic sentences using **Gemini Pro**[cite: 1].
* **Multi-Domain Focus:** Handles both Modern Standard Arabic (MSA) and Dialectal Arabic (DA) across 6 distinct domains (Restaurants, Telecommunications, Products, Attractions, Movies, and Hotels)[cite: 1].
* **Extensive Model Comparison:** Benchmarked 8 different models, ranging from classical Machine Learning (TF-IDF + Logistic Regression) to Sequential Models (BiLSTM) and State-of-the-Art Transformers (MARBERT, QARiB, CAMELBERT, etc.)[cite: 1].

## 🗄️ Dataset Overview
The final balanced dataset comprises **16,678 validated samples**[cite: 1]:
* 🟢 **Positive:** 8,504 (47.2%)[cite: 1]
* 🔴 **Negative:** 4,569 (25.4%)[cite: 1]
* ⚪ **Neutral:** 3,605 (20.0%)[cite: 1]

## 🚀 Performance & Results
* **Top Performing Models:** **MARBERT** and **QARiB** achieved the highest performance[cite: 1].
* **Accuracy:** 93.3%[cite: 1]
* **Macro F1-Score:** 92%[cite: 1]
* **Neutral Class Breakthrough:** The data enhancement pipeline drastically improved the neutral F1-score for models like CAMELBERT from 0.14 (on imbalanced data) to 0.89[cite: 1].

## 📂 Repository Structure
* `Data_Preparation/`: Jupyter Notebooks for data cleaning, hotel dataset merging, and synthetic data integration.
* `Models/`: Individual notebooks for training and fine-tuning the 8 evaluated models (e.g., MARBERT, BiLSTM, AraBERT).
* `Arabic_ABSA_Paper.pdf`: The complete research paper documenting the methodology, error analysis, and findings.

## 🛠️ Technologies & Tools Used
* **Languages:** Python
* **Libraries:** HuggingFace Transformers, TensorFlow/Keras, Scikit-Learn, Pandas, NLTK, imbalanced-learn (SMOTE).
