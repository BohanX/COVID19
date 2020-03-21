# COVID19
 Analysis on COVID-19 pandemic

# Predictions on growth of confirmed Novel Coronavirus (2019-nCoV) cases in countries   
## Goal: Make an educated guess on when the spread of the novel coronavirus will stabilize (i.e. when the things will get better) in different countries
  
## Method:   
1. Use the data from China as an example to create logistic models for different countries   
2. Use R^2 to evaluate goodness of fit
3. Use inflection point to predict the turning point (i.e. when the number of newly confirmed cases per day will start to decrease
4. Use 99.9% of the top horizontal asymptote value to predict when the situation wil stablize (i.e. the number of newly confirmed cases is closed to zero)
  
## Data:   
Publically available source from 2019 Novel Coronavirus COVID-19 (2019-nCoV) Data Repository by Johns Hopkins CSSE    
https://github.com/CSSEGISandData/COVID-19/blob/master/csse_covid_19_data/csse_covid_19_time_series/time_series_19-covid-Confirmed.csv  

## Disclaimer:   
### 1. The model assumes that everything stays constant, so the conclusions will be affected both positively and negatively by dramatic changes such as new travel restictions, shortage of health care supplies, ect  
### 2. Only confirmed cases were included, so the result depends number of tests done and it does not necessarily reflect the actual infected population in each countries  
### 3. Any inaccuracies in the data source can affect predictions  
### 4. I intend to update every week and conclusion may be different in each update (due to new models being generated from latest data)  

## Summary:   
### 1. The logistic model was applied to 26 countries  
### 2. Mean turning point for these countries is on 2020-03-16  
### 3. Mean CurveTop for these countries is on 2020-04-08  
### 4. The numbers of confirmed cases in Germany and Italy may exceed those in China, but there are uncertainties because the numbers in China is expected to rise again due to people going back to China from other countries.  
