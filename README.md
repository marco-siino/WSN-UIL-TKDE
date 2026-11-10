# WSN-UIL: Mitigating Dataset Biases in User Identity Linkage via Topology-Aware CNNs and Regressor Fusion

[![IEEE TKDE](https://img.shields.io/badge/Journal-IEEE%20TKDE-blue.svg)](https://www.ieee.org)
[![Python 3.10+](https://img.shields.io/badge/python-3.10%252B-brightgreen.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Official repository for the paper: **"Mitigating Dataset Biases in User Identity Linkage via Topology-Aware CNNs and Regressor Fusion"**, submitted to *IEEE Transactions on Knowledge and Data Engineering (TKDE)*.

---

## 📌 Abstract
User Identity Linkage (UIL) across heterogeneous online social networks (OSNs) suffers from a critical, unaddressed vulnerability: **dataset bias** introduced by ground-truth collection methodologies (e.g., self-disclosure profile links vs. cross-platform synchronized posting behaviors). Models trained and evaluated under a single paradigm yield overoptimistic performance that collapses in real-world cross-method scenarios. Furthermore, practical UIL faces extreme class imbalance ($1:N$). To address these challenges, we propose **WSN-UIL**, a hybrid multi-stage framework built on top of **Neo4j** that combines multi-hop topological expansion (*Tfriends*), a Deep Convolutional Neural Network (CNN) for JSON profiles, and a Logistic Regression meta-fusion layer.

---

## 🗂 Repository Structure
```text
WSN-UIL-TKDE/
│
├── data/                 # Datasets and train/test splits (Twitter, Instagram, FB, LinkedIn)
├── models/               # PyTorch CNN and Logistic Regression classifier scripts
├── utils/                # Graph engine (Neo4j / NetworkX) and evaluation metrics
├── notebooks/            # Google Colab development and experiment notebooks
│   ├── 01_Data_Preprocessing_and_Neo4j_Graph.ipynb
│   ├── 02_Deep_CNN_Profile_Training.ipynb
│   └── 03_Meta_Fusion_and_Evaluation.ipynb
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
