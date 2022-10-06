# Project Name
> Bike Sharing Analysis and Prediction

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- Bike Sharing counts prediction using linear regression algorithm. Finding significant features which effects bike sharing counts.
- FHow bike shared numbers are getting affected on external and environment factors.
- Finding best features with which we can maximise bike rentals numbers and and detect parameters to reduce business loss in slack season.
- Dataset used:
    a. day.csv: dataset available for model development.
    b. Readme.txt: information about columns.
    c. Sajal Tiwari.ipynb: Main Notebook.
    d. Subjective Questions - Asnwers.pdf: Answers to questiones asked.

### Dataset Characteristics
- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered

## Conclusions
- Features affecting bike rental numbers: 'yr_19', 'workingday', 'spring', 'winter', 'light_fall', 'mist', '03_mar', '04_apr', '05_may', '06_jun', '08_aug', '09_sep', '10_oct', '6_Sat', 'temp', 'hum', 'windspeed'
- Most significant features:
    * temp: temperature : 0.434234
    * light_fall : light fall weather situation : -0.254504
    * yr_19 : year 2019 : 0.232232
- R2 score with test dataset is 0.868
- Mean Squared error with test dataset is 0.00594.


## Technologies Used
- statsmodels : version 0.13.2
- matplotlib : version 3.5.1
- pandas : version 1.4.2
- numpy : version 1.21.5
- seaborn : version 0.11.2
- sklearn : version 1.0.2

## Acknowledgements
- This project was based on [upgrad](https://www.upgrad.com)
 - dataset source:
Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}
	
For further information about this dataset please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt).


## Contact
Created by [@sajalT05]