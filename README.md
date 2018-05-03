# New York Taxi Trip duration 
(please, follow this link if you are interested in my code [here!](https://github.com/KANG91/dss-project-taxi/blob/master/Kang/after_project_summary.ipynb)

### Before Start..
This is a first ML & kaggle project with my two great teammates, Sung in Ji, Moon SU Kim. We have tried to solve this project as Linear Regression, which is our first ML algorithm. Although I am not that good english writer, and we are new to data science, and machine learning, I hope you understand what we did. Appreciate in advance:)

### Synopsis
There are 1,458,644 taxi records from Jan, 01, 16 to June, 30, 16 that occured in New York. Independent variables are id which is unique value of each users, time when people pick up and drop off, place where people pick up and drop off given latitude, longitude, numbers how many people used and few more things. What we have to do was that predicted trip duration of next taxi user by using those past datas.

### Evaluation method
Root Mean Squared Logarithmic Error  
<p align="center">
  <img src="Evaluation_method" width="350"/>
</p>
epsilon is the RMSLE value(score)  
n is the total number of observations in the (public/private) data set,  
p_i is prediction of trip duration, and  
a_i is the actual trip duration for i.  
log(x) is the natural logarithm of x  

### Things that we consiered
- How to remove outliers
> remove obvious outliers at first, then check whether the performace of our model get worse or not
> 'obvious' means that could not have happened in reality normally like ride a taxi over 24days or trip from Canada to new york 
- Multicollinearity
> using VIF 
- All results we can check at 'OLS Regression summary'
> R-sqaure, Adj.R-squared, F-statistic, AIC, BIC, Condition Number and so on.
> if one of them were bad, we refects it and make a model again. 
> 
### Final result

Best score : 0.51219 - 810/1257(64%)
> feature selection : log distance from latitude, longitude, weekday, hour

### Conclusion

1. What we didn't do and we should have done in the first place
> We should have used insights from EDA, but we just repeated Trial and Error.
> While EDA, We should have focused on co-relation between independent and dependent variables.
> We should have not used visualization that we could not get any insight from them

2. What we learned from project
> 2-1. This project doesn't fit for linear regression well
> - Most of high scores teams didn't use linear regression and there is only one independent variables that has a correlation with dependent variables - ** Distance **
> 
> 2-2. How to present our project
> - Show audience result at first, and explain why we did like that
> 2-3. Best way to learn is just DOING.
> 
> - Thinking a lot doesn't really help as much as we thought
> 
> 2-4. Importance of EDA
> 
> - Good EDA make project easier and faster!

3. Now, We can do....
> - We do now know how to EDA, data preprocessing, make a visualization and check outliers, test our model and check which points are wrong.
> - We just made first, basic step of data science!
