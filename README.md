---

# Network Anomaly Detection System using Deep Learning

## Overview

This project implements a **Network Anomaly Detection System** using a **Multi-Layer Perceptron (MLP)** built with TensorFlow/Keras. The goal is to identify unusual patterns in network traffic that may indicate cyber threats such as intrusions or attacks.

Anomaly detection is a critical component in cybersecurity, helping organizations detect suspicious behavior in real time and respond proactively.

---

## Objectives

* Built an end-to-end anomaly detection pipeline
* Performed data preprocessing & feature engineering
* Designed a deep learning classification model (MLP)
* Evaluated using multiple performance metrics
* Visualized training performance and model behavior

---
## System Architecture

```bash
Raw Data → Preprocessing → Feature Encoding → Scaling → MLP Model → Predictions → Evaluation
```
---
## Tech Stack

| Category         | Tools Used          |
| ---------------- | ------------------- |
| Programming      | Python              |
| Data Processing  | Pandas, NumPy       |
| Machine Learning | Scikit-learn        |
| Deep Learning    | TensorFlow / Keras  |
| Visualization    | Matplotlib, Seaborn |

---

## Dataset

The dataset used:

```
Network_anomaly_data.csv
```

It includes:

* Network traffic features
* Categorical attributes (protocol, service, flag)
* Target variable (`attack`) representing normal vs anomaly classes

---

## Technologies Used

* Python 
* Pandas & NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib & Seaborn

---

## Workflow

### 1. Data Preprocessing

* Handle missing values
* Encode categorical features using one-hot encoding
* Label encode target variable
* Normalize features using StandardScaler

### 2. Train-Test Split

* 70% training / 30% testing
* Stratified split to preserve class distribution

### 3. Model Architecture (MLP)

* Input layer
* Dense layers: 128 → 64 → 32 neurons
* Dropout layers (0.4) to prevent overfitting
* Output layer with Softmax activation

### 4. Model Compilation

* Optimizer: Adam
* Loss: Sparse Categorical Crossentropy
* Metric: Accuracy

### 5. Training

* Epochs: 10
* Batch size: 64
* Validation split: 20%

---

## Evaluation Metrics

The model is evaluated using:

* Accuracy
* Precision (weighted)
* Recall (weighted)
* F1-Score
* Confusion Matrix

---

## Visualizations

* Training vs Validation Loss
* Training vs Validation Accuracy
* Confusion Matrix Heatmap

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/network-anomaly-detection.git
cd network-anomaly-detection
```

### 2. Install Dependencies

```bash
pip install pandas numpy scikit-learn tensorflow matplotlib seaborn
```

### 3. Run the Script

```bash
python AI_Network_Anomaly_Saranja.ipynb
```

---

## Results

* The MLP model successfully classifies network anomalies
* Performance is evaluated using multiple metrics
* Visualization helps detect overfitting or underfitting

---

## Future Improvements

* Use more advanced models (e.g., LSTM, Autoencoders)
* Hyperparameter tuning
* Handle class imbalance with techniques like SMOTE
* Deploy model as a real-time monitoring system

---

## License

This project is for educational purposes

---
## Author

Saranja Navaneethakumar
