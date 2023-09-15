# Crucial Sales Predictions

## Analyzing various stores to increase sales

Author: Loraine Rodriguez

___
## **Business Problem**

It is often  a challenge for companies to know where to focus resources and efforts. THere are many possibilites and it can be overwhelming to narrow down.       to know where to aim is to build models that will predict items sold at various stores. The goal of this is to help Big Mart Sales understand the products and outlets that play crucial roles in increasing sales.

## **Data**

Big Mart Sales Prediction: 
https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/
___

## **Methods**
With the data provided, we were able to create various different machine learning models. 

## **Models Created**
- Linear Regression
- Default Random Forest
- Tuned Random Forest
___

## **Linear Regression Metrics: Training Data**

MAE = 847.652

MSE = 1,298,672.978

RMSE = 1,139.593

R^2 = 0.561

## **Linear Regression Metrics: Test Data**

MAE = 810.395

MSE = 1,210,343.986

RMSE = 1,100.156

R^2 = 0.568
___

## **Default Random Forest Model: Training Data**

MAE = 296.621

MSE = 182,983.213

RMSE = 427.765

R^2 = 0.938

## **Default Random Forest Model: Testing Data**

MAE = 779.032

MSE = 1,252,109.443

RMSE = 1,118.977

R^2 = 0.553

____

## **Tuned Random Forest Model: Training Data**

MAE = 610.715

MSE = 754,716.507

RMSE = 868.744

R^2 = 0.745

## **Tuned Random Forest Model: Testing Data**

MAE = 760.789

MSE = 1,165,741.719

RMSE = 1,1079.695

R^2 = 0.584

Based off of these different models, I would recommend using the tuned Random Forest model which performed better than both the Linear Regression and default Random Forest model on MAE, MSE, RMSE, and R^2 for the testing data.

The Default model outperformed the Tuned model in the training data but fell short on the data that mattered, the test data.

Despite the Linear Regression model and Default Random Forest model having large differences in the training data, they both performed fairly similar on the test data.

The R^2 metric is probably the most important metric. It shows that the model can explain a specific % of the data.
The Tuned Random Forest model can explain for 59% of the test data.

## Explanatory Visuals

## Visual #1
![Frequency Of Item Type](https://github.com/lrnrdr/Prediction-of-Product-Sales/assets/138408700/98c91427-e395-4a8b-922e-831d2b8edcea)

- From this graph, we can see that the Item_Type "Fruits and Vegetables" has the highest frequency sold, followed by the "Snack Foods" and "Household Goods" which are the next highest, as they are both around 14% . 

  
## Visual #2

![Heatmap Of Data](https://github.com/lrnrdr/Prediction-of-Product-Sales/assets/138408700/2c7c1948-1817-4792-8052-984c7d9662cd)


- Here on the this heatmap, you can see that the Item Outlet Sales and Item MRP have the strongest correlation. 

## Visual #3
![image](https://github.com/lrnrdr/Prediction-of-Product-Sales/assets/138408700/2cb597ef-79c1-4bd2-8473-8f6c9ea8e50f)

The image above shows the top 10 most important features. Top 5 features are Item MRP, Outlet Type - Grocery Store, Item Visibility, Item Weight, and Outlet Type - Supermarket 3. These five were the most helpful in growing/sorting the tree-based model.

## Visual #4

![image](https://github.com/lrnrdr/Prediction-of-Product-Sales/assets/138408700/4ceb0f0d-606a-4d62-ba1e-b151fa6c2e78)

3 coefficients are Outlet Location Type Tier 2, Outlet Identifier - OUT049, and Outlet Location Type - Tier 3. Sales from these locations positively influence the target (Item Outlet Sales)

## **Recommendations**

The top three selling product types are Fruits & Vegetables, Snack Foods, and Household Goods, we need to make sure that the  outlets focus on this products when stocking up. 

The Item MRP is the strongest contrubuter to Item Outlet Sale, so attention to Item MRP is cruicial. 
