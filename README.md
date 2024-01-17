# SVM_Model
This Python script focuses on building and evaluating Support Vector Machine (SVM) models with different kernels for predicting insurance charges. 
Here's a breakdown of the code:

Data Loading and Preprocessing:
Loads the insurance dataset from a CSV file.
Utilizes one-hot encoding for categorical variables ('sex', 'smoker', 'region').
Standardizes numerical features ('age', 'bmi', 'children') using StandardScaler.

Data Splitting:
Splits the data into training and validation sets without randomization, allocating 20% for validation.

SVM Model Definition and Hyperparameter Tuning:
Defines three SVM models with different kernels: Linear, Polynomial, and RBF.
Performs hyperparameter tuning using GridSearchCV for each model to optimize model performance.

Model Training and Prediction:
Trains each SVM model with the best hyperparameters on the training set.
Makes predictions on the validation set for each model.

Model Evaluation:
Evaluates model performance using Mean Squared Error (MSE) and R-squared metrics for each kernel.
Prints the MSE and R-squared values for the Linear, Polynomial, and RBF kernels.

Results Presentation:
Creates a DataFrame to store predictions for all models.
Saves the predictions, along with an index column, to a CSV file named 'validation_predictions.csv'.

The script provides a comprehensive analysis of SVM models with different kernels, offering insights into their performance on predicting insurance charges. The evaluation metrics (MSE and R-squared) help assess the accuracy and goodness of fit for each SVM kernel.
