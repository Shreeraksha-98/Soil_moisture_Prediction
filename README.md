# Hyperspectral benchmark dataset on soil moisture

Hyperspectral and soil-moisture data from a field campaign based on a soil sample. Karlsruhe (Germany), 2017.

## Description
This dataset was measured in a five-day field campaign in May 2017 in Karlsruhe, Germany. An undisturbed soil sample is the centerpiece of the measurement setup. The soil sample consists of bare soil without any vegetation and was taken in the area near Waldbronn, Germany.

## Variables

- **datetime:** date and time of the measurement
- **soil_moisture:** soil moisture in %
- **soil_temperature:** soil temperature in °C
- **454, 458, … 946, 950:** hyperspectral bands in nm

Outliers are treated using IQR capping method.
The important features are selected using ExtraTreeRegressor.
The RandomForestRegressor is then trained on the training data and tested on the testing set.