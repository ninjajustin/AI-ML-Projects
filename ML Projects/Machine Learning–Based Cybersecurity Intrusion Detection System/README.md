# Machine Learning–Based Cybersecurity Intrusion Detection System

This project implements a scalable machine learning pipeline for detecting malicious network traffic using the CIC-IDS 2017 dataset, a real-world intrusion detection benchmark. The system processes raw network flow data, performs feature engineering, and trains supervised classifiers to distinguish benign traffic from cyber attacks.

System Overview

Built an end-to-end ML pipeline that ingests labeled network traffic data and outputs binary intrusion predictions.

Refactored the workflow into reusable functions to support multiple datasets and attack scenarios.

Designed the pipeline to generalize across 8 different datasets, each representing distinct traffic conditions and attack types.

Data Processing & Feature Engineering

Converted multi-class attack labels into a binary classification format (BENIGN vs. attack).

Applied domain-aware feature engineering using networking concepts:

Identified well-known service ports (HTTP, HTTPS, FTP, SSH, etc.)

One-hot encoded important ports and grouped low-signal ports into an "other" category

Selected and analyzed high-impact features such as:

Flow duration

Packet length statistics

Source and destination ports

Used visualizations (histograms, bar charts) to validate feature usefulness and detect bias.

Model Development & Evaluation

Implemented and compared multiple classifiers:

Naive Bayes

Support Vector Machines

Neural Networks (MLP)

Decision Trees

Random Forests

Evaluated models using 10-fold stratified cross-validation to ensure stable performance.

Selected Random Forest as the final model based on accuracy, robustness, and low variance across folds.

Achieved consistently high accuracy across all datasets, including noisy and imbalanced traffic distributions.

Engineering & ML Concepts Applied

Modular ML pipeline design

Supervised learning & binary classification

Feature encoding and data preprocessing

Cross-validation and model benchmarking

Ensemble methods (Random Forests)

Handling edge cases (single-class datasets)

Applying ML in a domain with limited prior expertise

Takeaways

This project demonstrates my ability to build production-style ML pipelines, adapt to unfamiliar domains, and write reusable, data-driven code. It highlights practical skills in data processing, model evaluation, and system generalization—core competencies for software engineering roles working with ML-driven systems.