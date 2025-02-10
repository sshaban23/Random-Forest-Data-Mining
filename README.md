# Random-Forest-Data-Mining

A1: PROPOSAL OF QUESTION:

My research question is: 
'What factors contribute to customer churn?' To analyze this, I used a Random Forest model, which is a robust machine learning technique that helps identify the key factors influencing whether customers decide to leave the service.


A2: DEFINED GOAL:

My goal for this data analysis is to identify the key factors that influence whether a customer will churn or not. By examining various attributes such as demographics, geographic location, service usage, and customer interactions, I aim to pinpoint which variables are most strongly associated with customer churn. Understanding these factors will help me develop strategies to retain customers and improve overall satisfaction. This analysis is achievable with the data I have, as it includes comprehensive details about each customer's profile and their service history.

B1: EXPLANATION OF CLASSIFICATION METHOD:

I chose the random forest prediction method because it analyzes the data set by creating multiple decision trees using different subsets of the data. Each tree makes its own prediction about whether a customer will churn or not, and then the method combines these predictions to make a final decision. This approach helps to reduce errors and improve accuracy compared to a single decision tree. I expect that the random forest method will help me identify the most important factors contributing to customer churn and provide a reliable model for predicting churn based on the various customer attributes in my dataset.

B2: SUMMARY OF METHOD ASSUMPTION:

One assumption of the random forest prediction method is that the individual decision trees within the forest are relatively uncorrelated with each other. This means that each tree should provide unique insights based on different subsets of the data and features. By ensuring that the trees are diverse, the random forest method can combine their predictions to create a more accurate and robust model. This assumption is crucial because if the trees were too similar, the benefits of averaging multiple trees would be lost, and the model's performance would not improve significantly over a single decision tree.

B3: PACKAGES OR LIBRARIES LIST:

- Pandas is used to load, clean and prep the data for analysis.
- Numpy provides support for numerical computations and handling arrays, which are useful for various data operations and manipulations within the analysis.
- Scikit-learn is necessary for Machine Learning because it has tools to implement the Random Forest model, split the data, evaluate the model.
- Matplotlib helps create visualizations of the data and present analysis results.
- Seaborn also has visualization capabilities, also can help us identify patters and understand the data.
- SciPy has advanced statistical tools for data manipulation and statistical analysis.
- Joblib is a library for loading and saving machine learning models which will help me serialize the random forest.

C1: DATA PREPROCESSING:

One data preprocessing goal relevant to the random forest prediction method is to handle missing values in the dataset. Random forest algorithms can handle some missing values, but it is essential to ensure that these are managed properly to improve the model's accuracy and reliability. This can be achieved by imputing missing values with appropriate strategies, such as replacing them with the median or mode of the respective column.

C2: DATA SET VARIABLES:

Numeric Variables:
1.	Age
2.	Income
3.	Outage_sec_perweek
4.	Email
5.	Contacts
6.	Yearly_equip_failure
7.	Tenure
8.	MonthlyCharge
9.	Bandwidth_GB_Year
    
Categorical Variables:
1.	City
2.	State
3.	County
4.	Area
5.	TimeZone
6.	Job
7.	Children
8.	Marital
9.	Gender
10.	Churn (target variable)
11.	Techie
12.	Contract
13.	Port_modem
14.	Tablet
15.	InternetService
16.	Phone
17.	Multiple
18.	OnlineSecurity
19.	OnlineBackup
20.	DeviceProtection
21.	TechSupport
22.	StreamingTV
23.	StreamingMovies
24.	PaperlessBilling
25.	PaymentMethod


C3: STEPS FOR ANALYSIS:

The steps I took to prepare for this analysis began with importing the necessary libraries and loading the dataset. I then dropped irrelevant columns that would not contribute to predicting customer churn. Next, I handled missing values by filling in numeric features with their median values and categorical features with their most frequent values. For binary categorical variables, I transformed them into a single column with values of 0 and 1, instead of creating multiple columns, to accurately represent their binary nature. After that, I one-hot encoded the non-binary categorical variables to convert them into a format suitable for machine learning models. I defined the target variable, 'Churn,' and separated it from the feature set. Finally, I split the data into training and testing sets to build and evaluate the predictive model accurately.

D2: OUTPUT AND INTERMEDIATE CALCULATIONS:

To analyze the data and predict customer churn, I used the Random Forest algorithm. I believe it is the best model because it builds multiple decision trees and merges them to get a more accurate and stable prediction.

![image](https://github.com/user-attachments/assets/b16d452c-fe62-4ba4-ae62-08220df3a428)

![image](https://github.com/user-attachments/assets/2c716a61-ae7b-4ef5-8140-780f0834ab93)


E1: ACCURACY AND MSE:

Using the Random Forest algorithm, I analyzed the data to predict customer churn. After cleaning and preparing the data, I trained the model and evaluated its performance. The model achieved an accuracy of 87.85%, meaning it correctly predicted whether customers would churn almost 88% of the time. Additionally, the Mean Squared Error (MSE) was 0.1215, indicating that the average squared difference between the predicted and actual values was low. These results demonstrate that the Random Forest model is effective and reliable for predicting customer churn, providing useful insights to help improve strategies for keeping customers.

E2: RESULTS AND IMPLICATIONS:

The results of my prediction analysis are impressive, with an accuracy of 87.85% and a low Mean Squared Error (MSE) of 0.1215. This means the model reliably predicts customer churn, correctly identifying which customers are likely to leave. These findings help us understand why customers might churn, so we can take action to keep them.

E3: LIMITATION:

One limitation of my data analysis is that it relies solely on the data available in the dataset, which may not include all the factors influencing customer churn. For example, personal reasons or external economic conditions could also play a significant role, but they aren't captured in the data we have. Additionally, if the data contains any biases or inaccuracies, those will also affect the model's predictions. This means that while the model is useful, it may not account for all the nuances of customer behavior, and its predictions should be interpreted with some caution.

E4: COURSE OF ACTION:

Based on my results and the insights gained from the Random Forest model, I recommend that the organization focus on improving customer retention strategies by targeting the factors most associated with churn. We should prioritize reaching out to at-risk customers identified by the model, offering them personalized incentives and support. Additionally, we should regularly review and update our data to ensure the model remains accurate over time. By taking these proactive steps, we can reduce customer churn, enhance satisfaction, and ultimately strengthen our customer base and overall business performance.






























