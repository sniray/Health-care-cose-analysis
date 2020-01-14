# Health-care-cose-analysis
A nationwide survey of hospital costs conducted by the US Agency for Healthcare consists of hospital records of inpatient samples. The given data is restricted to the city of Wisconsin and relates to patients in the age group 0-17 years. The agency wants to analyze the data to research on healthcare costs and their utilization
1.	To record the patient statistics, the agency wants to find the age category of people who frequent the hospital and has the maximum expenditure.
SOLUTION - I am using graphical analysis. A histogram would display the number of occurences of each age category. The as.factor is applied to convert the categories if they are numbers.
As I need the expenditure for the age and find the maximum value. I will use the aggregate function to add the 	values of total expenditure according to the age.
2.	In order of severity of the diagnosis and treatments and to find out the expensive treatments, the agency wants to find the diagnosis-related group that has maximum hospitalization and expenditure.
SOLUNTION-Here I have used the which.max () function to get the index of the data frame with the maximum value.
3.	To make sure that there is no malpractice, the agency needs to analyze if the race of the patient is related to the hospitalization costs.
SOLUTION- used NA.omit to remove n values. Converted the race variables to factors and performed the summary to know how many patients of different categories/groups were admitted. To find the impact of races on costs(weather it has or not) applied ANOVA.
4.	To properly utilize the costs, the agency has to analyze the severity of the hospital costs by age and gender for the proper allocation of resources.
SOLUTION: Used Linear regression. As per the result the age is very important factor in hospital costs (as per the significance level and p-value. As per the summary there are equal number of male and female patients. The negative coefficients show that on an average female sustain lesser cost than male.
5.	Since the length of stay is the crucial factor for inpatients, the agency wants to find if the length of stay can be predicted from age, gender, and race
SOLUTION-Used linear regression. The significant codes are almost null for all variables ,except for the intercept. The high p-values says that there is no linear relationship between the given variables. That is with just age, gender and race. So its not possible to predict the length of stay.
6.	To perform a complete analysis, the agency wants to find the variable that mainly affects hospital costs
SOLUTION-Used linear regression. As the age and length of stay affect the hospital cost. Length of stay positively affects the cost. 
