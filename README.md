<b>Breast Cancer Prediction using Support Vector Machine (SVM)</b>


<b>Overview</b>
Breast cancer is one of the most common cancers among women worldwide. Early detection and diagnosis are crucial for effective treatment and improved survival rates. This project aims to develop a predictive model using a Support Vector Machine (SVM) classifier to distinguish between malignant and benign breast tumors based on the Breast Cancer Wisconsin (Diagnostic) dataset.



<b>Theoretical Background</b>
<b>Support Vector Machine (SVM)</b>:
Support Vector Machine (SVM) is a supervised machine learning algorithm widely used for classification tasks. The primary objective of SVM is to find the optimal hyperplane that best separates the data into different classes. Key concepts include:



<b>Hyperplane:</b> A decision boundary that separates the data points of different classes.
<b>Support Vectors:</b> Data points that are closest to the hyperplane and influence its position and orientation.
<b>Margin</b>: The distance between the hyperplane and the nearest data points from either class. SVM aims to maximize this margin.
<b>Kernel Trick:</b>
SVM can perform linear and non-linear classification. For non-linear classification, SVM uses the kernel trick to transform the input space into a higher-dimensional space where a linear separator can be found. Commonly used kernels include:

Linear
Polynomial
Radial Basis Function (RBF)
Sigmoid
<b>Breast Cancer_Dataset</b>
<b>Dataset Description</b>
The dataset used in this project is the Breast Cancer Wisconsin (Diagnostic) dataset. It contains 569 instances of breast cancer data, each with 30 numeric features and one target label indicating the diagnosis (M = malignant, B = benign).

<b>Data Structure</b>
<br>Number of Instances: 569
Number of Features: 30 numeric features
Target Variable: Diagnosis (M = malignant, B = benign)
Features
The dataset includes the following features:

id: ID number
diagnosis: Diagnosis (M = malignant, B = benign)
radius_mean: Mean radius of the tumor
texture_mean: Mean texture of the tumor
perimeter_mean: Mean perimeter of the tumor
area_mean: Mean area of the tumor
smoothness_mean: Mean smoothness of the tumor
compactness_mean: Mean compactness of the tumor
concavity_mean: Mean concavity of the tumor
concave points_mean: Mean number of concave points of the tumor
symmetry_mean: Mean symmetry of the tumor
fractal_dimension_mean: Mean fractal dimension of the tumor
radius_se: Standard error of the radius
texture_se: Standard error of the texture
perimeter_se: Standard error of the perimeter
area_se: Standard error of the area
smoothness_se: Standard error of the smoothness
compactness_se: Standard error of the compactness
concavity_se: Standard error of the concavity
concave points_se: Standard error of the concave points
symmetry_se: Standard error of the symmetry
fractal_dimension_se: Standard error of the fractal dimension
radius_worst: Worst (largest) radius
texture_worst: Worst texture
perimeter_worst: Worst perimeter
area_worst: Worst area
smoothness_worst: Worst smoothness
compactness_worst: Worst compactness
concavity_worst: Worst concavity
concave points_worst: Worst number of concave points
symmetry_worst: Worst symmetry
fractal_dimension_worst: Worst fractal dimension
Data Sample
Here are the first few rows of the dataset:

id	diagnosis	radius_mean	texture_mean	...	fractal_dimension_worst
842302	M	17.99	10.38	...	0.11890
842517	M	20.57	17.77	...	0.08902
84300903	M	19.69	21.25	...	0.08758
84348301	M	11.42	20.38	...	0.17300
84358402	M	20.29	14.34	...	0.07678
Data Preprocessing
Before training the model, the following preprocessing steps are performed:

Dropping the ID column: The ID column is not useful for prediction.
Encoding the target variable: Convert the diagnosis labels (M, B) to numeric values (1, 0).
Standardizing features: Standardize the features to have zero mean and unit variance.




<b>Project Workflow<b>
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
