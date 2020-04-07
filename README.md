# Cardiovascular Disease
 
## Chapter 1: Introduction
Cardiovascular disease (CVD) is a class of disease that involves the heart or blood vessels. CVD includes coronary artery diseases (CAD) such as Angina and Myocardial Infarction (commonly known as heart attack).

Other CVDs include stroke, heart failure, hypertensive heart disease, rheumatic heart disease, cardiomyopathy, abnormal heart rhythms, congenital heart disease, etc.

On a global scale, CVDs are the leading cause of death. Altogether, CVD has resulted in 17.9 million deaths (32.1%) in 2015, which is an increment from 12.3 million (25.8%) in 1990.

Deaths at a given age, from CVD, are more common and have been increasing in todayâs day and age.

Through this project and analysis, we aim to identify the factors which cause Cardiovascular diseases in adults.

SMART QUESTIONS
Can age be a factor?
How important are alcohol and smoking in affecting Cardiovascular Diseases?
Apart from the most obvious factors, what other aspects of Gender can affect the risk of CVD?
## Chapter 2: Data Cleaning

As the skewness was -0.3 which means age is approximately symmetric. As if skewness is in between scale of (-0.5 to 0.5)it will be considered approximately symmetric.

So,in age as we can see the outliers are value 30 which are outside of 1.5IQR . We are going to use capping methiod in order to treat outlier. For missing values that lie outside the 1.5IQR limits, we could cap it by replacing those observations outside the lower limit with the value of 5th %ile and those that lie above the upper limit, with the value of 95th %ile.

As we can see there are few of outliers in Height variable , which is around .004 percent of total data. since this is continous data so we are going treat with capping method. For missing values that lie outside the 1.5*IQR limits, we could cap it by replacing those observations outside the lower limit with the value of 5th %ile and those that lie above the upper limit, with the value of 95th %ile. Moreover the skewness is around -0.63 which means height column is left skewed.

As we can see now there are no outliers in height column.Also earlier there was skewness in the column and it was (-0.63) but after the outlier treatment it reduces to 0.09 . so height variable is not skewed.so we are good to go.

There are no missing variables in the data , which means that we are good to go for our bivariate analysis.
since diastolic and systolic are connected and diastolic will always be greater than systolic . so for sanity we have implement few changes to swap values if sysytolic is less than diastolic
There are no missing variables in the data , which means that we are good to go for our bivariate analysis.
Calculating BMI
Dropping the id column
so we have create 2 dummy variables for cholestrol and 2 dummy variaables for glucose category and in both the columns there are 3 levels

## Chapter 3: Graphical Representation

We see that most people who are suffering from cardio vascular diseases are of the age 60, followed by 56.Majorly, people belonging to the age group 50+ are suffering from the disease.

There are three cholestrol levels-
1- Normal
2- Above Normal
3- Way above normal
The above pie chart shows that 3/4th of the population come under the normal cholestrol category.We see that most people who are suffering from cardio vascular diseases are of the age 60, followed by 56.Majorly, people belonging to the age group 50+ are suffering from the disease.


The above graph shows that there are comparitively higher chances of women to have a cardio vascular disease where 76.9% of the women have normal cholestrol level.


The above graph suggests that there are higher number of cases for women, but there are higher number of negative cases for women and higher number of positive cases for men.

There are three Glucose levels-
1- Normal
2- Above Normal
3- Way above normal
The above graph suggests that, the majority of the population comes under normal glucose level. Additionally, for normal glucose levels the chances of having cardio-vascular disease is less whereas for above normal glucose levels the chances of having a cardio-vascular disease is more.

The graph suggests that, the majority of the population comes under normal glucose level. Additionally, for normal Cholesterol levels the chances of having cardio-vascular disease is less whereas for above normal cholesterol levels the chances of having a cardio-vascular disease is more.


## Chapter 4: Data Division & Statistical Tests

1. We used t-test to check the statistical sigificance between Height & Cardio Vascular Disease risk which showed weak significance.

2. We used t-test to check the statistical sigificance between Weight & Cardio Vascular Disease risk which showed strong significance.

3. We used t-test to check the statistical sigificance between BMI & Cardio Vascular Disease risk which showed strong significance.

4. We used chi-sqaured test to check the statistical sigificance between Diastolic & Cardio Vascular Disease risk which showed strong significance.

5. We used t-test to check the statistical sigificance between Diastolic & Cardio Vascular Disease which showed strong significance.

## Chapter 5: Models

1. Logistic Regression: We achieved an accuracy of 72% using logistic regression model. Hence, we can say it was a good fit.

2. Decision Tree: We achieved an accuracy of 71.66% using decision tree model. Hence, we can say it was a good fit.

3. Random Forest: 73.58%


## Chapter 6: Top performing features
Comparing our 3 models, we found that the most important features are:
Ap_hi (Systolic blood pressure)

Cholesterol

Age

Ap_lo (Diastolic blood pressure)

BMI

Glucose


## Chapter 7: Limitations

Lack of more detailed factors such as genetics (family history), complains of chest pain, shock factor, etc.
Time periods for when a factor acted up were not available.
Separate data for both types of cholesterol (HDL and LDL), would have helped better in the classification.
## Chapter 8: Conclusion

Through our analysis, it was clear that most of the important features that run a risk to affect CVD are those that can be directly or indirectly affected by our health choices.
Some factors, however, are not in our control. After the age of 55, our chances to acquire a CVD increases greatly. This risk is greater for men than women between the ages of 40 â 59.
BMI is another factor that affects getting CVD. Considering this factor in terms of gender, middle-aged women tend to have a higher BMI than men. This is because, the body fat mass in middle-aged women tends to increase in general. M (30%) W (42%).
Features such as alcohol, smoking and physical activity are indirectly related to running a risk of CVD.
In general take care of your health and be happy.
