# Pokemon-Go-Data-Analysis-
The Pokémon Go project analyzes the various Pokémon's pre-evolution and post-evolution stats and tries to predict the post-evolution combat power using multiple linear regression. 


**1. About the dataset:**


The dataset includes information about various Pokémon species and their post and pre-evolution stats such as combat power (cp), weight, strong attack value, type, weak attack value, etc. There are 27 columns in the dataset and 75 rows of data. The column attack_strong is about various stronger attacks of the Pokémon and there are other columns which describe the strong attack’s damage and type. Similarly, attack_weak is about the weaker attack of Pokémon and it also has other columns that describe its damage and type.

**2. Data cleaning:**


There was no missing data or funky data in any of the columns of the dataset so there was no need for data cleaning. All the data types were also appropriate based on the data in the column. The only column that was deleted was the notes column because it didn’t serve any purpose for any analysis.

**3. Initial analysis:** 


From the initial analysis, the average CP of post evolution Pokémon species are greater than the average CP of pre-evolution Pokémon species. The post-evolution Pokémon’s are stronger than pre-evolution. In addition to this, the most common strong attack type in pre and post evolution Pokémon’s was struggle. Finally, the pre-evolution Pokémon’s weighted less compared to the post evolution Pokémon’s as it can be seen in the histogram.

**4. ANOVA:**

The first anova was a one-way anova to test whether all the post-evolution strong attack types have the same damage value. There are 6 types of strong attacks and from the anova test, it was found that they don’t all have the same damage value hence the hypothesis was rejected. The alpha value was 5%, and the p value was less than 5%. The 2nd hypothesis testing was a 3-way anova to test the impact of species, weak attack type, and strong attack type on the CP of post evolution Pokémon’s. The null hypothesis was that all the 3 independent variables don’t have a significant impact on the CP. After finding the p value, the null hypothesis was rejected because it was less than the alpha of 5%. Therefore, the species, weak attack type, and strong attack type does have an impact on the CP.

**5. Regression analysis:** 


Weight, power up candy, and power up stardust columns were used to predict the CP of post evolution species. The power up candy is the candy required to power up the Pokémon, likewise, power up stardust is the stardust required to power up the Pokémon. A data table with the actual and predicted CP values is the output of the regression analysis as well as a graph. The predicted values were not too far from the actual values except for the 3 negative predicted values. The model predicted 3 negative CP, which is wrong because combat power cannot be negative. There were also 2 actual values that was in the 1000s but the predicted CP was only
609. My guess for the cause of some wild predicted CP values is that there were only 75 rows of data. If there was more data, the predicted values would have been closer to the actual values of CP. The goodness of fit for the regression analysis was 42% which is still below 50% so the model has some flaws.
