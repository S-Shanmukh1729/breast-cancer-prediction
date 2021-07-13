# breast-cancer-prediction
Breast Cancer Predection(Malignant or Benign) Using Logistic Regression

![image](https://user-images.githubusercontent.com/80630137/125470078-299e97d1-d5c1-47e2-a05b-0fb57f6d2a17.png)


In this project we are going to Predict whether the cancer is benign or malignant using slearn's Logistic Regression with python.We will download the dataset from kaggle. To train a logistic regression model, we can use the LogisticRegression class from Scikit-learn. We will try to cover following tasks in this project:


Downloading a real-world dataset from Kaggle

Exploratory data analysis and visualization

Splitting a dataset into training, validation & test sets

Scaling numeric features to a (0,1) range

Training a logistic regression model using Scikit-learn

Evaluating a model using a validation set and test set

Saving a model to disk and loading it back


We are going to download Breast cancer Diagnosis data set from kaggle using opendatasets module of python, and load the csv data into pandas dataframe.

Pandas is a popular Python library used for working in tabular data (similar to the data stored in a spreadsheet). Pandas provides helper functions to read data from various file formats like CSV, Excel spreadsheets, HTML tables, JSON, SQL, and more.

Features are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. They describe characteristics of the cell nuclei present in the image. n the 3-dimensional space is that described in: [K. P. Bennett and O. L. Mangasarian: "Robust Linear Programming Discrimination of Two Linearly Inseparable Sets", Optimization Methods and Software 1, 1992, 23-34].

This database is also available through the UW CS ftp server: ftp ftp.cs.wisc.edu cd math-prog/cpo-dataset/machine-learn/WDBC/

Also can be found on UCI Machine Learning Repository: https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29

Attribute Information:

1) ID number

2) Diagnosis (M = malignant, B = benign)

3-32)

Ten real-valued features are computed for each cell nucleus:

a) radius (mean of distances from center to points on the perimeter)

b) texture (standard deviation of gray-scale values)

c) perimeter

d) area

e) smoothness (local variation in radius lengths)

f) compactness (perimeter^2 / area - 1.0)

g) concavity (severity of concave portions of the contour)

h) concave points (number of concave portions of the contour)

i) symmetry

j) fractal dimension ("coastline approximation" - 1)

The mean, standard error and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features. For instance, field 3 is Mean Radius, field 13 is Radius SE, field 23 is Worst Radius.

All feature values are recoded with four significant digits.

Missing attribute values: none

Class distribution: 357 benign, 212 malignant



### Logistic Regression:

Logistic regression is a commonly used technique for solving binary classification problems. In a logistic regression model:

1.we take linear combination (or weighted sum of the input features)
2.we apply the sigmoid function to the result to obtain a number between 0 and 1
3.this number represents the probability of the input being classified as "Yes"
4.instead of RMSE, the cross entropy loss function is used to evaluate the results

Here's a visual summary of how a logistic regression model is structured :
![image](https://user-images.githubusercontent.com/80630137/125470007-00ab2514-ad52-4aa2-94bf-93ad7feee7e6.png)
