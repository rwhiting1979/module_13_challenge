# Alphabet Soup Venture Capital Project
## Background
Alphabet Soup Venture Capital is a firm that receives many funding applications from startups daily. The business team wants to create a model that predicts whether an applicant will be successful if funded by the company. They have provided a CSV file containing information about more than 34,000 organizations that have received funding from Alphabet Soup in the past, including whether they ultimately became successful.

## Objective
To predict whether Alphabet Soup funding applicants will be successful, we will create a binary classification model using a deep neural network.

## Technical Deliverables
The project consists of three technical deliverables:

1. Prepare the Data for Use on a Neural Network Model: preprocess the dataset so that it can be used to compile and evaluate the neural network model.

2. Compile and Evaluate a Binary Classification Model Using a Neural Network: design a binary classification deep neural network model that uses the features of the dataset to predict whether a startup that's funded by Alphabet Soup will become successful.

3. Optimize the Neural Network Model: optimize the model to improve its accuracy.

## Instructions
## Prepare the Data for Use on a Neural Network Model

1. Read the applicants_data.csv file into a Pandas DataFrame. Review the DataFrame, checking for categorical variables that will need to be encoded and for columns that might eventually define your features and target variables.

2. Drop the "EIN" (Employer Identification Number) and "NAME" columns from the DataFrame since they are irrelevant for the binary classification model.

3. Encode the categorical variables of the dataset by using OneHotEncoder and place the encoded variables in a new DataFrame.

4. Add the numerical variables of the original DataFrame to the DataFrame that contains the encoded variables.

5. Create the features (X) and target (y) datasets using the preprocessed data. The "IS_SUCCESSFUL" column in the preprocessed DataFrame should define the target dataset. The remaining columns should define the features dataset.

6. Split the features and target datasets into training and testing datasets.

7. Scale the features data using StandardScaler from scikit-learn.

## Compile and Evaluate a Binary Classification Model Using a Neural Network
1. Use TensorFlow's Keras to create a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer.

2. Compile and fit the model using the binary_crossentropy loss function, the adam optimizer, and the accuracy evaluation metric. Start with a small number of epochs, such as 20, 50, or 100.

3. Evaluate the model using the test data to determine the model's loss and accuracy.

4. Save and export the model to an HDF5 file named "AlphabetSoup.h5".

## Optimize the Neural Network Model
1. Define at least three new deep neural network models (the original plus two optimization attempts) and try to improve the first model's predictive accuracy.

2. Display the accuracy scores that each model achieved and compare the results.

3. Save each model as an HDF5 file.