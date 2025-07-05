# Anxiety Level Classification Using LVQ and Wearable Data

This project implements a machine learning pipeline to classify anxiety levels using the Learning Vector Quantization (LVQ) algorithm based on physiological data from wearable devices. The model is designed to categorize stress into three classes: **Low**, **Normal**, and **High**, with a maximum accuracy of **95.26%**.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Results](#results)
- [Future Improvements](#future-improvements)

---

## 📘 Overview

Mental health has become a global concern in recent years. Physiological data from wearable devices like smartwatches and fitness trackers offers great potential in supporting real-time monitoring and early detection of stress and anxiety. This project utilizes LVQ (Learning Vector Quantization), a prototype-based supervised learning algorithm, to classify anxiety levels based on body humidity, temperature, and step count.

---

## 📊 Dataset

- **Source**: [Kaggle - Human Stress Detection Dataset](https://www.kaggle.com/datasets)
- **Name**: `Stress-Lysis.csv`
- **Size**: 2001 samples
- **Features**:
  - `Humidity` (10% – 30%)
  - `Temperature` (79°F – 99°F)
  - `Step_count` (0 – 200)
- **Label**: `Stress_Level` (0 = Low, 1 = Normal, 2 = High)

---

## 🧠 Methodology

1. **Data Preprocessing**:
   - Normalization using `MinMaxScaler`
   - Label encoding using `LabelEncoder`
   - Train-Test Split (80%-20%)

2. **Model Implementation**:
   - Custom implementation of the LVQ algorithm
   - Training with adjustable parameters:
     - `learning_rate`
     - `decay_factor`
     - `max_epochs`

3. **Evaluation Metrics**:
   - Accuracy
   - Comparison of predicted vs actual stress levels
   - Correlation analysis and feature impact

4. **Experiments**:
   - Effect of learning rate
   - Effect of decay factor
   - Impact of training data size
   - Cross-validation

---

## 🛠 Technologies Used

| Tool/Library     | Purpose                           |
|------------------|-----------------------------------|
| Python 3.11      | Programming language              |
| NumPy            | Numerical computation             |
| Pandas           | Data manipulation                 |
| Matplotlib       | Data visualization                |
| Seaborn          | Statistical plots                 |
| Scikit-learn     | Preprocessing and utilities       |
| Jupyter Notebook | Interactive development           |