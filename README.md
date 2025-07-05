# Anxiety Level Classification Using LVQ and Wearable Data

This repository contains the implementation of the Learning Vector Quantization (LVQ) algorithm to classify anxiety levels based on physiological data collected from wearable devices. The dataset is preprocessed, trained, and evaluated using various configurations such as learning rate, decay factor, and training data size.

## 📊 Dataset

- Source: [Kaggle - Human Stress Detection Dataset](https://www.kaggle.com/datasets)
- Filename: `Stress-Lysis.csv`
- Size: 2001 samples
- Features:
  - `Humidity` (10–30%)
  - `Temperature` (79–99°F)
  - `Step_count` (0–200)
- Target: `Stress_Level` (0 = Low, 1 = Normal, 2 = High)

## ⚙️ Project Structure

- `lvq-anxiety-classification.ipynb`: Main Jupyter Notebook containing:
  - Data preprocessing
  - LVQ class implementation
  - Accuracy calculation
  - Parameter experiments (learning rate, decay factor, training size)
  - Cross-validation
  - Visualization of prediction results

## 🧠 Algorithm

The project uses a custom implementation of the **Learning Vector Quantization (LVQ)** algorithm, trained and tested on normalized physiological data. The LVQ model uses Euclidean distance to find the closest class prototype and iteratively updates weights based on prediction correctness.

## 🧪 Experiments

- **Learning Rate Sensitivity**: Evaluates accuracy across different learning rates from 0.1 to 1.0.
- **Decay Factor Impact**: Tests how decay in learning rate affects convergence and performance.
- **Training Size Variations**: Measures model accuracy using training data from 10% to 80%.
- **Cross Validation**: 3-fold evaluation to assess model generalization.

## 🛠️ Technologies
- Python 3.11
- Jupyter Notebook / VS Code
- Libraries:
    - NumPy
    - Pandas
    - Matplotlib
    - Seaborn
    - Scikit-learn