# Automobile Price Prediction Model
## Machine Learning Price Prediction Model 

**Author: Thomas Greenacre**: 

### Business problem:

To create a model that accurately predicts the Price of automobiles based on historical data and machine learning techniques


### Data:
Source: https://www.kaggle.com/datasets/deepcontractor/car-price-prediction-challenge![image](https://user-images.githubusercontent.com/104700955/181681325-dfedeab3-5a6e-4bd3-9bab-aa7ef950ef8d.png)


Descitpion: the data set has the price (target) along with various features (manufacturer, model, drive type, mileage, etc.) of different automobiles


## Methods (Evaluate & Clean)
- check & remove (if needed) duplicate rows
- delete any unnessecary features (columns) from the dataset that dont impact the target (price)
- Checking & address any missing data
- identified and corrected inconsistencies in values of categorical features
- identified outliers and removed (price > 43,000 and mileage > 350,000)
- though not needed I built in nomininal encoded mean values for missing data on features with numeric (int, float) data type
- OneHot encoded the most frequent values for missing data on features with object data type

## Exploration and Analysis

#### Feature Correlation Heatmap
> this visual shows the correlation between all of the features (numeric and categorical) in the data set

![image](https://user-images.githubusercontent.com/104700955/181682758-86655876-cae2-49a4-864e-90a1d707bde3.png)


#### Car Prices by Manufacturer
> this visual shows the price of automobiles by manufactured (lexus, toyota, audi, etc.). Its helpful to see the volume (number of instances/automobiles) and to get a sense of the price scale/distribution (MIN, MAX, and AVG) visually for each manufacturer

![image](https://user-images.githubusercontent.com/104700955/181682552-f5c61fe1-e0d0-42f9-81f8-209635d7f3fa.png)

## ML Modeling




## Reccomendations


## Limitations & Next Steps

### For further information


For any additional questions, please contact **thomas.greenacre@gmail.com**

-----------------------------
## Results

#### Feature Correlation Heatmap

![image](https://user-images.githubusercontent.com/104700955/176902787-08c2a6eb-a7b2-472b-8fd1-f377b33a294d.png)

> this visual shows the relationship (correlation) between the different features in the dataset

#### Item MRP Box Plot

![image](https://user-images.githubusercontent.com/104700955/176902544-9e3ea546-06c6-4185-8a5e-e69b741bd91b.png)

this visual shows the range of values for the Item MRP feature represented by a Box Plot

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
