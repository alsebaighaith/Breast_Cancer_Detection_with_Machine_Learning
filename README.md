# Breast_Cancer_Detection_with_Machine_Learning
This project exemplifies the potential of machine learning in improving early breast cancer diagnosis and highlights the importance of selecting an appropriate algorithm for the specific task at hand.
Breast Cancer Detection with Machine Learning

Breast cancer is a significant health concern worldwide, and early detection plays a crucial role in improving patient outcomes. Machine learning techniques have shown promise in assisting medical professionals in the early diagnosis of breast cancer. 

## Data Acquisition
The project began by obtaining a substantial dataset from scikit-learn, which contains a multitude of features but a relatively small number of samples. This presented a challenge due to the risk of overfitting with limited data. Therefore, careful data analysis and preprocessing were essential.

## Data Preprocessing
To make the dataset suitable for training, several preprocessing steps were performed

## Split Data
Data Splitting: The data was split into training and testing sets using the train_test_split function. This allowed for the evaluation of the model's performance on unseen data.

## Model Training - SGDClassifier
The initial model trained for breast cancer detection was the Stochastic Gradient Descent (SGD) Classifier. This classifier was chosen as a starting point due to its efficiency . After training, the model was evaluated using various metrics, including the confusion matrix, precision score, and recall score.

## Evaluation
One of the primary concerns in this project was to minimize false negatives, as missing the diagnosis of malignant tumors could have severe consequences. Therefore, the project primarily focused on achieving a high recall score, indicating the model's ability to correctly identify malignant cases.

The initial SGDClassifier yielded a recall score of approximately 0.9721, indicating excellent performance in detecting malignant tumors.

## Model Training - GaussianNB
To explore different algorithms, the project continued with the Gaussian Naive Bayes (GaussianNB) classifier. Surprisingly, this model did not make any incorrect predictions, leading to concerns about overfitting. The model's perfect performance on the test data raised suspicions of potential issues related to sampling bias and the dataset's limited size and high dimensionality.

## Model Training - Logistic Regression
In search of a more balanced and reliable model, Logistic Regression was introduced. This model demonstrated exceptional performance, with a recall score of approximately 0.9930, making only two errors when evaluated on the test data. This result suggested that Logistic Regression was well-suited for the breast cancer detection task, striking a balance between precision and recall.
