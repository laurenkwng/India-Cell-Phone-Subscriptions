# A Time Series Analysis of India's Cell Phone Subscriptions

The purpose of this class project was to accurately forecast the number of mobile cellular phone subscriptions
in India, based on previous rates. This is of interest in relation to the recent and massive incorporation of a
digital identity system named Aadhaar. Aadhaar is a 12-digit unique identity number that can be obtained
by residents of India, based on their biometric and demographic data. In our analysis of the time-series,
we used various techniques, including Box-Cox transformations and differencing to make the time series
stationary and thus allowing us to identify potential models by looking at ACF and PACF plots.

During analysis, we developed many candidate models, however, only one of our candidates was most suitable for forecasting: ARIMA(1,1,2) model. The ARIMA(1,1,2) model passed the Box-Ljung and Shapiro-Wilk tests, is viable for forecasting, and best satisfies the principle of parsimony, compared to our other candidates. Through forecasting we were able to plot a potential trajectory with 95% confidence for four years in the future. Despite certain validation points being outside the confidence interval, our forecasted values still remain valid.

## 5 Year Forecast Accuracy
<img width="674" alt="Screen Shot 2019-07-07 at 6 03 06 PM" src="https://user-images.githubusercontent.com/30671201/60776480-815dba80-a0e1-11e9-936f-7da91e5d4426.png">


### Built With
R Studio 

### Methodology
* Time Series Plots
* ACF and PACF Plots
* Box Cox Transformations
* Difference Plots
* ARMA/ARIMA Modeling
* Box-Ljung Tests
* Box-Pierce Tests
* Shapiro-Wilk Normality Tests
* Analyzing Roots
* Forecasting

### Conclusions
Though not all of our validation points are within the 95% CI, the majority of them are and, furthermore,
the validation points converge towards our predictions as time goes on. Looking at the original time series,
we can see how this might be possible. The period that we are validating exhibits atypical behavior compared
to the rest of the graph. There are unusual amounts of growth and then a slight dip. However, with time, we
can see that our predictions are indeed valid and accurate, as our prediction for year 20 and our validation point are nearly the same. 

In conclusion, we believe that cellphone usage is a good indicator of Aadhaar’s
success, and by modeling the growth in usage, we would expect to see similar rates of growth in Aadhaar
and financial inclusion. Furthermore, we have accomplished our goal of understanding what future rates of
cellphone subscriptions/usage might look like in India, arriving at our final model of ARIMA(1,1,2).

### Contributors
* Lauren Wong
* Jeremy Berkov
* Maximilian Broekhuis
* Winson Li
* Crystal Chau
