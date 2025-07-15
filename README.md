# Intrusion Detection using Deep Learning on NSL-KDD and TON_IoT Datasets

This project explores deep learning–based intrusion detection systems (IDS) using two benchmark datasets: **NSL-KDD** and **TON_IoT**. The goal is to build, train, and evaluate robust models for network anomaly detection in both traditional and IoT-based environments.

## 🔍 Datasets Used

### 1. NSL-KDD
- A refined version of the KDD’99 dataset, addressing redundancy and class imbalance.
- Benchmark for IDS models in traditional network settings.

### 2. TON_IoT
- Modern dataset capturing telemetry from IoT/IIoT devices.
- Multiple attack categories targeting smart environments.

## 🧠 Models & Methodology

### Common Steps
1. **Data preprocessing**: label encoding, normalization, train-test split  
2. **Model training**: MLP architectures implemented in TensorFlow/Keras  
3. **Evaluation metrics**: Accuracy, Precision, Recall, F1‑score, Confusion Matrix  

### NSL-KDD
- **Architecture**: 3 hidden layers + dropout  
- **Optimization**: early stopping on validation loss  
- **Results**:
  - Accuracy: **99.32%**
  - F1 Score: **0.993**

### TON_IoT
- **Task**: binary classification (normal vs. attack)  
- **Architecture**: 4 dense layers + dropout, binary cross‑entropy loss  
- **Results**:
  - Accuracy: **99.85%**
  - F1 Score: **0.998**

## 📊 Evaluation Summary

| Dataset   | Accuracy | Precision | Recall | F1 Score |
|-----------|----------|-----------|--------|----------|
| NSL-KDD   | 99.32%   | 0.993     | 0.993  | 0.993    |
| TON_IoT   | 99.85%   | 0.999     | 0.998  | 0.998    |

## 🛠️ Dependencies

- Python ≥ 3.7  
- TensorFlow / Keras  
- NumPy, Pandas, Scikit‑learn  
- Matplotlib, Seaborn  

