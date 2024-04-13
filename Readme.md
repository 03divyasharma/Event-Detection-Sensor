# Event Detector Sensor

## Introduction
This is a programming assignment of the following course:

[Data For Machine Learning](https://www.coursera.org/learn/data-machine-learning)

## Description

The main data was gathered from an experimental sensor device oserving an electro-chemical plant. The sensor device detects "interesting" events. These events were labeled by an expert into four different classes `"P"`, `"N"` and `"L"`  as well as `"-"`, which denotes a false detection (not an "interesting" event). The data shows readings for 9 different sensors along with a 'detection mode'&mdash;which affects the class of detected phenomenon&mdash; along with the date annd time when events happened. 

However, the expert also indicated that multiple factors affect the sensor readings as well. The fecators can be put into two broad categories: weather conditions where the device was used and the calibration of the device itself. For this reason, we gathered two more datasets to be used alongside the main data: 

One shows daily averages of three different weather indicators: temperature, humidity and wind level in the area the device was opertaing, as the expert indicated these may be the most relevant factors.

The other dataset is acquired from the logs of the maintenance done on the device: Every week at midnight on Friday, the device was turned off and inspected by a technican in the foloowign day. If the device was found to be near-faulty (indicated from certain measurements taken from device), the device was repaired and recalibrated. Again, the expert indicated three different measurements from the device that might be affecting the sensor readings. The device was turned back on again on midnight on Saturday.

## Aim

We want to develop an algorithm that detects the class of the events automatically. We are informed, however, that there is a separate device available that indicates false detections, so there is no need for our algorithm to identify those.



## File Structure
The `assignment grader` file is named as `Programming Assignment.ipynb`. The other three files constitute the modified version of the same. The three different datasets are put in different notebooks and processed in indivisual files. Finally I've concatenated the results into one file `AligningAndAggregating.ipynb`.


## Datasets
The entire dataframe for all three datasets was given in the assignment grader file only. There was no explicit `csv file` provided. You can copy the cell output which gives a txt file. It can be converted into `'html document` and easily read using pandas command:

 `pd.read_html("file_name.html", skiprows=1)[0]`

 Then modify the result into correct dataframe format such as adding column names and dropping extra index column. 

## Skills:

### This assignment focuses on :
#### 1. Pandas 
#### 2. Numpy 
#### 3. Data Preprocessing
#### 4. Data Vizualization
#### 5. Feature Engineering 
#### 6. Feature Extraction 
#### 7. Python

## Note

To use result variables from another notebook:

   Save those variables in their original notebook as `%store "variable_name"` and retrieve in whichever notebook you need it by typing command `%store -r variable_name"`.
