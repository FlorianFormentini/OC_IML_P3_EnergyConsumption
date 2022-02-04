# OpenClassrooms IML - Project 3 : Electricity Consumption and CO2 emissions of Buildings

The city of Seattle aims to be a carbon neutral city by 2050. To achieve this, the project team needs to study the emissions from non-housing buildings.
Careful surveys have already been done, but they are expensive to obtain.

My task as a data scientist was to try to predict the energy consumption and C02 emissions of buildings for which this has not been measured.

There is also a tedious piece of data to obtain, the EnergyStar score, the importance of which should be evaluated for predictions in order to know whether it can be excluded or not


## Data
The available data are the commercial permits for the years 2015 and 2016. Files containing column metadata are also provided.

## Evaluation Metrics
Two metrics were used to evaluate and compare several models:
$${\displaystyle R^{2}=1-{\dfrac {\sum _{i=1}^{n}\left(y_{i}-{\hat {y_{i}}}\right)^{2}}{\sum _{i=1}^{n}\left(y_{i}-{\bar {y}}\right)^{2}}}}$$
$$ RMSE = \sqrt{\frac{1}{n}\Sigma_{i=1}^{n}{\Big(\frac{y_i -\hat{y}_i}{\sigma_i}\Big)^2}}$$

## Results
The selected and optimised model is **XGBoost Regressor**.  
And with this model, the EnergyStar score is necessary to make predictions.
<p align="center"><img width="400" height="300" src="Pelec_05_charts\scores.png"></p>
<p align="center"><img width="600" height="300" src="Pelec_05_charts\co2_preds.png"></p>
<p align="center"><img width="600" height="300" src="Pelec_05_charts\energy_preds.png"></p>
<p align="center"><img width="400" height="300" src="Pelec_05_charts\buildingTypeScores.png"></p>

