# **Notes**

> Relative frequency = Frequency / Total number of tries

> Relative frequency becomes more stable with more number of tries.

> For discrete variables, mean and variance can be calculated for probability distribution.

> For continuous variables, are under the Probability Density function determines the probability.

> Stock data is continuously distributed. 

> VaR: Measure of how much a set of invstment might lose

RANDOM SAMPLING

> ddof=1, provides an unbiased estimator(divides by n-1) while, ddof=0 provides maximum likelihood estimato(divides by n).

> Degrees of freedom: Number of values in calculation that are free to variate.

VARIATION OF SAMPLE

> Central limit theory of statistics say, if the sample size is large, the distribution of sample means looks like normal one. Hence, we can conclude this way, even if the population is not normal, the sample is approximately normal if the sample size is large enough. 

> Sample mean and standard deviation keep changing for a population, but always within a certain range.

> Population average means are usually normally distributed while sample means are right skewed. But for large sample size, sample means appear normally distributed. 
 
CONFIDENCE INTERVALS

> If sample is a good representation of a population, population mean must be close to sample mean.

> If confidence interval is on the positive side it implies that the average return is very likely to be positive.

> x% confidence interval means that there is a x% chance that the average stock return lie between the lower and upper bounds.

HYPOTHESIS TESTING

> In hypothesis testing, we start with assumption that the null is correct. Hence, we know population mean is equal to 0. But in most situations, population standard deviation is not known. Then we can replace population standard deviation with the sample standard deviation. Then this new term denoted as t-hat, has a new distribution, t-distribution.

> If sample size is large enough, we can use z-distribution instead of t-distribution.

> P value test:
>>   If Ha: mu not equal 0, it is two tail test and  p-value=2(1-norm.cdf(np.abs(z), 0, 1))
>
>>if Ha: mu>0, it is upper tail test and  p-value=1-norm.cdf(z,0,1)
>
>>if Ha:mu<0, it is lower tail test and  p-value=norm.cdf(z,0,1)

LINEAR REGRESSION MODELS

> Covariance: Degree of association between two or more random variables.

> Correlation: Covariance is divided by the standard deviation of both variables. Now, the correlation will only take values in between negative one and one, no matter what are the variation of the two variables.
 
> Covariance and correlation can only address linear pattern. There are quite a lot of quantitative measure for non-linear association.

> Correlation only measures strength of association between two variables.

> Variable user wants to estimate is called response and variables used to estimate response is called predictors.

> We assume that response variable in population are all normal. They have equal variance sigma square. But in the mean of the response variable is determined by predictors. In linear form, mu_i equal to beta_0, plus beta_1, times X_i. Like in confidence interval estimation, we use the samples to estimate a population parameter, mu. Similarly, we also use samples to estimate parameters of population, beta_0, beta_1, sigma. In conclusion, if we apply linear regression model, we assume there exists such a real pattern in population. More specifically, linearity: The mean of y is linearly determined by predictors. Independence: With different X, responses are independent. Normality: The random noise and y follow normal distributions. Equal variance: The variance y are all equal even if the values of predictors are different.

> Assumptions
>> Independence
>
>> Linearity
>
>> Normality
>
>> Equal Variance

VALIDATION AND DIAGNOSIS OF MODEL ASSUMPTIONS

> Durbin Watson is that, there's no serial correlation in errors.

>  We have a rule of thumb that test statistic values in the range of 1.5 and 2.5 are rated normal. If below 1.5, it maybe positively correlated. If above 2.5, it maybe negatively correlated, hence an assumption of independence is violated. For normality validation, we can use quantile - quantile plot or QQ plot. We use stats.probplot from python package scipy.stats to draw QQ plot. The first input of probplot is a standardized error. The second term dist = 'norm' is to compare your distribution of standardized error with normal distribution. If errors follow normal distribution, they will fall on the 45 degree line roughly. In our model, it deviates a bit in the right tail, but overall it satisfies the normality assumption. For equal variance, we can plot observed error versus predictor. If variance of noise is equal for different variance predictor, it should not have pattern. In our model, noise variance is smaller for houses with big numbers of rooms. Hence, assumption of equal variance is also violated.

---



# **Useful Code snippets**

> sort_index(): Sorts dataframes, series

> sample(x, replace=true): This function of pandas does random sampling on a population. x is the number of samples required. Replace parameter is set to true for sampling with replacement and set to false for sampling without replacement.

> shape(): Returns number of rows and columns.

> mean(): Mean of sample/population.

> std(ddof=1): Standard deviation of sample/population.

> var(ddof=1): Variance of sample/population
