# Final Project - Coffee Quality

![photo](http://coffeequalitylaboratory.com/wp-content/uploads/2017/11/unnamed.jpg)


## Background & Objectiv
I am a great coffee fan and asked myself wheter its is possible to predict the quality of coffee by some gives parameters. So I found a dataset from the Coffee Quality Institute. There I wanted to try oiut different regressors and answer the question whether it is possible or not. For the modeling part I used Python and the column "cupper points" as the target. The visualization part is mostly Tableau.


## Dataset 
In this project, I used the provided [** Coffee Quality**](https://www.kaggle.com/volpatto/coffee-quality-database-from-cqi) dataset from kaggle.

**Data**: The data set consists of information on 1339 different coffees which the Coffee Quality Insitute tested and presented January 2018. Existing Colunmns are f.e.:
**Quality Measures**
- Aroma
- Flavor
- Aftertaste
- Acidity
- Body
- Balance
- Uniformity
- Cup Cleanliness
- Sweetness
- Moisture
- Defects

**Bean Metadata**

- Processing Method
- Color
- Species (arabica / robusta)

**Farm Metadata**

- Owner
- Country of Origin
- Farm Name
- Lot Number
- Mill
- Company
- Altitude
- Region


## Workflow
After importing all nesessary libraries and loading the data from SQL, I did some data exploration. After I get a feel for it, I did some data cleaning: droping duplicates (there were none), renaming the columns, droping unesessary columns, dealing with null values, reducing to many unique values in a column, changing outliers in numerical columns etc.
After tranforming the numericals with StandardScaler and Normalizer, I tried diffrent regressors:
- Linear Regression
- Decision Trees Regressor
- KNN Regressor
- Random Forest Regressor
Therefore I used the whole dataset (categorical & numerical) and only numericals (standard scaled/ normalized).

The last step was clustering the data and visulization in Tableau.

## Conclusion
The transformed data with the StandardScaler perfomed way better than the normalizes data.
The best Regressor was the Random Forest Regressor with the only numerical dataset. But the R2 Score is still only 0,6829. So you can't fully predict the quality of a coffee.
