# Project-Retail-sales-prediction
I dealt with the past data of Europe Drug stores in this project and the dataset name was "Rossmann Store"


Sales forecasting plays an integral role in setting expectations and making plans for your business. It’s your best shot at predicting the future. Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. You are provided with historical sales data for 1,115 Rossmann stores. The task is to forecast the "Sales" column for the test set.

I performed an exhaustive analysis in order to gain insights and engineer features with an interactive exploratory analysis and finally will use different algorithms to predict.

<img src = "https://user-images.githubusercontent.com/83903018/124346442-78365400-dbfc-11eb-8311-2b8689315b38.png">


## Columns in the dataframe:
1. Id - an Id that represents a Store within the test set
2. Store - a unique Id for each store
3. Sales - the turnover for any given day (this is what you are predicting)
4. Open - an indicator for whether the store was open: 0 = closed, 1 = open
5. StateHoliday - indicates a state holiday. a = public holiday, b = Easter holiday, c = Christmas, 0 = None
6. SchoolHoliday - indicates if the Store on a particular Date was affected by the closure of public schools
7. StoreType - differentiates between 4 different store models: a, b, c, d
8. Assortment - describes an assortment level: a = basic, b = extra, c = extended
9. CompetitionDistance - distance in meters to the nearest competitor store
10. CompetitionOpenSince[Month/Year] - gives the approximate year and month of the time the nearest competitor was opened
11. Promo - indicates whether a store is running a promo on that day
12. Promo2 - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating
13. Promo2Since[Year/Week] - describes the year and calendar week when the store started participating in Promo2
14. PromoInterval - describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store

## After Exploratory data Analysis, I used different Regression algorithms for training the model


- There were 4 different type of stores among which 54% stores were of type – "a" which was maximum, and the least was type – "b"

- There were 1115 different stores among which 38% stores were running promo and 62% are not

- we can say maximum sales by store type “b”, but also the number of store with type “b” is minimum so we should consider type “a”

- From 212 stores, store number - 158, 277, 370, 612, 637, 808, 960 had run the promo for maximum number of months i.e. 71 months

- Store number 815 had a competition from year 1900, so more than 100 years

- We made these PromoOpen negative values to zeros, because they have not started the promos at that time

- Decision tree was the best for this dataset problem among algorithms which I have used

