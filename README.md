# COVID19
A Canada-first breakdown and analysis of the COVID19 pandemic. The data are from John-Hopkins University CSSE 

https://github.com/CSSEGISandData/COVID-19

# Canada

![](Canada_exp_2020-03-23.png)
*Figure 1*: Per-province, logy growth of reported infected cases. Reference growth rates expressed as days to double are shown. Cases are shown as days since the, at least 5th reported case. 

![](Canada_2020-03-23.png)
*Figure 2*: Time series of logy growth of reported infected cases. Black line is Canada. Per province sums shown on the right, although some overplotting of the values may occure when the values are close together.

![](Cad_deaths2020-03-23.png)
*Figure 3*: Per-province, time series of logy death counts. Black line is Canada. Per province sums shown on the right, although some overplotting of the values may occure when the values are close together.

# Global
A subset of global countries are included so-as to ensure clear communication of data. 

These are currently: Canada, France, Italy, Spain, UK, US

![](World_exp_2020-03-23.png)
*Figure 4*: Global logy growth  of reported infected cases. Reference growth rates expressed as days to double are shown. Cases are shown as days since the, at least 100th reported case. 

![](World_deaths_since10th_2020-03-23.png)
*Figure 5*: Global time series of logy death counts. Per province sums shown on the right, although some overplotting of the values may occure when the values are close together.

# Global change in rate of growth

As countries' growth rates slow and hasten, the rate of change of these rates can be useful for quanitfying if the situation is getting better or worse.

This below figure shows a 7-day moving window calculation of the growth rate of covid19 cases, expressed as days to double.

Specifically, a linear fit to `log(value)`  is calculated using a 7-day moving window. The slope of this line is expressed as a doubling rate via `log(2)/log(slope)`. This is then plotted with time. It's essentially the change in time of a moving window first derivative. The moving window approach is used to help filter out some of the noise in data, e.g., when there is no reporting over weekends, etc.

![](World_movingwindow_growth2020-03-23)
*Figure 6*: 7-day moving window rate of change of growth for select countries. Greater doubling rates implies a slow down.









