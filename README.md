Data Acquisition: csv from kaggle 
Data Cleaning: Remove duplicates values, there were no missing values not incorrect data, etc. Data was almost ready and clean.

Data Preparation: I Converted some columns that have 'Yes' and 'No' values into numeric one so I can perform analysis and calculation easier.

Exploratory Data Analysis: 
1- I used summary statistics and some basic visualizations like boxplots and histograms on numeric data to describe data spread and shape using matplotlib library.
2- I created bar chart for 'Age_Category' counts using seaborn library for its more varied effects.
3- I created data frame of columns that have 'Yes' and 'No' values with their value counts indexed by 'Yes' and 'No', Then I transposed this dataframe so it can be used in a stacked bar plot to visualize the majority and minority value counts for each of these columns using matplot library.

Analyzing the Data:
I proposed three questions and used mashine learning to perfrom prediction
1- I wanted to know if there's a relation between heart disease and smoking history using this data. At first I wanted to see the relation nature across different age categories. I transformed 'Heart_Disease' column into binary numeric values instead of 'Yes' and 'No' values to get the proportion and percentages of heart disease across age categories and smoking history and then I visualized it using matplotlib. I visualized percentages of heart disease. for both somkers and non-smokers then visualized percentages of smokers for people with and without heart disease.
2- In the second question:  Is the probability of having a heart disease is the same or different as for those who smoke and for those who don't? I answered my question using hypothesis testing and set alpha to .05 .
First I divided the data into smokers and non-smokers and then bootstrapped 10000 samples to get the difference of means of the data, next I simulated dataset from the null hypothesis of different means and visualized it along with the original difference of means. Finally, I calculated P-value and made conclusion based on it.
3- Question three: Is there a relationship between General Health and Smoking?
I answered the question using matplot bar plot visualization for smoking proportions of each of General Health categories.
4- For the last section of my analysis I wanted to predict heart disease using Decision Tree Classifier. First I prepared my data by removing multi-collinearity columns, transforming columns of 'Yes' and 'No' into binary numeric values, split data into X and y and then split twice further into training, validation, testing data. I build a pipeline for decision tree model and used ordinal encoding and set max depth to 13 after tuning hyper-parameters. 
Model accuracy: 0.92
I visualized the decision logic of my model and created a horizontal bar chart for Gini Importances of the model.

Conclusions: 
1- There's positive relation between having heart disease and smoking.
2- According to test results the probability of having heart disease for smokers is higher than that of those who are non-smokers.
3- There's also a relation between general health and smoking as higher rates of smokers [53:62]% are associated with poor and fair general health conditions.
4- Model performance for decision tree classifier of heart disease is 0.9115 


