<div align="center">

# 🧬 AI & ML Project Portfolio

### A collection of Machine Learning, Deep Learning, NLP, and Reinforcement Learning projects

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Web%20App-000000?style=for-the-badge&logo=flask&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-RAG-009688?style=for-the-badge&logo=fastapi&logoColor=white)

</div>

---

## 🗺️ Table of Contents

- [Overview](#-overview)
- [Project Index](#-project-index)
- [Project Details](#-project-details)
- [Tech Stack](#-tech-stack)
- [Repository Structure](#-repository-structure)

---

## 🌐 Overview

This repository is a curated portfolio of **9 end-to-end AI/ML projects** spanning four major domains:

| Domain | Focus |
|:---:|---|
| 🧮 **Classical ML** | Regression & classification on structured/tabular data |
| 🧠 **Deep Learning** | CNNs for image classification & face/medical recognition |
| 💬 **NLP & RAG** | Recommender systems & retrieval-augmented chatbots |
| 🎮 **Reinforcement Learning** | Agents trained with PPO & DQN in simulated environments |

Each project is self-contained with its own code, dataset references, and — where applicable — a live deployment.

---

## 📌 Project Index

<table>
<tr>
<th>#</th><th>Project</th><th>Domain</th><th>Key Tech</th><th>Demo</th>
</tr>
<tr>
<td>01</td>
<td><a href="./Adult%20Census%20Income%20Classification/"><b>Adult Census Income Classification</b></a></td>
<td>ML · Classification</td>
<td>Logistic Regression, Decision Tree, Random Forest, KNN, SVM</td>
<td>—</td>
</tr>
<tr>
<td>02</td>
<td><a href="./Cancer%20Classification/"><b>Brain Tumor MRI Classification</b></a></td>
<td>DL · Medical Imaging</td>
<td>CNN, TensorFlow, 4-class MRI</td>
<td>—</td>
</tr>
<tr>
<td>03</td>
<td><a href="./car%20price%20prediction/"><b>Car Price Prediction</b></a></td>
<td>ML · Regression</td>
<td>Random Forest, Flask, Pickle</td>
<td>🌍 <a href="https://car-price-prediction-app-00au.onrender.com">Live</a></td>
</tr>
<tr>
<td>04</td>
<td><a href="./CIFAR%2010/"><b>CIFAR-10 Image Classification</b></a></td>
<td>DL · Computer Vision</td>
<td>CNN, Augmentation, BatchNorm</td>
<td>—</td>
</tr>
<tr>
<td>05</td>
<td><a href="./LFW%20face%20recognition/"><b>LFW Face Recognition</b></a></td>
<td>DL · Face Recognition</td>
<td>CNN, 7-class Face ID</td>
<td>—</td>
</tr>
<tr>
<td>06</td>
<td><a href="./Movie-Recommendation-System/"><b>Movie Recommendation System</b></a></td>
<td>ML · NLP / Recommender</td>
<td>TF-IDF, Cosine Similarity, Flask</td>
<td>—</td>
</tr>
<tr>
<td>07</td>
<td><a href="./Rag%20Chatbot%20/"><b>RAG Chatbot (Amazon 10-Q)</b></a></td>
<td>NLP · RAG</td>
<td>FastAPI, FAISS, Gemini AI</td>
<td>—</td>
</tr>
<tr>
<td>08</td>
<td><a href="./cartpole/"><b>CartPole (PPO)</b></a></td>
<td>RL · Control</td>
<td>Stable-Baselines3, PPO, Gymnasium</td>
<td>—</td>
</tr>
<tr>
<td>09</td>
<td><a href="./lunar%20lander/"><b>Lunar Lander (DQN)</b></a></td>
<td>RL · Control</td>
<td>Stable-Baselines3, DQN, Box2D</td>
<td>—</td>
</tr>
</table>

---

## 🔬 Project Details

### 01 · 💰 Adult Census Income Classification
> Predicts whether an individual's annual income exceeds **$50K** based on census data.

- **Dataset:** Adult Census Income Dataset (Kaggle) — ~32,561 records · 14 features
- **Models Compared:** Logistic Regression, Decision Tree, Random Forest, KNN, SVM
- **Metrics:** Accuracy, Precision, Recall, F1, ROC-AUC
- **Pipeline:** `Data Cleaning` → `Feature Engineering (One-Hot, StandardScaler)` → `Model Training` → `Evaluation`

📂 [`./Adult Census Income Classification/`](./Adult%20Census%20Income%20Classification/)

<br>

### 02 · 🧠 Brain Tumor MRI Classification
> Classifies brain MRI scans into **4 categories** — Glioma, Meningioma, No Tumor, Pituitary.

- **Dataset:** Brain Tumor MRI Dataset (Kaggle) — 5,600 train / 1,600 test images
- **Architecture:** 3 × Conv blocks (32 → 64 → 128) + GlobalAveragePooling + EarlyStopping
- **Target:** 90%+ accuracy

📂 [`./Cancer Classification/`](./Cancer%20Classification/)

<br>

### 03 · 🚗 Car Price Prediction
> Predicts the resale value of used cars — deployed live as a Flask web app.

- **Dataset:** CarDekho Vehicle Dataset (Kaggle) — ~301 records
- **Features:** Present Price, Kms Driven, Fuel Type, Transmission, Car Age
- **Model:** Random Forest Regressor
- **Deployment:** Flask + Pickle → Render

📂 [`./car price prediction/`](./car%20price%20prediction/) · 🌍 **[Live Demo](https://car-price-prediction-app-00au.onrender.com)**

<br>

### 04 · 🖼️ CIFAR-10 Image Classification
> Classifies 32×32 RGB images into **10 object categories**.

- **Dataset:** CIFAR-10 — 50,000 train / 10,000 test images (via TensorFlow)
- **Architecture:** 3 × Conv blocks (32 → 64 → 128) + Flatten + Dense + ReduceLROnPlateau
- **Target:** 85%+ accuracy

📂 [`./CIFAR 10/`](./CIFAR%2010/)

<br>

### 05 · 👤 LFW Face Recognition
> Recognizes faces of **7 public figures** from the Labeled Faces in the Wild dataset.

- **Dataset:** LFW — 1,288 grayscale images (50×37), 7 classes (via scikit-learn)
- **Architecture:** 3 × Conv blocks (32 → 64 → 128) + EarlyStopping (patience=20)
- **Challenge Handled:** Limited data via augmentation + stratified splitting

📂 [`./LFW face recognition/`](./LFW%20face%20recognition/)

<br>

### 06 · 🎬 Movie Recommendation System
> A content-based recommender served through a Flask web interface.

- **Dataset:** TMDB Movie Dataset
- **Pipeline:** `TF-IDF on Genres` → `Cosine Similarity Matrix` → `Top-N Recommendations`

📂 [`./Movie-Recommendation-System/`](./Movie-Recommendation-System/)

<br>

### 07 · 🤖 RAG Chatbot — Amazon 10-Q
> A Retrieval-Augmented Generation chatbot that answers questions about Amazon's quarterly filing, with **citations**.

- **Stack:** FastAPI + Sentence-Transformers (MiniLM) + FAISS + Gemini AI
- **Flow:** `Embed Query` → `FAISS Similarity Search` → `Top-k Excerpts` → `Gemini Grounded Answer`

📂 [`./Rag Chatbot/`](./Rag%20Chatbot%20/)

<br>

### 08 · 🎮 CartPole — PPO Reinforcement Learning
> Trains an agent to balance a pole on a cart using **PPO**.

- **Framework:** Stable-Baselines3, Gymnasium (CartPole-v1)
- **Components:** `train.py` · `evaluate.py` · `test.py` · `record_video.py` · `plot_training.py`

📂 [`./cartpole/`](./cartpole/)

<br>

### 09 · 🚀 Lunar Lander — DQN Reinforcement Learning
> Trains an autonomous spacecraft agent to safely land on a designated pad using **DQN**.

- **Framework:** Stable-Baselines3, Gymnasium (LunarLander-v3), Box2D physics
- **Components:** `train.py` · `evaluate.py` · `test.py` · `record_video.py` · `plot_training.py`

📂 [`./lunar lander/`](./lunar%20lander/)

---

## 🧰 Tech Stack

<table>
<tr><td><b>Languages</b></td><td>Python 3</td></tr>
<tr><td><b>ML / DL</b></td><td>Scikit-learn, TensorFlow / Keras</td></tr>
<tr><td><b>Reinforcement Learning</b></td><td>Stable-Baselines3, Gymnasium</td></tr>
<tr><td><b>NLP / RAG</b></td><td>TF-IDF, Sentence-Transformers, FAISS, Gemini AI</td></tr>
<tr><td><b>Web Frameworks</b></td><td>Flask, FastAPI</td></tr>
<tr><td><b>Data Handling</b></td><td>Pandas, NumPy</td></tr>
<tr><td><b>Visualization</b></td><td>Matplotlib, Seaborn</td></tr>
<tr><td><b>Deployment</b></td><td>Render, Pickle</td></tr>
<tr><td><b>Environment</b></td><td>Jupyter Notebook, VS Code</td></tr>
</table>

---

## 📁 Repository Structure

```text
.
├── Adult Census Income Classification/   # ML classification (5 models)
├── Cancer Classification/                # CNN brain tumor MRI (4-class)
├── car price prediction/                 # Random Forest + Flask web app
├── CIFAR 10/                             # CNN image classification (10-class)
├── LFW face recognition/                 # CNN face recognition (7-class)
├── Movie-Recommendation-System/          # TF-IDF + Flask recommender
├── Rag Chatbot/                          # RAG chatbot with FAISS + Gemini
├── cartpole/                             # PPO reinforcement learning
├── lunar lander/                         # DQN reinforcement learning
└── README.md                             # You are here
```

---

<div align="center">

**⭐ If you find this portfolio useful, consider giving it a star!**

</div>
