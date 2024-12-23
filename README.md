# ZOO Animal Classifier

## Overview
This project is designed to classify different animals based on various features such as habitat, physical characteristics, and behaviors. The goal is to build a machine learning model using the Random Forest classifier to predict the animal type from a set of predefined features.

## Dataset
The dataset contains 101 rows and 17 columns, with each row representing an animal. The features include information about the animal's habitat, physical traits, and behavior.

### Features
- `name`: Name of the animal
- `hair`: Indicates if the animal has hair (1 for yes, 0 for no)
- `features`: Various other binary features describing the animal
- `eggs`: Whether the animal lays eggs
- `milk`: Whether the animal produces milk
- `airborne`: Whether the animal can fly
- `aquatic`: Whether the animal lives in water
- `predator`: Whether the animal is a predator
- `toothed`: Whether the animal has teeth
- `backbone`: Whether the animal has a backbone
- `breathes`: Whether the animal breathes air
- `venomous`: Whether the animal is venomous
- `fins`: Whether the animal has fins
- `legs`: Number of legs the animal has
- `tail`: Whether the animal has a tail
- `domestic`: Whether the animal is domestic
- `catsize`: Size of the animal (small, medium, large)
- `type`: The animal type (e.g., mammal, bird, fish, etc.)

## Usage

### 1. Load the Dataset
The dataset is loaded and preprocessed using pandas.

### 2. Data Preprocessing
The dataset is cleaned by filling missing values and performing feature encoding. The target variable (`type`) is separated from the features.

### 3. Model Training
A Random Forest classifier is used to train the model on the preprocessed data. Cross-validation is performed to evaluate the model's performance.

### 4. Model Evaluation
The model is evaluated using various metrics such as accuracy, precision, recall, and F1-score. The model is also tested using cross-validation for a more robust evaluation.

### 5. Model Predictions
The trained model is used to predict the animal type based on new input data.

## Cross-validation
The model uses cross-validation to assess its performance. The dataset is split into multiple folds, and the model is trained on each fold to provide a more reliable accuracy score.

## Results
The model achieves high accuracy in classifying animals based on the features. The cross-validation scores demonstrate a stable and consistent performance across different splits of the dataset.
