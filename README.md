# Intrusion_Detection_System
Description : This project implements an AI/ML-based Intrusion Detection System (IDS) using the Cybersecurity Intrusion Detection dataset. The goal is to classify network sessions as either normal or anomalous (attack) based on various features such as packet size, login attempts, encryption usage, and more.
Dataset
Source: Kaggle - Cybersecurity Intrusion Detection Dataset

Features Used:network_packet_size, protocol_type, login_attempts, session_duration,encryption_used, ip_reputation_score, failed_logins, browser_type,unusual_time_access

Target Column: attack_detected (0 = Normal, 1 = Anomalous)

Machine Learning Approach
Model Used: Random Forest Classifier
Why Random Forest? It handles both numerical and categorical data well, is robust to overfitting, and gives good accuracy out of the box.

Preprocessing
Dropped non-useful identifier column: session_id

Applied LabelEncoder to categorical features

Normalized features using StandardScaler

Split data into training (80%) and testing (20%)
Visualization:Used PCA (Principal Component Analysis) to reduce high-dimensional feature space to 2D

Plotted normal vs. anomalous behavior to visually understand model performance
Model Evaluation
Accuracy, precision, recall, and F1-score were calculated

Accuracy Example: 94.0%

Confusion matrix and classification report used for performance analysis

Output: A 2D scatter plot showing PCA-reduced feature space with:
Blue = Normal sessions
Red = Attack sessions

