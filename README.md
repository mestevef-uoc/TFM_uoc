# TFM_uoc
Treball final de master - Use of Artificial Intelligence and Machine Learning in SOCs network and systems security

Welcome to the TFM_UOC repository! This project is part of a Treball final de Master TFM  focused on enhancing the capabilities of Security Operations Centers (SOC) using Artificial Intelligence (AI) and Machine Learning (ML). This repository documents the development process, implementation, and findings of the project.

Table of Contents
* 1.Introduction
* 2.Objectives
* 3.Methodology
* 4.System Architecture
* 5.Technologies Used
* 6.Datasets
* 7.How to Run the Project
* 8.Notebook overview
* 9.Possible Future Enhancements
* 10.References


# Introduction 

This is the first approach to understanding how Security Operations Centers (SOC) can leverage AI and ML to improve their performance in detecting and mitigating cyber threats. Traditional SOCs often struggle with data overload, false positives, and slow response times. By integrating advanced ML models, this project aims to:

* Detect and predict attacks more accurately.
* Automate certain security operations.
* Provide real-time alerts and insights using both supervised and unsupervised learning models.


# Objectives

* Improve incident detection and response times.
* Reduce the rate of false positives in threat detection.
* Analyze and visualize active cyber threats in a simulated SOC environment.
* Evaluate the performance of different ML classifiers for identifying attacks such as DDoS, malware, and network anomalies.


# Methodology 

* Data Preprocessing: Cleaning and transforming datasets, including network logs and PCAP data.
* Feature Engineering: Extracting relevant features such as packet size, flow duration, and protocol usage patterns.
* Model Selection: Training and evaluating machine learning models such as Decision Trees, Random Forest, SVM, and MLPs.
* Evaluation Metrics: Measuring performance using accuracy, precision, recall, F1-score, and confusion matrices.

# System Architecture

* The project is based on a modular architecture consisting of:

* Data Collection Layer: Ingests network logs and packet captures.
* Preprocessing Module: Handles data transformation and labeling.
* Model Training Module: Trains and tests ML models using the preprocessed data.

# Technlogies Used 

* Python Libraries: Scikit-learn, TensorFlow, Pandas, NumPy, Matplotlib.
* Tools: Google Colab.
* Frameworks: NIST Cybersecurity Framework for structured SOC design​NIST.CSWP.29.


# Datasets 

This project utilizes several datasets to train and test the machine learning models:

* # 1. NSL-KDD Dataset
* Description: An improved version of the original KDD'99 dataset used for network intrusion detection. NSL-KDD resolves some inherent issues in the original dataset, such as redundancy and class imbalance.
* Features: 41 features, including protocol type, service, duration, and flag.
* Classes: Normal traffic and different types of attacks (Denial of Service, Probe, User to Root (U2R), and Remote to Local (R2L)).
* Use Case: This dataset is ideal for testing various ML classifiers' ability to distinguish between normal and malicious traff

* Reference  [ NSL-KDD Dataset Information](https://www.kaggle.com/datasets/hassan06/nslkdd)

#  2. UNSW-NB15 Dataset 

* Description: A more modern dataset designed to address the limitations of older datasets like KDD’99. UNSW-NB15 captures real network traffic and simulates a wide range of attack types.
* Features: 49 features, including flow-based features like TCP window size, packet count, and data volume.
* Classes: Includes both normal and 9 types of attacks (e.g., Exploit, Fuzzers, DoS, Worms).
* Use Case: This dataset is used to benchmark more advanced classifiers and evaluate their ability to detect complex attacks in realistic scenarios.

* Reference [UNSW-NB15 Dataset Information ] https://research.unsw.edu.au/projects/unsw-nb15-dataset 

# 3. Microsoft Security Incident Prediction Dataset
* Description: This dataset, hosted on Kaggle, contains logs and telemetry data used for predicting security incidents and outcomes. The dataset is useful for understanding patterns in real-world enterprise security incidents.
* Progress: The dataset has been added to the project plan but is not included in the repository due to its large file size.  but it still requires fine-tuning and preprocessing to handle missing values, normalize features, and balance class distributions.
* Next Steps: Perform feature selection and hyperparameter optimization for better prediction accuracy.

* Reference [Microsoft Security Incident prediction ] https://www.kaggle.com/datasets/Microsoft/microsoft-security-incident-prediction/data


# 7. How to run the project 

*  Clone the repository:
*   git clone https://github.com/mestevef-uoc/TFM_uoc.git
* Install dependencies
* Run the Jupyter notebook or Python scripts in your preferred IDE or Google Colab. 

# 8. Notebook overview 

* GUIDE.ipynb  -> This notebook focuses on providing an introduction and instructions for working with a large-scale security incident dataset that contains detailed records of alerts and incidents logged by a Security Information and Event Management (SIEM) system.
* NSL-KDD.ipynb -> This notebook is specific to the NSL-KDD dataset and focuses on performing network intrusion detection by identifying malicious and normal traffic.
* Random_forest_NSL_KDD_dataset.ipynb (Random Forest on NSL-KDD) -> This notebook is dedicated to training and evaluating the Random Forest classifier on the NSL-KDD dataset.
* UNSW-NB15.ipynb (UNSW-NB15 Dataset Analysis) -> This notebook is focused on processing and analyzing the UNSW-NB15 dataset, which contains real-world modern attack scenarios.

# 9. Possible future enchancements 

* Deep Learning Models -  
    * Implement deep learning models like Recurrent Neural Networks (RNNs) or Long Short-Term Memory (LSTM) networks to capture sequential dependencies in the dataset (e.g., detecting patterns in alert sequences leading to incidents).
    * Use Transformer-based architectures (like BERT for time-series) for better representation of large-scale data.

* Explainable AI (XAI) Integration 
    * Incorporate tools such as SHAP (SHapley Additive Explanations) or LIME (Local Interpretable Model-agnostic Explanations) to provide interpretability and explain why a particular alert or incident was classified as malicious or benign.
    * SOC analysts could use these explanations to gain insights into model decisions and trust the system's predictions
