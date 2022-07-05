


In this project, I analyzed Energy consumption data on behalf of a power company.
Exploratory visuals pointed to a linear relationship between variables so we use a linear regression model for this prediction.


the steps in ths project:
1. data importation from csv(local) to my python notebook.
2. feature selection: I dropped some columns recommended by domain experts.
3. we use the sklearn library to normalize the dataset as a numpy array. 
- this step reduces variance and allows the ML model to find more meaningful relationships in data. always recommended.
4. create a matrix of featured from the normalized dataset. X1 = all dependent variables and y1 = all the outcomes.
5. use sklearn library to split the dataset into Train and test set for validation and learning.
6. from sklearn import and fit linear model.
7. use various evaluation metrics to analyze the performance of the model.
tadah!. 
