# CustChurn

EDA
Prediction using both Regression and Classification

<img width="474" alt="Screenshot 2022-07-18 at 02 33 41" src="https://user-images.githubusercontent.com/100385953/179431211-5f38f17b-946f-4899-9b70-b135697f3b28.png">


Churn could occur due to many different reasons, and customer churn analysis helps to identify the cause and timing of this churn leading to implement effective churn retention strategies.
Here are eight steps of data science life cycle to make sure wise data-driven decisions have been made to fight against the customer churn:
1- Understand the business model, requirements, and risks.
2- Collect available customer behavior, transactions, demographics data, and usage patterns.
3- Formulate initial hypotheses based on domain knowledge and exploratory analysis that will assist in defining metrics to tackle these hypotheses.
4- Do the required data processing to have a cleaned dataset suitable as an input to a machine learning model.
5- Utilize these data points to create a model that predicts customer segments who are likely to churn.
6- Assess the results to ensure that the model satisfies the original business goals.
7- Report the results to the stakeholders.
8- Deploy the model into a production system.

Customer retention should be a top priority of any business as acquiring new customers is often far more expensive that keeping existing ones. It is no longer a given that long standing customers will remain loyal given the numerous options in the market. Therefore, it is vital that companies can proactively determine the customers most at risk of leaving and take preventative measures against this.

Predictive models for customer churn can show the overall rate of attrition, while knowledge of how the churn rate varies over a period of time, customer cohort, product lines and other changes can provide numerous valuable insights. Yet, customers also vary enormously in their behaviors and preferences which means that applying a simple “rule of thumb” analysis will not work. Here’s where a predictive model using gradient boosting can help you.

How accurately can we predict customer churn with gradient boosting?

Gradient boosting has various internal parameters know generically as hyper-parameters. These settings determine the size of the underlying trees and the impact that each round of boosting has on the overall model. It can be time consuming to explore all of the possibilities to find the best values. To create the model below I automatically performed a grid search of 36 different combinations of hyper-parameters. I selected the best set by 5-fold cross validation.

Why choose gradient boosting over other models?

In the same way that I just fitted a gradient boosting model, we can fit other models. I tried 3 other approaches. Each time I followed the same procedure as above, selecting the same variables, fitting with the training sample and calculating accuracy from the testing sample. The results are:

Model	Accuracy
Gradient Boosted Tree	80.87%
CART	79.21%
Random Forest	79.94%
Linear Discriminant Analysis	79.97%
Whilst this is not a comprehensive comparison, gradient boosting performs the best amongst these models with the highest accuracy score.
