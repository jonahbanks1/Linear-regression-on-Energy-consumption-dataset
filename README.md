


In this project, I analyzed Energy consumption data on behalf of a power company.


**Dataset Description**: 
  This archive contains 2075259 measurements gathered in a house located in Sceaux (7km of Paris, France) between December 2006 and November 2010 (47 months).
Notes:
1.(global_active_power*1000/60 - sub_metering_1 - sub_metering_2 - sub_metering_3) represents the active energy consumed every minute (in watt hour) in the household by electrical equipment not measured in sub-meterings 1, 2 and 3.
2.The dataset contains some missing values in the measurements (nearly 1,25% of the rows). All calendar timestamps are present in the dataset but for some timestamps, the measurement values are missing: a missing value is represented by the absence of value between two consecutive semi-colon attribute separators. For instance, the dataset shows missing values on April 28, 2007.


**Attribute Information**:

1.date: Date in format dd/mm/yyyy
2.time: time in format hh:mm:ss
3.global_active_power: household global minute-averaged active power (in kilowatt)
4.global_reactive_power: household global minute-averaged reactive power (in kilowatt)
5.voltage: minute-averaged voltage (in volt)
6.global_intensity: household global minute-averaged current intensity (in ampere)
7.sub_metering_1: energy sub-metering No. 1 (in watt-hour of active energy). It corresponds to the kitchen, containing mainly a dishwasher, an oven and a microwave (hot plates are not electric but gas powered).
8.sub_metering_2: energy sub-metering No. 2 (in watt-hour of active energy). It corresponds to the laundry room, containing a washing-machine, a tumble-drier, a refrigerator and a light.
9.sub_metering_3: energy sub-metering No. 3 (in watt-hour of active energy). It corresponds to an electric water-heater and an air-conditioner.


**Dataset source**: https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption#


Exploratory visuals pointed to a linear relationship between variables so we use a linear regression model for this prediction.

**the steps** in ths project:
1. data importation from csv(local) to my python notebook.
2. feature selection: I dropped some columns recommended by domain experts.
3. we use the sklearn library to normalize the dataset as a numpy array. 
- this step reduces variance and allows the ML model to find more meaningful relationships in data. always recommended.
4. create a matrix of featured from the normalized dataset. X1 = all dependent variables and y1 = all the outcomes.
5. use sklearn library to split the dataset into Train and test set for validation and learning.
6. from sklearn import and fit linear model.
7. use various evaluation metrics to analyze the performance of the model.
tadah!. 
