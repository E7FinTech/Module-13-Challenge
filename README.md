# Module 13 Challenge

![alt text](13-challenge-image.png)

## Background
You work as a risk management associate at Alphabet Soup, a fictitious venture capital firm. The Alphabet Soup business team receives many funding applications from startups every day. This team has asked you to help them create a model that predicts whether applicants will become successful if funded by Alphabet Soup.

The team has given you a CSV file containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. This file contains various types of information about the organizations, including whether they ultimately became successful. With your knowledge of machine learning and neural networks, you decide to use the features in the provided dataset to create a binary classifier model that will predict whether an applicant will become successful.

## What You're Creating
To predict whether Alphabet Soup funding applicants will be successful, you will create a binary classification model using a deep neural network.

This challenge consists of three technical deliverables. You will do the following:

* Preprocess data for a neural network model.

* Use the model-fit-predict pattern to compile and evaluate a binary classification model.

* Optimize the model.

## Files
Download the following files to help you get started:
Module 13 Challenge files

## Instructions
The instructions for this Challenge are divided into the following subsections:

1. Prepare the Data for Use on a Neural Network Model

2. Compile and Evaluate a Binary Classification Model Using a Neural Network

3. Optimize the Neural Network Model

## Prepare the Data for Use on a Neural Network Model
Using your knowledge of Pandas and `StandardScaler` from scikit-learn, preprocess the dataset so that you can later use it to compile and evaluate the neural network model. To do so, complete the following steps:

1. Read the `applicants_data.csv` file into a Pandas DataFrame. Review the DataFrame, checking for categorical variables that will need to be encoded and for columns that might eventually define your features and target variables.

2. Drop the “EIN” (Employer Identification Number) and “NAME” columns from the DataFrame, because they’re irrelevant for the binary classification model.

3. Encode the categorical variables of the dataset by using `OneHotEncoder`, and then place the encoded variables in a new DataFrame.

4. Add the numerical variables of the original DataFrame to the DataFrame that contains the encoded variables

**NOTE**
To complete this step, use the Pandas `concat` function.

5. Using the preprocessed data, create the features (`X`) and target (`y`) datasets. The “IS_SUCCESSFUL” column in the preprocessed DataFrame should define the target dataset. The remaining columns should define the features dataset.

6. Split the features and target datasets into training and testing datasets.

7. Use `StandardScaler` from scikit-learn to scale the features data.

## Compile and Evaluate a Binary Classification Model Using a Neural Network
Use your knowledge of TensorFlow to design a binary classification deep neural network model. This model should use the features of the dataset to predict whether a startup that’s funded by Alphabet Soup will become successful. Consider the number of inputs before determining both the number of layers that your model will contain and the number of neurons on each layer. Then compile and fit your model. Finally, evaluate your binary classification model to calculate the model’s loss and accuracy.

1. To do so, complete the following steps:

Use Tensorflow’s Keras to create a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer.

**HINT**
You can start with a two-layer deep neural network model that uses the `relu` activation function for both layers.

2. Compile and fit the model by using the `binary_crossentropy` loss function, the `adam` optimizer, and the `accuracy` evaluation metric.

**HINT**
When fitting the model, start with a small number of epochs, such as 20, 50, or 100.

3. Evaluate the model by using the test data to determine the model’s loss and accuracy.

4. Save and export your model to an HDF5 file, and name the file `AlphabetSoup.h5`.

## Optimize the Neural Network Model
Using your knowledge of TensorFlow and Keras, optimize your model to improve its accuracy. Even if you don’t achieve a better accuracy, you'll need to demonstrate at least two attempts to optimize the model. You can include these attempts in your existing notebook. Or, you can make copies of the starter notebook in the same folder, rename them, and code each model optimization in a new notebook.

**NOTE**
You won’t lose points if your model doesn’t achieve a high accuracy—as long as you make at least two attempts to optimize the model.

To do so, complete the following steps:

1. Define at least three new deep neural network models (that is, the original plus two optimization attempts). For each, try to improve your first model’s predictive accuracy.

**REWIND**
Recall that perfect accuracy has a value of 1, so accuracy improves as its value moves closer to 1. To optimize your model for a predictive accuracy that’s as close as possible to 1, you can use any or all of the following techniques:

    * Adjust the input data by dropping different features columns to ensure that no variables or outliers confuse the model.

    * Add more neurons (nodes) to a hidden layer.

    * Add more hidden layers.

    * Use different activation functions for the hidden layers.

    * Increase or reduce the number of epochs in the training regimen.

2. Display the accuracy scores that each model achieved, and then compare the results.

3. Save each model as an HDF5 file.

## Requirements
## Prepare the Data for Use on a Neural Network Model (20 points)
# To receive all points, you must

* Read the data into a DataFrame and drop the columns that are not relevant. (5 points)

* Encode the categorical variables using `OneHotEncoder`, and place the encoded variables in a new DataFrame. (5 points)

* Create the features (`X`) and target (`y`) datasets, and split them into training and testing datasets. (5 points)

Use scikit-learn's `StandardScaler` to scale the features data. (5 points)

## Compile and Evaluate a Binary Classification Model Using a Neural Network (25 points)
# To receive all points, you must

* Create a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer using Tensorflow’s Keras. (5 points)

* Compile and fit the neural network model using the `binary_crossentropy` loss function, the `adam` optimizer, and the `accuracy` evaluation metric. (5 points)

* Evaluate the model using the test data to determine the model’s loss and accuracy. (10 points)

* Save and export the model to an HDF5 file, and name the file `AlphabetSoup.h5`. (5 points)

## Optimize the Neural Network Model (25 points)
# To receive all points, you must

* Define at least two deep neural network models (the original model, plus two optimisation attempts). Try to improve on your first model’s predictive accuracy. (10 points)

* Display the accuracy scores achieved by each model, and compare the results. (10 points)

* Save each model as an HDF5 file. (5 points)

**NOTE**
You will not lose points if your model does not achieve high accuracy, as long as you make at least two attempts to optimize the model.

## Coding Conventions and Formatting (10 points)
# To receive all points, you must

* Place imports at the top of the file, just after any module comments and docstrings, and before module globals and constants. (3 points)

* Name functions and variables with lowercase characters, with words separated by underscores. (2 points)

* Follow DRY (Don't Repeat Yourself) principles, creating maintainable and reusable code. (3 points)

* Use concise logic and creative engineering where possible. (2 points)

## Deployment and Submission (10 points)
# To receive all points, you must

* Submit a link to a GitHub repository that’s cloned to your local machine and contains your files. (5 points)

* Include appropriate commit messages in your files. (5 points)

## Code Comments (10 points)
# To receive all points, your code must

* Be well commented with concise, relevant notes that other developers can understand. (10 points)

## Submission
To submit your Challenge assignment, click Submit, and then provide the URL of your GitHub repository for grading.

**NOTE:**
You are allowed to miss up to two Challenge assignments and still earn your certificate. If you complete all Challenge assignments, your lowest two grades will be dropped. If you wish to skip this assignment, click Next, and move on to the next module.

Comments are disabled for graded submissions in Bootcamp Spot. If you have questions about your feedback, please notify your instructional staff or your Student Success Manager. If you would like to resubmit your work for an additional review, you can use the Resubmit Assignment button to upload new links. You may resubmit up to three times for a total of four submissions.
