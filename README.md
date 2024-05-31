# Python and statistics for Financial Analysis
This is a course done using the available Coursera free courses provided by The Hong Kong University of Science and Technology. It gives a basic unedrstanding of how to leverage Python and Statistics for financial analysis. It discusses four modules - Visualizing and Munging Stock data, Random Variables and distribution, Sampling and Interference and Linear regression models for financial analysis. It is taught by Xuhu Wan, Associate Professor, Department of Information Systems, Business Statistics and Operations Management. 

# About this Course
Course Overview: https://youtu.be/JgFV5qzAYno

Python is now becoming the number 1 programming language for data science. Due to python’s simplicity and high readability, it is gaining its importance in the financial industry.  The course combines both python coding and statistical concepts and applies into analyzing financial data, such as stock data.

By the end of the course, you can achieve the following using python:

- Import, pre-process, save and visualize financial data into pandas Dataframe

- Manipulate the existing financial data by generating new variables using multiple columns

- Recall and apply the important statistical concepts (random variable, frequency, distribution, population and sample, confidence interval, linear regression, etc. ) into financial contexts

- Build a trading model using multiple linear regression model 

- Evaluate the performance of the trading model using different investment indicators

Jupyter Notebook environment is configured in the course platform for practicing python coding without installing any client applications.

# **Notes**


> Relative frequency = Frequency / Total number of tries

> Relative frequency becomes more stable with more number of tries.

> For discrete variables, mean and variance can be calculated for probability distribution.

> For continuous variables, are under the Probability Density function determines the probability.

> VaR: Measure of how much a set of invstment might lose

> ddof=1, provides an unbiased estimator(divides by n-1) while, ddof=0 provides maximum likelihood estimato(divides by n).

> Degrees of freedom: Number of values in calculation that are free to variate.


---



# **Useful Code snippets**

> sort_index(): Sorts dataframes, series

> sample(x, replace=true): This function of pandas does random sampling on a population. x is the number of samples required. Replace parameter is set to true for sampling with replacement and set to false for sampling without replacement.

> shape(): Returns number of rows and columns.

> mean(): Mean of sample/population.

> std(ddof=1): Standard deviation of sample/population.

> var(ddof=1): Variance of sample/population
