# COVID19
 Analysis on COVID-19 pandemic
updated on March 29, 2020  

# Predictions on growth of confirmed Novel Coronavirus (2019-nCoV) cases in countries   
## Goal: Make an educated guess on when the spread of the novel coronavirus will stabilize (i.e. when the things will get better) in different countries

For detailed numbers chec: Predictions_on_growth_of_confirmed_cases.ipynb
  
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
### 1. The logistic model was applied to 59 countries
### 2. Mean turning point for these countries is on 2020-03-24 (This is an understimate because only countries close to turning points can be modeled)
### 3. Mean CurveTop for these countries is on 2020-04-21
### 4. The numbers of confirmed cases in US, Spain,	Italy, United Kingdom, Germany, France may exceed those in China
### 5. Comparing to last week, more countries can be modeled by logistic model, indicating that an increase in number of confirmed cases globally and more countries are getting closer to turning points
### 6. By looking at CruveTop and comparing from last week, Gemany reduced future confirmed cases by half. On the other hand, Italy, Spain, and France need to enforce containment measures because the total confirmed cases in the future are predicted to be increasing.