🛍️ E-COMMERCE TEXT CLASSIFICATION USING MULTIPLE OPTIMIZERS
📘 Project Overview
This project implements an E-commerce product text classification system using deep learning techniques. The model classifies product descriptions into appropriate categories such as Household, Clothing, Electronics, etc. It also compares the performance of multiple optimizers — including SGD, Adam, RMSProp, Adagrad, and Nadam — to identify which achieves the best accuracy and convergence speed.
🧭 Workflow
Each step is modular and automated — from dataset loading to model evaluation.
•	Dataset → Preprocessing → Tokenization → Model Training (with multiple optimizers) → Evaluation → Visualization
⚙️ Features
•	Automatic dataset download from Kaggle via kagglehub
•	Tokenization and padding using TensorFlow’s Tokenizer
•	Multi-class label encoding for product categories
•	Training and validation with five optimizers (SGD, Adam, RMSProp, Adagrad, Nadam)
•	Comparative analysis of accuracy and loss curves
•	Reproducibility through fixed random seeds
📂 Input Dataset
Source: Kaggle — E-commerce Text Classification Dataset
Sample Columns:
Column	Example
Category	Household
Text	SAF 'Floral' Framed Painting (Wood, 30 inch x 40 inch)...
🧠 How It Works
•	1️⃣ Dataset Loading
The dataset is automatically fetched using kagglehub and loaded as a DataFrame.
•	2️⃣ File Detection
Identifies the main .csv file dynamically for loading.
•	3️⃣ Data Preparation
Extracts text and label columns, encodes labels, and splits into train and test sets.
•	4️⃣ Tokenization & Padding
Converts text to sequences and pads them to uniform length.
•	5️⃣ Model Training
Trains using different optimizers to compare convergence and validation accuracy.
•	6️⃣ Evaluation
Plots validation accuracy/loss and compares final optimizer performance.
📊 Example Results
Optimizer	Final Validation Accuracy	Final Validation Loss
Adam	0.89	0.31
RMSProp	0.87	0.35
Nadam	0.88	0.34
Adagrad	0.72	0.68
SGD	0.65	0.75
Adam, Nadam, and RMSProp perform best, while SGD and Adagrad show slower learning and higher loss values.
🚀 How to Run the Script
Prerequisites: Python 3.8+ and the following libraries:
•	pip install tensorflow pandas scikit-learn kagglehub matplotlib
Run the notebook sequentially: Dataset download → Preprocessing → Tokenization → Model training → Evaluation
📤 Outputs
•	Accuracy and loss graphs for each optimizer
•	Final summary table comparing all optimizers
•	Sample predictions on test data
🤝 Contributors
Anushika Gupta (Team Lead) — Model Design & Optimizer Analysis
Akash — Data Preparation 
Suryansh jain-Evaluation Scripts
Supervised by:
Dr. Rajni Ranjan Singh (HoD, CAI Department, MITS)
📜 License
This repository is provided for academic and educational purposes only. Reproduction or redistribution without permission is prohibited.
⭐ Acknowledgment
We thank Madhav Institute of Technology and Science (MITS), Gwalior for their guidance and support in completing this project.

