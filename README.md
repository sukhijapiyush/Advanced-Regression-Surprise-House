# Advanced Regression(Regularization) on Surprise House Dataset

> This project uses regularization( L1 aned L2) on Surprise House Dataset and compare the both and provide the variables are significant in predicting the price of a house, and How well those variables describe the price of a house.

## Table of Contents

- [Advanced Regression(Regularization) on Surprise House Dataset](#advanced-regressionregularization-on-surprise-house-dataset)
  - [Table of Contents](#table-of-contents)
  - [General Information](#general-information)
    - [Business Problem](#business-problem)
    - [Goal of the Project](#goal-of-the-project)
  - [Business Requiremnt](#business-requiremnt)
    - [Steps involved](#steps-involved)
  - [Result](#result)
  - [Conclusion](#conclusion)
  - [Technologies Used](#technologies-used)
  - [Acknowledgements](#acknowledgements)
  - [Contact](#contact)
  - [License](#license)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

### Business Problem

A US-based housing company named _Surprise Housing_ has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia.
The company is looking at prospective properties to buy to enter the market. You are
required to build a regression model using regularisation in order to
predict the actual value of the prospective properties and decide whether to invest in them or not.
The company wants to know:
**Target** : Which variables are significant in predicting the price of a house, and How well those variables describe the price of a house.s.

### Goal of the Project

Build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest.
Determine the optimal value of lambda for ridge and lasso regression.
This model will then be used by the management to understand how exactly the prices vary with the variables

## Business Requiremnt

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

### Steps involved

- Data Load and Analysis
- Data Wragling
- Exploratory Data Analysis
- Splitting the dataset
- Scaling of the variables(RobustScaler)
- Modelling
- Tuning with Regularization (Ridge & Lasso)
- Model Evaluation

## Result

We achieved the following results:

- Ridge

  - Test Accuracy : 0.867015
  - Mean Absolute Error : 0.090746
  - Durbin-Watson value : 1.9778
  - Lamda : 0.00079901

- Lasso
  - Test Accuracy : 0.894023
  - Mean Absolute Error : 0.072316
  - Durbin-Watson value : 1.9778
  - Lamda : 0.00058701

## Conclusion

As it can be observed the Lasso performed better than Ridge and has higher accuracy on test (89>86) with less MSE.
Both models are valid as they follows the assumptions of the linear regresion and for final conclusion we will use Lasso as it has feature selection which will help reducing the variable making model easier to understand.

## Technologies Used

- Pandas - version 1.3.4
- NumPy - version 1.20.3
- MatplotLib - version 3.4.3
- Seaborn - version 0.11.2
- Scikit-Learn - version 0.24.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

This project was inspired by UpGrad IITB Programme as a case study for the Machine Learning and Artificial Intelligence course.

## Contact

Created by [@sukhijapiyush] - feel free to contact me!

<!-- Optional -->

## License

This project is open source and available without restrictions.

<!-- You don't have to include all sections - just the one's relevant to your project -->
