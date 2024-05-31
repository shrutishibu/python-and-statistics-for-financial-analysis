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

---



# **Useful Code snippets**

> sort_index(): Sorts dataframes, series

> sample(x, replace=true): This function of pandas does random sampling on a population. x is the number of samples required. Replace parameter is set to true for sampling with replacement and set to false for sampling without replacement.

> shape(): Returns number of rows and columns.

> mean(): Mean of sample/population.

> std(ddof=1): Standard deviation of sample/population.

> var(ddof=1): Variance of sample/population
