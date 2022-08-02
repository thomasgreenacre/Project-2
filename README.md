# Automobile Price Prediction Model
## Machine Learning Price Prediction Model 

**Author: Thomas Greenacre**: 

### Business problem:

To create a model that accurately predicts the price of automobiles based on historical data and machine learning techniques


### Data:
Source: https://www.kaggle.com/datasets/deepcontractor/car-price-prediction-challenge


Description: the data set has the price (target) along with various features (manufacturer, model, drive type, mileage, etc.) of different automobiles


## Methods (Evaluate & Clean)
- removed (if needed) duplicate rows
- deleted unnecessary features (columns) from the dataset that do not impact the target (price)
- checked & address any missing data
- identified and corrected inconsistencies in values of categorical features
- identified and removed outliers (price > 43,000 and mileage > 350,000)
- built in nominal encoded mean values for missing data on features with numeric (int, float) data type
- OneHot encoded the most frequent values for missing data on features with object data type

## Exploration and Analysis

#### Feature Correlation Heatmap
> This visual shows the correlation between all of the features (numeric and categorical) in the data set

![image](https://user-images.githubusercontent.com/104700955/181682758-86655876-cae2-49a4-864e-90a1d707bde3.png)


#### Car Prices by Manufacturer
> This visual shows the price of automobiles by manufacturer (Lexus, Toyota, Audi, etc.). Its helpful to see the volume (number of instances/automobiles) and to get a sense of the price scale/distribution (MIN, MAX, and AVG) visually for each manufacturer

![image](https://user-images.githubusercontent.com/104700955/181682552-f5c61fe1-e0d0-42f9-81f8-209635d7f3fa.png)

## ML Modeling
> 3 different base ML models were built and evaluated with PCA and no PCA 
  - Model #1: Linear Regression
  - Model #2: Random Forest
  - Model #3: Decision Tree 

  - Evaluation Metrics (best performing model): Model 2 w/out PCA had a prediction score of 0.9128 on the training data but only a 0.4136 prediction score on the test data
    >-  MAE Train: 2167.55
    >-  MAE Test: 5733.19

    >-  MSE Train: 9272681.74
    >-  MSE Test: 62966247.39

    >-  RMSE Train: 3045.10
    >-  RMSE Test: 7935.12

## Recommendations

 - Recommendation #1: Given that none of the 3 models (Linear Regression, Random Forest, Decision Tree) yielded great results with or without PCA, I would recommend to try and improve model results first before implementing

 - Recommendation #2: If you were to implement 1 of the 3 models despite the lack of great results, recommendation would be to implement "Model 2 (Random Forest) w/out PCA" because out of all the models tested, this one scored the best across all evaluation metrics

### For further information


For any additional questions, please contact **thomas.greenacre@gmail.com**

