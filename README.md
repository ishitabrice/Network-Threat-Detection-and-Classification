# 🛡️ Network Intrusion Detection System

> **Machine Learning & Deep Learning for Network Intrusion Detection using the NSL-KDD Dataset**

A machine learning and deep learning–based **Network Intrusion Detection System (NIDS)** designed to identify and classify malicious network activity from network traffic patterns.

This project explores multiple machine learning and deep learning techniques for cybersecurity, with a focus on detecting network attacks and distinguishing malicious traffic from normal network activity.

---

## 📌 Project Overview

Cyber attacks are becoming increasingly sophisticated, making automated network monitoring and intrusion detection essential for modern cybersecurity systems.

This project uses the **NSL-KDD dataset** to build and evaluate an intrusion detection system.

The workflow focuses on:

* 🔹 Data preprocessing and feature engineering
* 🔹 Extracting relevant network traffic features
* 🔹 Feature normalization and transformation
* 🔹 Training multiple machine learning and deep learning models
* 🔹 Comparing model performance
* 🔹 Detecting and classifying malicious network activity

The project evaluates several machine learning approaches, with particular emphasis on neural network models such as **Multi-Layer Perceptron (MLP)** and **Long Short-Term Memory (LSTM)**.

---

## 🎯 Objectives

* Develop a machine learning–based Network Intrusion Detection System.
* Analyze network traffic using the NSL-KDD dataset.
* Extract and preprocess relevant network features.
* Experiment with different machine learning and deep learning approaches.
* Evaluate models using appropriate classification metrics.
* Reduce unnecessary feature overhead while maintaining detection performance.

---

## 🗂️ Dataset

### NSL-KDD

The project uses the **NSL-KDD dataset**, a refined version of the original KDD'99 dataset commonly used for research in network intrusion detection.

The dataset contains network connection records representing both:

* ✅ Normal network activity
* ⚠️ Various types of network attacks

**Official Dataset:**

https://www.unb.ca/cic/datasets/nsl.html

Typical files used in the project include:

```text
KDDTrain.txt
KDDTest.txt
```

---

## 🧠 Models

The project experiments with multiple machine learning and deep learning approaches.

### Multi-Layer Perceptron (MLP)

A feed-forward neural network used to learn complex relationships between network traffic features and intrusion classes.

### Long Short-Term Memory (LSTM)

An RNN architecture capable of learning sequential patterns in network traffic data.

The LSTM model achieved a **recall score of approximately 0.9904** in the reported experiments.

Other implemented approaches include:

* K-Nearest Neighbors
* Logistic Regression
* Linear SVM
* Random Forest
* Neural Network models

---

## 🔄 Project Workflow

```text
                NSL-KDD Dataset
                       │
                       ▼
               Data Preprocessing
                       │
                       ▼
                Feature Engineering
                       │
                       ▼
              Feature Normalization
                       │
                       ▼
                 Train / Test Split
                       │
             ┌─────────┴─────────┐
             ▼                   ▼
      Machine Learning      Deep Learning
             │                   │
             │              ┌────┴────┐
             │              ▼         ▼
             │             MLP       LSTM
             │              │         │
             └──────────────┴─────────┘
                       │
                       ▼
                 Model Evaluation
                       │
                       ▼
            Intrusion Detection Results
```

---

## 📊 Results

The experiments demonstrate that appropriate preprocessing and feature manipulation can improve intrusion detection performance while reducing unnecessary modelling overhead.

### Highlight

| Model    | Metric |      Score |
| :------- | :----- | ---------: |
| **LSTM** | Recall | **0.9904** |

> The reported LSTM recall of **0.9904** indicates that the model detected a very high proportion of malicious instances in the evaluated data.

---

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Scikit-learn**
* **TensorFlow / Keras**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**
* **Google Colab**

---

## ▶️ Running the Notebook

The notebooks can be executed using either **Google Colab** or **Jupyter Notebook**.

### Google Colab

Upload the required notebook to Google Colab and run the cells sequentially.

### Jupyter Notebook

Launch Jupyter Notebook from the project directory:

```bash
jupyter notebook
```

Then open the required notebook and execute the cells.

---

## 📚 Research Reference

This project is **partially based on the following research work**:

**Network intrusion detection using deep learning techniques**

Research paper:

https://www.sciencedirect.com/science/article/pii/S0925231219315759

---

## 📁 Project Structure

```text
NIDS-Using-Deep-Learning/

│
├── datasets/
│   └── bin_data_test.csv
│
├── Models/
│   ├── config.py
│   ├── K-nearestneighbor.py
│   ├── LogisticRegression.py
│   ├── LSTM.py
│   ├── LSVM.py
│   ├── Multi_perceptron.py
│   ├── NeuralNetworks.py
│   └── RandomForest.py
│
├── data_load.py
├── data-preprocessing-nsl-kdd(1).ipynb
├── extract_feat.py
├── Imports.py
├── nids-models-ml-dl (1).ipynb
├── nsl-kdd-models.ipynb
└── README.md
```

> Dataset files may be excluded from the repository depending on their size and redistribution restrictions.

---

## 🚀 Key Takeaways

* Network traffic can be analyzed using machine learning to detect cyber attacks.
* Feature preprocessing plays an important role in intrusion detection performance.
* Different machine learning and deep learning models can be applied to network traffic classification.
* Neural networks can learn complex patterns from network traffic.
* LSTM demonstrated strong intrusion detection performance in the experiments.
* Proper feature manipulation can help reduce modelling overhead without significantly compromising detection capability.

---

## 👤 Author

**Siba Sankar Mallick**

B.Tech — Mathematics & Computing
IIT Guwahati

---

⭐ If you find this project useful, consider giving the repository a star!
