# Automobile Price Prediction Model
## Machine Learning Price Prediction Model 

**Author: Thomas Greenacre**: 

### Business problem:

To create a model that accurately predicts the Price of automobiles based on historical data and machine learning techniques


### Data:
Source: [https://www.kaggle.com/datasets/deepcontractor/car-price-prediction-challenge


Descitpion: the data set has the price (target) along with various features (manufacturer, model, drive type, mileage, etc.) of different automobiles


## Methods (Evaluate & Clean)
- removed (if needed) duplicate rows
- deleted unnessecary features (columns) from the dataset that dont impact the target (price)
- checked & address any missing data
- identified and corrected inconsistencies in values of categorical features
- identified and removed outliers (price > 43,000 and mileage > 350,000)
- built in nomininal encoded mean values for missing data on features with numeric (int, float) data type
- OneHot encoded the most frequent values for missing data on features with object data type

## Exploration and Analysis

#### Feature Correlation Heatmap
> this visual shows the correlation between all of the features (numeric and categorical) in the data set

![image](https://user-images.githubusercontent.com/104700955/181682758-86655876-cae2-49a4-864e-90a1d707bde3.png)


#### Car Prices by Manufacturer
> this visual shows the price of automobiles by manufactured (lexus, toyota, audi, etc.). Its helpful to see the volume (number of instances/automobiles) and to get a sense of the price scale/distribution (MIN, MAX, and AVG) visually for each manufacturer

![image](https://user-images.githubusercontent.com/104700955/181682552-f5c61fe1-e0d0-42f9-81f8-209635d7f3fa.png)

## ML Modeling
> 3 different base ML models were built and evaluated with PCA and no PCA 
  - Model #1: Linear Regression
  - Model #2: Random Forest
  - Model #3: Decision Tree 



## Reccomendations
 - Reccomediation #1: Given that none of the 3 models (Linear Regression, Random Forest, Decision Tree) yielded great results with or without PCA, I would reccomend to try and improve model results first before implementing

 - Reccomediation #2: If you were to implement 1 of the 3 models despite the lack of great results, reccomendation would be to implement "Model 2 (Random Forest) w/out PCA" because out of all the models tested, this one scored the best across all evaluation metrics.

Evaluation Metrics: Model 2 w/out PCA had a prediction score of 0.9128 on the training data but only a 0.4136 prediction score on the test data.

## Limitations & Next Steps

### For further information


For any additional questions, please contact **thomas.greenacre@gmail.com**

-----------------------------
## Results


## Model
 Pr
The final model(s) tested to predict the Sales (Item_Outlet_Sales) are 1 Linear Regression model and 1 Decision Tree model.

The most important metric is the R-Squared (R2) which was used to evaulate how well the models would accurately predict Sales (Item_Outlet_Sales)

Additinal metric used to evaluate the models was the Root Mean Squared Error (RMSE)

## Recommendations:

Based on the R2 scores used to evaluate both models (see below); the Decision Tree Model should be impletemented

Linear Regression R2 Scores
*   Train: 0.560543
*   Test: 0.565847

Decisions Tree R2 Scores
*   Train: 0.603925
*   Test: 0.594747


## Limitations & Next Steps

Both models coulds be improved with more data and/or features. Next step to improve the data set used and re-run prediction models to improve overal R2 scores.


### For further information


For any additional questions, please contact **thomas.greenacre@gmail.com**
