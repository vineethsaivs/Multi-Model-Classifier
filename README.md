# Multi-Model-Classifier
Automating model selection for classification problems in Machine Learning by comparing performance metrics across multiple models.

This project demonstrates the use of multiple machine learning models to classify the Iris dataset. The Iris dataset is a multiclass classification problem where the task is to predict one of three classes of iris plants.

## Models Used

The following models are used in this project:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Classifier
- K-Nearest Neighbors Classifier
- Gaussian Naive Bayes
- Gradient Boosting Classifier
- Multi-Layer Perceptron Classifier

## Workflow

1. The Iris dataset is loaded and split into a training set and a test set.
2. The features are standardized using `StandardScaler`.
3. Each model is trained on the training set and evaluated on the test set.
4. The performance of each model is evaluated using the following metrics: accuracy, precision, recall, and F1 score. The results are stored in a DataFrame and displayed in a bar plot.
5. For the first model (Logistic Regression in this case), a confusion matrix, ROC curves for each class, a precision-recall curve for class 1, and a feature importance plot (if the model supports it) are generated.

## Results

The results include a table of performance metrics for each model and several plots. The plots include a bar plot of model accuracy, a heatmap of the confusion matrix, ROC curves for each class, a precision-recall curve for class 1, and a feature importance plot (for models that support it).

## Usage

To run the project, simply execute the Python script `multi_model_classifier.ipynb`. The script requires the following Python packages: pandas, sklearn, matplotlib, seaborn.

## Note

The precision-recall curve does not directly support multiclass problems. In this project, we choose class 1 as positive and the rest as negative for demonstration. You may need to adjust this based on your specific problem.
