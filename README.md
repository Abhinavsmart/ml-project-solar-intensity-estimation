# CSE 343 Machine Learning

## Solar Intensity estimation using time series weather data

We apply machine learning techniques to predict solar intensity in a region 48 hrs to the future using local time series weather data.

## Contributors
- Kushal Juneja (2019057, kushal19057@iiitd.ac.in)
- Naval Kumar Shukla (2019065, naval19065@iiitd.ac.in)
- Rishi Singhal (2019194, rishi19194@iiitd.ac.in)
- Udit Narang(2019120, udit19120@iiitd.ac.in)

## Abstract
Predicting future renewable energy generation is important, since the power grid must use fossil fuel based energy as demand varies. We explore prediction models for solar power generation from NSRDB database using machine learning techniques. We compare multiple regression techniques for generating prediction models.

## Motivation
Energy from the sun is an inexhaustible resource that creates little to no pollution. However, current methods of collecting solar energy and converting it to electricity can capture and store only a small amount of the available energy from the sun at any given time. The highly variable nature of solar energy production puts stress on fossil fuel based power generation. We aim to predict solar intensity for a given area 48 hours into the future using local time-series weather data. Our goal is to provide high-confidence forecasts of solar generation (via solar intensity) using readily-available weather data. This will enable better regulation of fossil fuel based power generation. We have acquired solar intensity and weather data from NSRDB and Sunrise-Sunset-API. This project aligns with our sustainable development goals and deploying machine learning techniques to solve real world problems.

## Dataset Description
The NSRDB dataset includes both observed weather data (temperature, pressure, cloud cover, solar zenith angle ,etc.) and solar intensity data measured in watts per square meter. The dataset includes several solar radiation measures such as Diffused Normal Irradiance (DNI), Diffused Horizontal Irradiance (DHI) and Global Horizontal Irradiance (GHI). We choose to include GHI measurements since it incorporates DHI, DNI and ambient solar radiation reflected from nearby surfaces. This makes it a good indicator for solar panel readings.

The NSRDB data is measured once every 10 minutes. We investigate a single location - Las Vegas, Nevada, USA. We limit our analysis to the year 2019 only.
<br>
Our dataset contains more than 50,000 distinct observations, each with 16 features (including Time values such as Month, Day, Hour and Minute) shown in table 1 with corresponding measure of GHI.

We obtain the sunrise and sunset times for each day from Sunrise-Sunset-API\cite{sunrise}. Using this, we add a new boolean column 'isDay'.

## Dataset Link
To access the final dataset that we have used in our project, visit : https://drive.google.com/file/d/18AaOanU9qqKgag7rtMpUm9I4kVXVocPt/view?usp=sharing

## Libraries Used
1. Numpy<br>
2. Pandas<br>
3. Matplotlib<br>
4. Seaborn<br>
5. Scikit-Learn<br>

## Models & Techniques Used
1. Linear Regression & its subtypes<br>
2. Polynomial Regression<br>
3. SVM Regression<br>
4. Regression Trees<br>
5. Artificial Neural Networks<br>
6. Alpha Pruning<br>
7. Feature Expansion<br>
8. PCA<br>

## Other Details
Simply download the datasets from the link shared above, then run the .ipynb files for training & testing on different models. You could also access the models & their features using the pickled models present in the weights/models folders.

To run the pickled files used the following code snippet:

![image](https://user-images.githubusercontent.com/58341663/143772279-889238f0-9d67-4819-8505-d33eb3a02e15.png)

Note : For further results & analysis of our models, please refer to the final report that we have uploaded.

## Future Work
<ol>
<li>Train dense neural networks </li>
<li>Apply deep learning techniques such as LSTM’s, recurrent neural networks etc.</li>
<li>Apply clustering techniques </li>
<li>Extend our predictions to more geographical locations</li>
</ol>  


