BOOMBIKES SHARING CASE STUDY:USING MULTIPLE REGRESSION MODEL

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.we are using multiple linear regression model to predict a high demand for bikes.Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 
The company aims to know:
1.which variables are significant in predicting the demand of shared bikes 
2.how those variables exaplin well on bike demand.


## Table of Contents
* [General Info](#general-information)
* [Methods used](#methods-used)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information

- Analysis:boombikes has recently suffered considerible dips in their revenue during covid 19 so we are using multiple linear regression so that we can build a model with a best fit line which will help managment achieve the needs of customers and get a huge demand in american market.
- Bussiness problem:During corona there was a significant decrease in bike sharing.the goal of the company is to solve the problem and find independent features which  might help in rising the demand and later they can accordingly manipulate the demand levels and meet customer needs and expectation which will help them grow.
Bussiness goal:identify the factors or variables leading to this loss in american market.
- Dataset:past bike-sharing data during pandemic(COVID-19) of Boombikes dataset(day.csv)

## Methods used:
-Reading and understanding the Data:
    1.importing neccesary libraries.
    2.checking for Null values.
    3.Dropping unnecessry columns.
    4.visualizing numerical and categorical variables.
    5.using heatmap to check correlation between variables.
    6.univariate analysis using barplot and scatterplot.
-Data Preparation:
    1.creating dummy variables.
    2.splitting into train and test data.
    3.rescaling of variables using min-max scaler.
-Training the Model:
    using RFE-recursive feature elimination.
-Building the Model:
    1.fit tranform the training dataset.
    2.calculate VIF-variance inflation factor.
    3.find out the best fit linear model.
-Residual analysis:
    calculate the error distribution it should be Normal.
-Prediction and evaluation on Test Data:
    Transform the test data and evaluate using R^2 and Adjusted R^2 values with bestfit linear Model.


## Conclusions
1.the top 3 feautures which contribute to the explaination of bike sharing
    -year:+ve correlation
    -spring:-ve correlation
    -light_rain:-ve correlation
  it is highly recommended to use these variables for planning.
2.year 2019 has more demand for bikes when compared to year 2018.
3.Bike rentals are more suring the fall and summer.
4.sep month has a huge demand for bikes.
5.the demand increases in the case of variables : year,july,sep,aug.
6.the demand decreases for variables :holiday,soring,light_rain,jan,nov,dec.
7.The best fit line after building a model is :
   -count = 0.246 x year - 0.073 x holiday - 0.221 x spring - 0.290 x light_rain - 0.112 x jan + 0.053 x july - 0.077 x nov + 0.100 x sep + 0.066 x aug - 0.084 x dec
8.Model evaluation results:
  1.Train data
       -R^2 value:0.739
       -Adjusted R^2 value:0.734
  2.Test data
       -R^2 value:0.754
       -Adjusted R^2:0.720


## Technologies Used
- pandas - version 1.4.2
- numpy - version 1.21.5
- seaborn - version 0.11.2
- matplotlib - version 3.5.1
- plotly - version 5.6.0
- statsmodels - version 0.14.0
- sklearn - version 1.0.2.
- scipy - version 1.7.3



## Acknowledgements
Greatful to upgrad for giving a chance to work on this project.


## Contact
Created by [@tejaswini1968] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->