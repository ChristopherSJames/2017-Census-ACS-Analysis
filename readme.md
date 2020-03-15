# 2017 Census Income Per Capita analysis
## by Christopher James

## Dataset

This dataset contains population, travel, work, and income information from the 2017 Census Bureau ACS survey. Wrangling was done in the notebook 'census_wrangle.ipynb'. 
	The column 'County' had values that all contained the word 'County' in them. This was redundant, so I removed this word from them.
	There were not enough missing values in any column to cause any significant changes, so I toyed around a bit by using a random forest regressor to
predict a few of the values of one of them.

## Summary of Findings
	UNIVARIATE ANALYSIS
	The distribution of per capita income peaks between 20k and 25k dollars and declining from there, until it reaches 130k, with few after that.
	Poverty levels are rightly skewed quite a bit. They start off between 0 and 10 percent, and rapidy decline from there, espicially after 20%.
Few Census tracts have poverty levels abouve 70%.
	Much like poverty levels, the child poverty levels are rightly skewed, but in a somewhat less dramatic way. The fall after 20% onward is less pronounced. 
In addition, there are more places that have child poverty levels abouve 70%.
	The distribution of professional jobs is rightly skewed, peaking at between 20 and 30 percent, before falling slightly at 30%, then falling rapidly until it gets to 80%. 
Few tracts have a level higher than that.
	Service jobs peak early on, between 10 and 20 percent, before collapsing rapidly through between 40 and 50%. After that, the numbers are extremely low.
	The distribution of tracts based on percentage of jobs in construction is extremely skewed to the right, peaking right off the bat between 0 and 10%. 
It then falls rapidly to between 30 and 40%, with very little after that.
	The distribution of production job levels is extremely skewed to the right, with the majority, along with the peak, occuring before it hits 20 percent. 
Then it declines until it hits 50%, with virtually nothing after that.
	This chart of the distribution of work at home job levels is about as rightly skewed as they come. 
It clearly peaks between 0 and 10%, before cliff diving until it hits 30%, with nothing after that.
	In yet another incredibly skewed chart, the vast majority of tracts have unemployment levels between 0 and 10%. 
After that, there is an enormous drop that culminates with a flat line after 40%.
	BIVARIATE ANALYSIS
	Per capita by poverty shows that even a somewhat small amount of poverty can have large negative consequences. 
Per capita income falls much more when poverty increases from a lower amount than it does from a higher amount.
	The effect that child poverty has on per capita income is smaller than overall poverty, with a more even and gradual decline as child poverty increases.
	There is a pretty strong coorelation between increased per capita income and increased percentage of professional jobs. 
Interestingly enough, that coorelation appears to get somewhat weaker towards the higher end of the professional jobs scale.
	There is a negative coorelation between per capita income and the level of service jobs. 
It is not as strong as that of professional jobs. There also seems to be far fewer tracts that have more than 40% service jobs than professional jobs.
	There is a weaker coorelation between per capita income and the percentage of construction jobs than there is between either professional or service jobs.
	There is a negative coorelation between per capita income and percent of production jobs slightly greater than that of construction jobs. 
There appears to be a slightly higher percentage of tracts that have these jobs at rates higher than 20% than do construction jobs.
	There appears to be little coorelation between work at home jobs and per capita income.
There is a moderate coorelation between unemployment and per capita income.
	MULTIVARIATE ANALYSIS
	Per capita income is higher in places that have more professional jobs and lower levels of poverty. 
Even though the overall trend is clear, there appear to be plenty of places with lower poverty levels that have lower levels of incomes and professional jobs. 
In addition, places with high poverty seem to stagnate in the income department even with the increase in professional jobs.
	Per capita income seems to benefit when there are less production jobs. 
As seen with professional jobs, places with the highest poverty levels are not affected by the level of production jobs.
	Per capita income drops rapidly with just a fairly small increase in service jobs, then the decrease is much more mild after that. 
A pattern appears to be emerging that shows that per capita income in places with high poverty does not change no matter the job composition.
	The trend points to per capita income increasing along with the level of professional jobs, along with the decreasing number of service jobs. 
The service job level seems to be more polarized than with poverty levels.
	The trend points to per capita income increasing along with the level of professional jobs, along with the decreasing number of construction jobs. 
Even though the overall trend is clear, there appear to be plenty of places with higher construction job levels that have lower levels of incomes and professional jobs.



## Key Insights for Presentation

Per capita income is higher in places that have more professional jobs and lower levels of poverty. 
Even though the overall trend is clear, there appear to be plenty of places with lower poverty levels that have lower levels of incomes and professional jobs. 
In addition, places with high poverty seem to stagnate in the income department even with the increase in professional jobs.
	Per capita income seems to benefit when there are less production jobs. 
As seen with professional jobs, places with the highest poverty levels are not affected by the level of production jobs.
	Per capita income drops rapidly with just a fairly small increase in service jobs, then the decrease is much more mild after that. 
A pattern appears to be emerging that shows that per capita income in places with high poverty does not change no matter the job composition.
	 It might seem surprising that there is not a stronger coorelation between unemployment numbers and per capita income. 
However, it could be that there are simply not that many tracts with high enough levels of unemployment to bring down the averages.

