# House Price Prediction Using Linear Regression

## Project Overview

This project focuses on building and evaluating a Machine Learning model to predict house prices using **Linear Regression**.

The project uses the cleaned and preprocessed house-price dataset prepared in the previous exercise. The dataset was divided into training and testing sets, a Linear Regression model was trained, and the trained model was used to predict house prices for unseen test data.

The model was evaluated using multiple regression performance metrics to understand its prediction accuracy and overall performance.

## Project Objectives

The main objectives of this project were to:

- Use a cleaned and preprocessed dataset for Machine Learning.
- Split the dataset into training and testing sets.
- Train a Linear Regression model.
- Predict house prices using unseen test data.
- Evaluate model performance using regression metrics.
- Interpret the results and identify possible areas for improvement.

## Project Workflow

 
Preprocessed House-Price Dataset
                ↓
                
Feature and Target Selection
                ↓
                
Train-Test Split
                ↓
                
Linear Regression Model Training
                ↓
                
House-Price Prediction
                ↓
                
Model Evaluation
                ↓
                
Performance Interpretation
                  ↓
                  
Preprocessed House-Price Dataset
                ↓
                
Feature and Target Selection
                ↓
                
Train-Test Split
                ↓
                
Linear Regression Model Training
                ↓
                
House-Price Prediction
                ↓
                
Model Evaluation
                ↓
                
Performance Interpretation

## Dataset

Dataset: **HousePricePrediction.csv**

The dataset contains house-related features used to develop a Machine Learning model for predicting house prices.

The dataset was cleaned and preprocessed during the previous exercise before being used for model development.

### Tasks Completed

#### 1. Train-Test Split

The dataset was divided into two parts:

Training Data — Used to train the Machine Learning model.
Testing Data — Used to evaluate the model on unseen data.

An appropriate training and testing ratio was used to support model development and evaluation.

#### 2. Linear Regression Model Training

A Linear Regression model was created and trained using the training dataset.

The model learned the relationship between the selected house features and the target house-price variable.

#### 3. House-Price Prediction

After training, the model was used to generate house-price predictions using the test dataset.

The predicted values were compared with the actual house-price values to assess model performance.

#### 4. Model Evaluation

The model was evaluated using the following regression metrics:

Mean Absolute Error (MAE)

MAE measures the average absolute difference between the actual and predicted house prices.

A lower MAE generally indicates that the predictions are closer to the actual values.

Mean Squared Error (MSE)

MSE calculates the average of the squared differences between actual and predicted values.

Larger prediction errors have a greater effect because the errors are squared.

Root Mean Squared Error (RMSE)

RMSE is the square root of MSE.

It provides an error value in the same unit as the target variable and helps show the typical size of prediction errors.

R² Score

The R² Score measures how well the model explains variation in the target variable.

A higher R² Score generally indicates that the model explains more of the variation in house prices.

#### 5. Model Performance Interpretation

The evaluation results were analyzed to determine whether the Linear Regression model produced satisfactory predictions or required further improvement.

The model performance was interpreted by reviewing:

- Prediction errors
- The relationship between predicted and actual values
- The R² Score
- Possible limitations of the model
- Tools and Technologies
- Python
- Google Colab
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- Machine Learning Concepts Demonstrated
- Supervised Machine Learning
- Regression
- Feature selection
- Target-variable selection
- Train-test splitting
- Linear Regression
- Model training
- Model prediction
- Model evaluation
- Regression performance metrics
- Skills Demonstrated
- Data preparation
- Machine Learning workflow development
- Training and testing data preparation
- Regression modeling
- House-price prediction
- Model evaluation
- Performance analysis
- Results interpretation

## Project Files

03_House_Price_Prediction/

├── README.md

├── house_price_prediction.ipynb

└── house_price_prediction.pdf

#### File Descriptions

Jupyter Notebook (.ipynb)

## The Jupyter Notebook contains:

Python code

Dataset preparation

Train-test splitting

Linear Regression model development

Model training

House-price predictions

Model evaluation

Performance results

PDF (.pdf)

## The PDF contains:

- The completed exercise documentation
- Screenshots of the Python code
- Screenshots of the model outputs
- Evidence of the completed Machine Learning tasks
- 
  ### Project Outcomes:

Through this project, I developed practical experience in:

- Preparing data for Machine Learning.
- Splitting a dataset into training and testing sets.
- Building a Linear Regression model.
- Training a Machine Learning model.
- Generating predictions using unseen test data.
- Evaluating regression models using MAE, MSE, RMSE, and R² Score.
- Interpreting Machine Learning model performance.
- Connection to Previous and Future Projects

#### This project is connected to the previous data-preprocessing exercise:

**Exercise 2:**

Data Preprocessing with Pandas
                ↓
**Exercise 3:**

House Price Prediction Using Linear Regression

The preprocessing work completed in Exercise 2 provides the structured dataset used for model development in this project.

The next exercise moves from traditional Machine Learning to Deep Learning:

Linear Regression
        ↓
        
Deep Learning
        ↓
        
Convolutional Neural Networks
        ↓
        
Fashion-MNIST Image Classification

### Future Improvements:

Possible improvements include:

Testing additional regression algorithms.

Comparing Linear Regression with Decision Tree Regression.

Testing Random Forest Regression.

Improving feature selection.

Applying feature engineering.

Performing hyperparameter tuning.

Using cross-validation.

Visualizing predicted values against actual values.

Building an interactive house-price prediction application.

By

Bakht Zamin

AI Automation & Prompt Engineering | Data Analytics & Business Intelligence | Python | Machine Learning
