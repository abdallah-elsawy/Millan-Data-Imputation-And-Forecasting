<h1>Millan Data Imputation And Forecasting</h1>

<h2> Dataset</h2>

The dataset reports lines in the format above for 10,000 areas (organized in a regular grid) during a continued period of two months.
A preliminary description of the data is provided in a paper published in Scientific Data by Barlacchi et al. [Link](https://www.nature.com/articles/sdata201555). While the paper presents the many datasets that were made available for the other challenges, only two are relevant to the above mentioned tasks:

<h2>The objective of this project is:</h2>
  <h3>1) Gathering and preprocessing the <a href="https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/EGZHFV">Telecommunications Millan Data</a></h3><br>
    <ul>
      <li> Read the txt-file as csv.
      <li> Group the data by time and grid.
      <li> Concatenate all the data in one DataFrame.
      <li> Convert the full data into a numpy array, where each sample is a (100, 100) matrix.
        <ul>
          <li> Each sample is a matrix which is the measurements for all grids at a specific time step.
          <li> Each value in the matrix is a measurement for one grid at a this time step.
        </ul>
    </ul>
  <h3>2) Applying many missing data imputation methods to the data</h3><br>
  <ul>
    <li> Missing data imputation methodes :
      <ul>
      <li> Conventional methods:
        <ul>
          <li> Ignore or deletion.
          <li> Mean imputaion.
          <li> Mode imputaion.
          <li> Median imputaion.
        </ul>
      <li> Imputation procedure:
        <ul>
          <li> Last valid observation forward.
          <li> Next valid observation forward.
          <li> Interpolation.
        </ul>
      <li> Learnable methods:
        <ul>
          <li> KNN algorithm.
          <li> AutoRegressive.
          <li> Genitic algorithm.
          <li> MICE algorithm.
          <li> Least square SVM.
          <li> GAIN.
          <li> Conv-GAIN.
        </ul>
      </ul>
    </ul>
  <h2>3) Time series Forecasting: </h2><br>
    <li> Statistical methods:
      <ul>
        <li> Common Approaches:
          <ul>
          <li>Trend, Seasonal, Residual Decompositions:
          <li> Seasonal Extraction in ARIMA Time Series (SEATS).
          <li> Seasonal and Trend decomposition using Loess (STL). 
          <li> Exponential smoothing:
            <ul>
              <li> Single Exponential Smoothing, or SES, for univariate data without trend or seasonality.
              <li> Double Exponential Smoothing for univariate data with support for trends.
              <li> Triple Exponential Smoothing, or Holt-Winters Exponential Smoothing, with support for both trends and seasonality.(TES)
            </ul>
          <li> Autoregressive Models (AR).
          <li> Moving Average Models (MA).
          </ul>
      <li> Box–Jenkins Approaches: 
        <ul>
          <li> ARIMA.
          <li> SARIMA.
        </ul>
    </ul>
    <li> Machine Learning Methods
      <ul>
        <li> KNN.
        <li> SVR.
        <li> Linear Regression.
        <li> ElasticNet.
        <li> Lasso.
      </ul>
    <li> Deep Learning Methods:
      <ul>
        <li> MLP.
        <li> CNN.
        <li> LSTM.
      </ul>
      </ul>
