# EarthWise - Spot the Fire V3.0

MODIS (or Moderate Resolution Imaging Spectroradiometer) is a key instrument aboard the Terra (originally known as EOS AM-1) and Aqua (originally known as EOS PM-1) satellites. Terra's orbit around the Earth is timed so that it passes from north to south across the equator in the morning, while Aqua passes south to north over the equator in the afternoon. Terra MODIS and Aqua MODIS are viewing the entire Earth's surface every 1 to 2 days, acquiring data in 36 spectral bands, or groups of wavelengths (see MODIS Technical Specifications). These data will improve our understanding of global dynamics and processes occurring on the land, in the oceans, and in the lower atmosphere. MODIS is playing a vital role in the development of validated, global, interactive Earth system models able to predict global change accurately enough to assist policy makers in making sound decisions concerning the protection of our environment.


MODIS standard quality Thermal Anomalies / Fire locations processed by the University of Maryland with a 3-month lag and distributed by FIRMS. These standard data (MCD14ML) replace the NRT (MCD14DL) files when available.

Dataset contains:

1.	Latitude
2.	Longitude
3.	Brightness
4.	Scan
5.	Track 
6.	Acq_date
7.	Acq_time
8.	Satellite
9.	Confidence
10.	Version
11.	Bright_t31
12.	Frp
13.	Daynight

Code explanation:	

1.	Plot histogram using brightness
2.	Find quantile of brightness, latitude and longitude
3.	Divide brightness in low, high and extreme on the basis of value and add this as a column
4.	Categorize area on the basis of latitude and longitude
5.	Preprocess the data by replacing object value with integer value
6.	Apply different machine learning algorithms

    6.1 Kneighbours

    6.2 SVC

    6.3 Random Forest

    6.4  Logistic Regression

     6.5 SGD

