# CyberAttackDetection

# Machine Learning-Based Intrusion Detection System for IoT Networks

## Project Overview

This project aims to enhance the security of Internet of Things (IoT) networks through the implementation of a machine learning-based Intrusion Detection System (IDS). By leveraging data mimicking real-world attack scenarios, our models can predict and classify various types of routing attacks with high accuracy, contributing to more secure IoT environments.

## Contributors

- Sudalakshmee Chiniah
- Mahira Pathan
- Elizabeth Wei


## Data Sources

The datasets consist of .csv files for four different routing attacks targeting the RPL protocol, collected via the Contiki network simulator (Cooja). These include the Blackhole Attack, Flooding Attack, DODAG Version Number Attack, and Decreased Rank Attack. This dataset was obtained from the IEEEDataPort. In this repo, we will show work done on the ranking dataset only. The multi-class will not be shown.

## Models Used

- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Decision Trees**
- **Random Forest**
- **Extreme Gradient Boosting (XGBoost)**

## Key Results

- A 99.3% F1-score was achieved in predicting the presence of an attack using a KNN model.
- A 99.6% F1-score was obtained for the classification of attack types using a Random Forest model.

## Methodology

### Binary Classification

Models such as Logistic Regression, Decision Trees, and KNN were employed to predict whether an attack was present based on features extracted from the network traffic.

### Multi-Classification

Advanced models like XGBoost and Random Forest were used to classify the type of attack, demonstrating high accuracy and robustness in detecting sophisticated threats.


## Metrics

Performance metrics such as accuracy, precision, recall (sensitivity), specificity, F1-score, and false negative rate were used to evaluate the models, with a focus on minimizing false negatives due to the high cost associated with missed detections.

## Experimental Analysis

### Data Preprocessing

Key preprocessing steps included:
- Addressing class imbalance with the ADASYN algorithm.
- Feature normalization to prevent dominance of particular variables.
- Dropping highly correlated features to reduce model complexity and overfitting.

### Model Evaluation

Models were evaluated based on their performance on the test sets, with considerations of overfitting checked through validation techniques.

## Conclusion

The machine learning models developed demonstrate high efficacy in detecting and classifying routing attacks in IoT networks, with potential for real-world application to improve network security.
