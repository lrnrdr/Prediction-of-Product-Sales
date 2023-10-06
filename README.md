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
___

## **Models Created & Metrics**
- Linear Regression
- Default Random Forest
- Tuned Random Forest

![image](https://github.com/lrnrdr/Prediction-of-Product-Sales/assets/138408700/e98dc26b-8a62-49bd-b4c5-056a4fded23c)

___



Based off of these different models, I would recommend using the tuned Random Forest model which performed better than both the Linear Regression and default Random Forest model on MAE, MSE, RMSE, and R^2 for the testing data.


The (test_R2) metric in the models is probably the most important metric. It shows that the model can explain a specific % of the data.
The Tuned Random Forest model can explain for 59% of the test data which means the others explain less of the variations in the target.

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
