Intrusion Detection using Deep Learning on NSL-KDD and TON_IoT Datasets
This project explores deep learning-based intrusion detection systems (IDS) using two benchmark datasets: NSL-KDD and TON_IoT. The goal is to build, train, and evaluate robust models for network anomaly detection in both traditional and IoT-based environments.

🔍 Datasets Used
1. NSL-KDD
A refined version of the KDD’99 dataset, addressing redundancy and imbalance issues.

Used for benchmarking IDS models in traditional network settings.

2. TON_IoT
A modern dataset capturing telemetry from IoT/IIoT devices.

Contains multiple attack categories targeting smart environments.

🧠 Models & Methodology
Common Approach:
Data preprocessing: label encoding, normalization, and train-test splits.

Model training using deep learning (MLP-based architectures).

Evaluation using metrics like Accuracy, Precision, Recall, F1-score, and Confusion Matrix.

NSL-KDD:
Trained an MLP classifier with:

3 hidden layers, dropout regularization.

Early stopping based on validation loss.

Achieved:

Accuracy: 99.32%

F1 Score: 0.993

High precision and recall across all classes.

TON_IoT:
Binary classification of normal vs attack traffic.

Preprocessed CSV logs from telemetry sources.

Model architecture:

4 dense layers with ReLU activation and dropout.

Binary cross-entropy loss.

Achieved:

Accuracy: 99.85%

F1 Score: 0.998

📊 Evaluation
Dataset	Accuracy	Precision	Recall	F1 Score
NSL-KDD	99.32%	0.993	0.993	0.993
TON_IoT	99.85%	0.999	0.998	0.998

Confusion matrices show minimal false positives/negatives.

Models generalize well to unseen test data.

🛠️ Dependencies
Python ≥ 3.7

TensorFlow / Keras

NumPy, Pandas, Scikit-learn

Matplotlib, Seaborn

Install via:

bash
Copy
Edit
pip install -r requirements.txt
📁 Structure
bash
Copy
Edit
├── final_model_nsl_kdd.ipynb     # NSL-KDD Model Training and Evaluation
├── Ton_Iot_Run_final_results.ipynb  # TON_IoT Model Training and Evaluation
├── README.md
└── requirements.txt              # Dependencies (to be added)
🚀 Future Work
Integrate real-time detection pipeline.

Expand to multi-class detection on TON_IoT.

Compare with classical ML algorithms for baseline benchmarking.

📌 Citation
If you use this work, please cite the relevant datasets and credit this repository.
