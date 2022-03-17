JOB QUALITY IN OECD COUNTRIES

**Goal**

The determinants of job quality are visualized which can provide insights towards discriminated or privileged groups and the manner in which they are particular. By considering the shown details, policymakers and the general public can set goals and work towards improving job quality balance. 

**Motivation**

OECD member countries comprise developed countries like Australia, Canada, the US, the UK, Japan other developed European countries.  It would make sense to find the quality of the job in those countries. The quality of a job is directly proportional to the social and economic advancement of that country. So, one can assume that underdeveloped, developing countries have low job quality in comparison to developed countries. So, taking the first step to measure the job quality of OECD countries and comparing it with the other nations as we progress would be ideal.  

**Dataset**

The data is from oecd.org. This database is structured around the three main dimensions of the OECD Job Quality framework. It displays country-level information on Earnings Quality, Labor Market Security, and the Quality of the Working Environment as well as their sub-dimensions. Data are available between 2005 and 2015 for OECD countries. The figures can be disaggregated by gender, by age (15-29, 30-49, and 50-64), or by education groups (low, medium, and high). Additional datasets, also from OECD, give data on hourly wages, working hours, career advancement opportunities, physical health factors, etc.

**Methodology**

Five different models were used to find the R-squared score. They are Linear Regression, Decision Tree Regressor, Decision Tree Classifier, Random Forest Classifier, and Oblique Decision Tree. 


R-squared (R2) is a statistical measure that represents the proportion of the variance for a dependent variable that's explained by an independent variable or variables in a regression model. Whereas correlation explains the strength of the relationship between an independent and dependent variable, R-squared explains to what extent the variance of one variable explains the variance of the second variable. So, if the R2 of a model is 0.50, then approximately half of the observed variation can be explained by the model's inputs.

Experiment #1

The attributes/features were "Sex, Country, Age, EDU, Components, and Time".  The target was the "Value". The best r2 score was given by the Decision Tree Regressor. The second best was Oblique Decision Tree. However, it was computationally expensive in comparison to the other models used. The blue line in the figure represents the linear regression line in the scatter plot. The title of the figure contains the r2 score value for the respective model. 

Experiment #2

The attributes/features were "Country and Type".  The target was the "Value". Out of all the models, Decision Tree Regressor has the better r2 score in comparison. The second best was the result given by the Oblique Decision Tree. However, the score was less than 0.5 in both cases. The blue line in the figure represents the linear regression line in the scatter plot. The title of the figure contains the r2 score value for the respective model. 

**Cluster Analysis**

A clustering algorithm was used based to divide the countries into groups based on inherent patterns present in their values of Earnings Quality, Job Strain, GDP, etc. 

K-means clustering was the clustering algorithm of choice. But similar results were found through other methods as well.

Through the use of the elbow-method, it was found that the ideal number of clusters is k=3. The main factor that seemed to differentiate these clusters is the GDP of the countries. The division boundaries for the 3 Tiers on the basis of GDP is:

Tier 1: GDP > 50000

Tier 2: 30000 < GDP < 50000

Tier 3: GDP < 30000

The same division boundaries in the clusters were found for the year 2010 as well as 2015, but the members of the clusters were found to be different due to rise and fall of the GDP in certain countries. These results help us to clearly see which countries are showing growth or decline. They also help us analyze trends in nations with higher GDP vs nations with a lower GDP.

**Trend Analysis**

The trends of various metrics between the years 2010 and 2015 can be visualized in this section.  Trends are found by seeing the change in the values of the various metrics between 2015 and 2010 and normalizing the values. Visualizations are made using Geopandas.

**Results and Discussion**

Data Analysis Result

1] There is a positive correlation between the quality of the working environment and labor market security, whereas earnings quality has a negative correlation with them. 

2] The age range of 15-29 has the highest job strain bar, highest physical health risk factors bar, and highest inflexibility of working of hours bar which implies that they have the least quality of the work environment in that aspect as compared to the age group of 30-49 and 50-64. However, they have the highest bar in the opportunity for career advancement which works better on their behalf. In contrast, the age group of 50-64 has comparatively less job strain, fewer physical risk factors, less inflexibility of working hours, and less opportunity for career advancement. The population of 30-49 has better work autonomy and learning opportunities, training and learning opportunities, but however, has long working hours. 

3] Men have the highest job strain bar, highest physical health risk factors bar, and highest long working hours bar which implies that they have the least quality of the work environment in that aspect as compared to women. However, they have better work autonomy and learning opportunities, and opportunities for career advancement than women. Women have better long working hours and better training and learning opportunities than men. Women have more inflexibility of working hours than men.

**Methodology Result**

Experiment #1
Out of the 5 models used, Decision Tree Classifier, Decision Tree Regressor, and Oblique Decision Tree had R-squared score over 0.5. However, in comparison to Decision Tree Regressor and Oblique Decision Tree, Decision Tree Classifier didn't perform well. There is only a close difference of less than 0.006 between Decision Tree Regressor and Oblique Decision Tree. Out of the two, Decision Tree Regressor performed the best with an R-squared score of 0.929. 

Experiment #2
Out of the 5 models used, Decision Tree Regressor and Oblique Decision Tree had better R-squared scores. However, the value is less than 0.5.  The R-squared score by Decision Tree Regressor is 0.3454 and the R-squared score by Oblique Decision Tree is 0.3449. Thus, out of the two, Decision Tree Regressor performed slightly better than Oblique Decision Tree. 

**Conclusion**

From the result of Experiment #1 and Experiment #2, Decision Tree Regressor has the best performance. The Oblique Decision Tree comes to the second position.**

**Cluster Analysis**

Result

The countries were divided into 3 clusters, with the primary dividing factor being the GDP of the countries.

Conclusion

These results seem to reflect the basis on which we have already divided the countries as first world, second word and third world countries, which is also a division that is made based on the economic factors of these countries. It also shows that GDP is a very powerful measure of a nation as it provides a more clear representation of a country than all the other measures.

**Trend Analysis **

Result

It is observed that the number of hours of work per week required by the employees in most countries has reduced in 2015, with a high positive correlation to the Job strain experienced and the nation's GDP.

We also find that more countries have seen an increase in Earnings Quality for low-skilled workers compared to more highly skilled workers. Earnings Quality is only positively correlated to the GDP of the country.

We find that LMI is higher in European countries and has shown a large decrease in America. The GDP of these nations also shows a high positive correlation to their LMI and Unemployment Duration.

It is observed that a larger number of countries have seen a decline in job strain for men than for women. It is also observed that the reduction in job strain has been more prevalent in medium-skilled workers compared to others.

Conclusion

The data shows the clear need and effect of having a work-life balance, which has often been a topic of dispute. The reduction in hours worked per week by employees in most countries indicates that the world is moving towards establishing a better work-life balance for everyone. This, combined with a reduction in  Unemployment Duration and Labour Market Insecurity has led not only to an improvement in people’s lives but the countries’ GDP as a whole.  

The data indicate that increasing work hours does not usually lead to an increase in Earnings Quality or GDP.

The improvements that were seen in the Earnings Quality of Low skilled workers also shows that a lot of nations are focusing on increasing the Quality of work and life for people working in the labor force.

The disparity between the reduction in Job strain between men and women also indicates that there is a need to restructure workplace policies to particularly address the factors contributing to the stress that women experience at work. 

**
**Future Work**

The work done here is not fully comprehensive of job quality across all the different countries. Ethical concerns involve the validity and representational power of the dataset. Finding additional datasets with different features would help strengthen the points for policy changes.

Our next step is to find Job Quality in the following group of countries.

Job Quality in each Continent

Job Quality of Developed Countries Only

Job Quality of Developing Countries Only

Job Quality of Undeveloped Countries Only

**References**

OECD.org, https://www.oecd.org/statistics/job-quality.htm

https://stats.oecd.org/Index.aspx?DataSetCode=SKILLS_2018_TOTAL
