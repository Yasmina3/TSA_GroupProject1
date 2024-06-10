# TSA_GroupProject1
Time Series Classification of ECG Signals
Introduction
Electrocardiogram (ECG) signals are crucial for monitoring heart activity and diagnosing various cardiac conditions. The primary objective of this project is to classify ECG signals into two categories: normal heartbeats and abnormal heartbeats (Myocardial Infarction).

ECG signals are time series data that represent the electrical activity of the heart over time. This project involves applying time series classification techniques to accurately distinguish between normal and abnormal heartbeats.

Objectives
The main objectives of this project are:

To preprocess and prepare ECG time series data for classification.
To explore and apply different machine learning algorithms for classifying ECG signals.
To handle class imbalance using techniques like Synthetic Minority Over-sampling Technique (SMOTE).
To transform the time series data into different representations such as Continuous Wavelet Transform (CWT) and Gramian Angular Field (GAF) for enhanced feature extraction.
To evaluate the performance of the classification models using appropriate metrics.
Data Set
The dataset consists of ECG recordings, each containing 96 data points representing a single heartbeat. Each sample is labeled as either normal or abnormal. Normal heartbeats are labeled as 1 and abnormal heartbeats (Myocardial Infarction) are labeled as -1.

Approach
Data Preprocessing:

Load the ECG data and separate the features and labels.
Standardize the labels by converting -1 to 0.
Handling Class Imbalance:

Apply SMOTE to balance the class distribution in the training data.
Feature Extraction:

Apply Continuous Wavelet Transform (CWT) to capture both time and frequency information.
Transform the time series data into Gramian Angular Field (GAF) images to capture temporal correlations.
Model Training and Evaluation:

Train various machine learning models on the transformed data.
Evaluate the models using metrics such as accuracy, precision, recall, F1 score, and confusion matrix.
Models and Techniques
Convolutional Neural Network (CNN):

Architecture definition and fitting with trial and error to find the best configuration.
Best configuration resulted in significant accuracy improvements.
Support Vector Machine (SVM):

Applied with different kernels; the RBF kernel was found to be the most effective.
Parameter tuning with grid search to optimize C and gamma parameters for the RBF kernel.
Results
The SVM with RBF kernel provided robust accuracy by capturing complex relationships within the data.
Continuous improvement through parameter tuning and feature extraction techniques.
How to Use
Run the Notebook:

Ensure all dependencies are installed (e.g., numpy, pandas, scikit-learn, tensorflow, keras).
Execute the notebook cells sequentially to preprocess data, apply SMOTE, transform data, train models, and evaluate results.
Upload Your Data:

To test with unseen data, upload your train and test data files.
Update the file paths in the relevant cells of the notebook.
Conclusion
This project demonstrates the effectiveness of time series classification techniques in diagnosing cardiac conditions from ECG signals. The application of advanced feature extraction methods and machine learning algorithms resulted in high classification accuracy, contributing to better diagnostic tools in healthcare.

