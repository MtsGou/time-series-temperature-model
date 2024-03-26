# TIME SERIES ANALYSIS AND FORECAST MODELS - WORLD AND BRAZIL

**Data science repository with files and codes used to analyze temperatures in Brazil and in the world overall, since 1750. Also created models to predict temperatures in a near future.**

----

## Methods

Data was collected from Kaggle's [dataset](https://www.kaggle.com/datasets/berkeleyearth/climate-change-earth-surface-temperature-data) "Climate Change: Earth Surface Temperature Data". Used two tables from this dataset: _'GlobalLandTemperaturesByCountry'_ and _'GlobalTemperatures'_.

Some packages and APIs were used: [Pandas](https://pandas.pydata.org/), [Matplotlib](https://matplotlib.org/), [Numpy](https://numpy.org/), [Scikit-Learn](https://scikit-learn.org/stable/), [Statsmodels Time Series Analysis](https://www.statsmodels.org/stable/tsa.html), [PyPI Pmdarima](https://pypi.org/project/pmdarima/) and also [SciPy](https://scipy.org/).

**Models used:**

 - [XG Boost Regressor](https://xgboost.readthedocs.io/en/stable/python/index.html);
 - [Pmdarima Auto ARIMA](https://alkaline-ml.com/pmdarima/modules/generated/pmdarima.arima.auto_arima.html);
 - [Statsmodels SARIMA/SARIMAX](https://www.statsmodels.org/stable/examples/notebooks/generated/statespace_sarimax_stata.html).

**Metrics and analysis:**

 - [sklearn.metrics.mean_absolute_error](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_absolute_error.html);
 - [statsmodels.tools.eval_measures.rmse](https://www.statsmodels.org/dev/generated/statsmodels.tools.eval_measures.rmse.html)
 - [statsmodels Seasonal decomposition](https://www.statsmodels.org/dev/generated/statsmodels.tsa.seasonal.seasonal_decompose.html);
 - [adfuller test (ADF) - statsmodels.tsa.stattools.adfuller](https://www.statsmodels.org/dev/generated/statsmodels.tsa.stattools.adfuller.html).

-----

## Average temperature along the years

### Brazil

![Temperaturas](/plots/average_temp_br.png)

- Applying moving average (range 10)

![Temperaturas MA](/plots/average_temp_br_MA.png)

### World

![Temperaturas world](/plots/average_temp_world.png)

- Applying moving average (range 10)

![Temperaturas world MA](/plots/average_temp_world_MA.png)

----

## Forecast temperatures in Brazil

### ARIMA model

![ARIMA](/plots/ARIMA_br.png)

### SARIMA model

![SARIMA](/plots/SARIMA_br.png)

![SARIMA Forecast](/plots/SARIMA_br_forecast.png)

## Forecast temperatures worldwide

### XG Boost Regressor (month ahead)

![XG Boost](/plots/XGBoost_world.png)

### SARIMAX Model

![SARIMAX](/plots/SARIMAX_world.png)


**[`🔼         back to top        `](#time-series-analysis-and-forecast-models---world-and-brazil)**

