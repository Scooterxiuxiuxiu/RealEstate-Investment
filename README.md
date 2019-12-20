# RealEstate-Investment
#### Project 7 for EECS

Data for project is Beijing' housing price for Beijing. Dataset was uploaded into the same repository. <br>
In this project, I explored the general shape of the data and correlations btw features. <br>
To get more information, I built several models to get the geometirc distribution, regression prediction and time trend. <br>

All results were showed in plots:<br>


  * Feature Distribution in histogram

  * Feature correlations in heatmap

  * Pairplots for house with different number of bathroom
    
  * Geometric distribution drawed by average housing price at points with different longitude and latitude
    >The average housing price in beijing shows a clear increasing pattern from suburban area to city center, 
     which matches the city transportation loop regulation for the city.
  
  * Distribution in administrative district given by K-means clustering
    >Using the geographic information, the result shows that, 
    K-means clusters the data into clusters that are fairly close to the actual subregions of each city, 
    using K=13 for Beijing,  where 13 is the number of adminstrative districts in Beijing. 

  * Comparation btw Linear regression prediction and real data for average price
    >The original data sets were divided into training and testing data set with the ratio of 70% and 30%. 
    
  * Showing housing price time trend
      > Using weekly average to reduce effect from uneven distribution in time
      > Taking first 300 data as training data
    
   * MA model 
     > set window width=3
     > prediction shows a flat trend with no increasing in price in the future

   * ARIMA(7,1,2) model
     > Taking first and second differencing to detrend and get stationary data:
       Second differenciated data shows no big difference in trend with first differenciated data.
       So weekly total price data could be considered as stationary after first differenciating. 
     > Ploting acf and pacf to find ordes for auto regression and moving average
     
   * Seasonal ARIMA model
     > set period as 4 weeks / a month
     
   * Prophet Time Series Forecasting
     
   


More details and discussion could be found in code comments.
