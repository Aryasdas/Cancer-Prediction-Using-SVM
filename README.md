*Breast Cancer Prediction using Support Vector Machine (SVM)*.
<b>Overview<b>
<br>Breast cancer is one of the most common cancers among women worldwide. Early detection and diagnosis are crucial for effective treatment and improved survival rates. This project aims to develop a predictive model using a Support Vector Machine (SVM) classifier to distinguish between malignant and benign breast tumors based on the Breast Cancer Wisconsin (Diagnostic) dataset.<br>

Theoretical Background
Support Vector Machine (SVM)
Support Vector Machine (SVM) is a supervised machine learning algorithm widely used for classification tasks. The primary objective of SVM is to find the optimal hyperplane that best separates the data into different classes. Key concepts include:

Hyperplane: A decision boundary that separates the data points of different classes.
Support Vectors: Data points that are closest to the hyperplane and influence its position and orientation.
Margin: The distance between the hyperplane and the nearest data points from either class. SVM aims to maximize this margin.
Kernel Trick
SVM can perform linear and non-linear classification. For non-linear classification, SVM uses the kernel trick to transform the input space into a higher-dimensional space where a linear separator can be found. Commonly used kernels include:

Linear
Polynomial
Radial Basis Function (RBF)
Sigmoid
Breast Cancer Wisconsin (Diagnostic) Dataset
The Breast Cancer Wisconsin (Diagnostic) dataset contains 569 samples of breast tumors, each described by 30 numerical features. The features are computed from digitized images of fine needle aspirate (FNA) of breast masses. Each sample is labeled as malignant (M) or benign (B).

Project Workflow
1. Data Preprocessing
Loading Data: Read the dataset from a CSV file.
Data Cleaning: Remove unnecessary columns (e.g., ID).
Encoding Labels: Convert categorical labels (M, B) into numerical labels (1, 0).
Feature Scaling: Standardize features to have zero mean and unit variance.
2. Model Training
Split Data: Divide the dataset into training and testing sets.
Train Model: Train the SVM classifier on the training set using a linear kernel.
3. Model Evaluation
Predictions: Use the trained model to make predictions on the testing set.
Performance Metrics: Evaluate the model using classification metrics such as accuracy, precision, recall, F1-score, and confusion matrix.
4. Visualization (Optional)
Decision Boundary: Visualize the decision boundary for a subset of features (only for 2D visualization).
