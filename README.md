Linear Regression.
This repository contains Python code for implementing Linear Regression with Ridge and Lasso regularization. The dataset used for this demonstration is the Housing dataset, and the code is written using the pandas, numpy, and scikit-learn libraries.

Introduction
Linear regression is a fundamental machine learning algorithm used for predicting a continuous outcome variable based on one or more predictor variables. Regularization techniques, such as Ridge and Lasso, are applied to linear regression to prevent overfitting and improve model generalization.

Dataset
The dataset used is the Housing dataset, loaded from the "Housing.csv" file.

Features
area: Area of the property
bedrooms: Number of bedrooms
bathrooms: Number of bathrooms
stories: Number of stories
mainroad: Presence of a main road (1 for yes, 0 for no)
guestroom: Presence of a guest room (1 for yes, 0 for no)
basement: Presence of a basement (1 for yes, 0 for no)
hotwaterheating: Presence of hot water heating (1 for yes, 0 for no)
airconditioning: Presence of air conditioning (1 for yes, 0 for no)
parking: Number of parking spaces
prefarea: Preferred area (1 for yes, 0 for no)
furnishingstatus: Furnishing status (1 for furnished, 0 for semi-furnished, 2 for unfurnished)

Target Variable
price: Price of the property

Preprocessing
The categorical variables (mainroad, guestroom, basement, hotwaterheating, airconditioning, prefarea, furnishingstatus) are encoded using one-hot encoding. The furnishingstatus is encoded as follows: 1 for furnished, 0 for semi-furnished, and 2 for unfurnished.

Model Training
The dataset is split into training and testing sets using the train_test_split function from scikit-learn. A linear regression model is trained using the training data.
The model achieves an R-squared score of approximately 0.678.

Ridge Regression
The Ridge regression model achieves an R-squared score of approximately 0.678.

Lasso Regression
The Lasso regression model achieves an R-squared score of approximately 0.678.

Prediction
Predictions are made on the test data using each of the trained models.

New Prediction
A new set of features is provided to make predictions for a new property.

The predicted price for the new property using linear regression is approximately 7,841,608.83.

Conclusion
This repository demonstrates the implementation of linear regression and its regularized versions, Ridge and Lasso, for predicting property prices based on various features. The models are evaluated using R-squared scores, and predictions are made for both test data and new data.
