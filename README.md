# Project-Retail-sales-prediction
I dealt with the past data of Europe Drug stores in this project and the dataset name was "Rossmann Store"


Sales forecasting plays an integral role in setting expectations and making plans for your business. It’s your best shot at predicting the future. Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. You are provided with historical sales data for 1,115 Rossmann stores. The task is to forecast the "Sales" column for the test set.

I performed an exhaustive analysis in order to gain insights and engineer features with an interactive exploratory analysis and finally will use different algorithms to predict.


## After Exploratory data Analysis, I used different Regression algorithms for training the model


There were 4 different type of stores among which 54% stores were of type – "a" which was maximum, and the least was type – "b"

There were 1115 different stores among which 38% stores were running promo and 62% are not

we can say maximum sales by store type “b”, but also the number of store with type “b” is minimum so we should consider type “a”

 From 212 stores, store number - 158, 277, 370, 612, 637, 808, 960 had run the promo for maximum number of months i.e. 71 months

 Store number 815 had a competition from year 1900, so more than 100 years

 We made these PromoOpen negative values to zeros, because they have not started the promos at that time

 Decision tree was the best for this dataset problem among algorithms which I have used

