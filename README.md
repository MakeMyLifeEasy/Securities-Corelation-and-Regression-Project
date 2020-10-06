# Securities-Corelation-and-Regression-Project

## Findings

### A.	Correlation analysis
A correlation coefficient is used to quantify the strength of association between two variables and analyse how they will behave based on historical data. The correlation matrix or correlation heatmap calculates the correlation coefficient of a security based on all other securities. The findings for this project can be summarized as follows:

#### 1.	Strongest positive correlation: Visa and Mastercard (0.912)
Visa and Mastercard both operate in the financial services industry and are payment technology companies that connect consumers, businesses and other entities to electronic payments. The prices of their stocks are closely related to each other as they operate in similar industrial environments.

#### 2.	Strongest negative correlation: Wells Fargo and GS Investment Grade Corporate Bond ETF(-0.181)
There is a high inverse correlation between Wells Fargo and GS IG Corporate bond EFT. One possible explanation for this might be the nature of their work. While both firms are associated with the financial services industry, Wells Fargo provides insurance and GS IG Bond EFT is predominantly into Investment. An increase in Insurance rates can adversely affect investment. However, the relationship between two variables can change over time and may have periods of positive correlation as well. Although these two sets of data have a strong negative correlation for the given time period, we cannot conclude that the behaviour of one security has a causation relationship with the other.


#### 3.	Some other correlations:

##### a.	Citigroup and Bank of America (0.879)
Citigroup and Bank of America have a strong positive correlation as they both operate in the Banking and investment sector of the Financial services industry.

##### b.	Abercrombie and Fitch and The Gap (0.518)
Abercrombie and Fitch and the gap are both concerned with the apparel retail industry and have a medium positive correlation.

### B.	Regression analysis
Regression analysis is a tool used for finding the relationship between two or more variables of interest (here prices of securities) and predict future data points based on historical data. In a regression model the regression coefficient is an indicator of the direction and the magnitude of the relationship while R squared gives the measurement of how closely the stock varies to the fitted regression line.

#### 1.	Regressing Visa% on Mastercard%:

●	Regression line: y = 0.00037192 + (1.03802986) x

Here we take Visa as the dependent variable and Mastercard as the independent variable. The Regression coefficient, 1.03802986, represents the rate of change in Visa as Mastercard changes. R-squared (R2) is 0.8316216841815536, which means that approximately 83% of the observed values for Visa can be explained by the Mastercard stock’s closing price. The 
mean squared error is 4.1296541519194695e-07. Therefore, the regression model for these two securities can reasonably predict the closing price for Mastercard

●	Evaluating the model

We evaluate the model by using last week’s (12/9/2019-12/13/2019) % daily change with historic (1/1/2018-12/31/2018) % daily change. Since the mean squared error value is 3.291390512583535e-07, which is very close to 0, we can conclude that our model is good.

#### 2.	Regressing Wells fargo on GS IG Corp BD EFT

●	Regression line: y = -0.00032462 + (-0.02350817) x

In this model, we take Wells Fargo as the dependent variable and GS IG Corp BD EFT as the independent variable.

The Regression coefficient, -0.02350817, represents the rate of change in Wells Fargo as GS IG Corp BD EFT changes. As this value is negative, we can say that they move in an opposite direction or have an inverse relationship. 

R-squared (R2) is 0.032793712414711296, which means that approximately 03% of the observed values for Wells Fargo can be explained by the GS IG Corp BD EFT stock’s closing price. The mean squared error is 0.0001665102377144904. Therefore, the regression model for these two securities can reasonably predict the closing price for GS IG Corp BD EFT

●	Evaluating the model

We evaluate the model by using last week’s (12/9/2019-12/13/2019) % daily change with historic (1/1/2018-12/31/2018) % daily change. Since the mean squared error value is 0.032793712414711296, which is close to 0, we can conclude that our model is good.


