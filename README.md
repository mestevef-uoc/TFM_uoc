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
* 7.Results and Performance Metrics
* 8.How to Run the Project
* 9.Future Enhancements
* 10..References


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

# Technlogies Used 


# Datasets 

This project utilizes several datasets to train and test the machine learning models:

* 1. NSL-KDD Dataset
* Description: An improved version of the original KDD'99 dataset used for network intrusion detection. NSL-KDD resolves some inherent issues in the original dataset, such as redundancy and class imbalance.
* Features: 41 features, including protocol type, service, duration, and flag.
* Classes: Normal traffic and different types of attacks (Denial of Service, Probe, User to Root (U2R), and Remote to Local (R2L)).
* Use Case: This dataset is ideal for testing various ML classifiers' ability to distinguish between normal and malicious traff

* Reference  [ NSL-KDD Dataset Information](https://www.kaggle.com/datasets/hassan06/nslkdd)


