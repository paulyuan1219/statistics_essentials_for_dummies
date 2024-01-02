# 02 Descriptive Statistics

# 03 Charts and Graphs

## Categorical Data
- Pie Charts
- Bar Graphs
  - It breaks categorical data down by group
  - often used to compare groups by breaking down the categories for each and showing them as side-by-side bars.
- Time Charts

## Numerical Data
- Histograms
  - it is a bar graph applying to numerical data
  - it provides a snapshot of all the data broken down into numerically ordered groups.
  - it provides a quick way to get the big idea about a numerical data set.
- Boxplots

## How to interpret a histogram or boxplot
- data distribution
  - symmetric
  - skewed right: a lopsided mound with one long tail going off to the right
  - skewed left
- data variability
- data center 


# 04 The Binomial Distribution



# 05 The Normal Distribution
If n is large enough, then we can use a normal distibution to approximate the binomial distribution

The following two conditions must hold
- np >= 10
- n(1-p) >= 10

# 06 Sampling Distributions and the Cebtral Limit Theorem

## Charactristics of a sampling distribution

- For the whole population
  - mean of the population
  - standard deviation of a population
- For a sample mean $\bar{X}$
  - mean of the sample mean
    - $u_{\bar{x}} = u_{x}$ 
  - standard error of a sample mean. 
    - Error here doesn't mean there's been a mistake. It means that there is a gap between the population and sample results.  
    - $\sigma_{\bar{x}} = \frac{\sigma_x}{\sqrt{n}}$ 
- Shape
  - If X's distribution is normal, so is $\bar{X}$
  - If X's distribution is unknown or not normal, we can approximate $\bar{x}$ via a normal distribution if the sample size is large enough. 

## Finding Probabilities for $\bar{X}$
- $Z = \frac{\bar{X} - u_{\bar{x}}}{\sigma_{\bar{x}}} = \frac{\bar{X} - u_{\bar{x}}}{\frac{\sigma_x}{\sqrt{n}}}$ 

## The Sampling Distribution of the Sample Proportion

The CLT doesn't apply only to sample means. You can also use it with other statistics, including sample proportions.

- Population proportion: $p$
- Sample proportion: $\hat{p}$
  - its mean is $p$
  - its standard error is $\sqrt{\frac{p(1-p)}{n}}$
  - its shape is approximately normal, given that the sample size is large enough.
  - the larger the sample size, the closer to a normal distribution
    - $np >=10$
    - $n(1-p) >= 10$

## Finding Probabilities for $\hat{p}$
- $Z = \frac{\hat{p} - p}{\sqrt{\frac{p(1-p)}{n}}}$

# 07 Confidence Intervals

## Definition of a confidence interval (CI)
- A confidence interval is used for the purpose of estimating a population parameter (a single number that describes a population) by using statistics (numbers that describe a sample of data).
- For example, you may estimate the average household income (parameter) based on the average household income from a random sample of 1,000 homes (statistic).
- However, because sample results will vary, you need to add a measue of that variability to your estimate.
- This measure of variability is called **the margin of error**, the heart of a confidence interval.
- Your sample statistic, plus or minus your margin of error, gives you a range of likely values of the parameter, in other words, a confidence interval.

The margin of error is not the chance a mistake was made; it measures variation in the random sampls due to chance. Because you didn't get to sample everybody in the population, you expect your sample results to be "off" by a certain amount, just by chance.

## How to estimate a parameter with a confidence interval:

1. Choose your confidence level and your sample size (see details later in this chapter).
2. Select a random sample of individuals from the population.
3. Collect reliable and relevant data from the individuals in the sample.
4. Summarize the data into a statistic (for example, a sample mean or proportion).
5. Calculate the margin of error. (Details later in this chapter.)
6. Take the statistic plus or minus the margin of error to get your final estimate of the parameter. This is called a confidence interval for that parameter.


## The Goal: Small Margin or Error

The ultimate goal when making an estimate using a confidence level is to have a small margin of error. The narrower the interval, the more precise the results are.

### Three factors affect the size of the margin of error. 
- The confidence level
- The sample size
- The amount of variability in the population.


Please note that the sample statistic itself isn't related to the width of the confidence interval. The statistic only determines the midpoint of the confidence interval, not its width. 

## Choosing a Confidence Level

Variability in sample statistics is measured in standard errors. A **standard error** is very similar to the standard deviation of a data set or a populatio. The difference is that the standard error measues the variation among all possible values of the statistic while A standard deviation of a population measures the variation among all possible values within the population itself. 

The **confidence level** of a confidence interval corresponds to the percentage of the time your result will be correct if you took numerous random samples. 

When working with means and proportions, if the proper conditions are met, the number of standard errors to be added and subtracted for a given confidence level is based on the standard normal distribution, and is labelled $z^*$. 

## Factoring in the Sample Size
The relationship between margin of error and sample size is simple. As the sample size increases, the margin of error decreases.

Recall the formula for standard error for the sample mean: $\sigma_{\bar{x}} = \frac{\sigma_x}{\sqrt{n}}$ . As $n$ increases, $\sigma_{\bar{x}}$ decreases, so does the margin of error $z*\frac{\sigma_x}{\sqrt{n}}$.
- Goal: to get a smaller margin of error
- $z$ is large when high confidence interval is required.
- if $n$ is large enough, it can offset the impact of $z$ to keep the margin of error small


Before starting a study, you can determine the sample size you need to achieve a certain margin of error.

When estimating a population mean, try this sample size formula: ![](https://www.dummies.com/wp-content/uploads/250707.image0.jpg)

In this formula, MOE represents the desired margin of error (which you set ahead of time), and σ represents the population standard deviation.  z* is the critical value for the confidence level you need.

If σ is unknown, you can estimate it with the sample standard deviation, s, from a pilot study. In this case, you would use the appropriate value of the t-distribution with $n-1$ degees of freedom, rather than $z^*$. 

when your statistic is a sample proportion or percentage (such as the proportion of femails, or the percentage of semis), a quick-and-dirty way to figure margin of error is to take 1 divided by the square root of n (the sample size).

For example, consider what sample size is needed to have a narrow confidence interval with respect to polls. 
- A survey of 100 people will have a margin of error of about $\frac{1}{\sqrt{100}} = 0.10$, or 10%
- A survey of 1000 people will have a margin of error of about $\frac{1}{\sqrt{1000}} = 0.03$, or 3%
- A survey of 2500 people will have a margin of error of about $\frac{1}{\sqrt{2500}} = 0.02$, or 2%
- A survey of 5000 people will have a margin of error of about $\frac{1}{\sqrt{5000}} = 0.014$, or 1.4%


The following table shows formulas for the components of the most common confidence intervals and keys for when to use them.

![](https://www.dummies.com/wp-content/uploads/250709.image0.jpg)

## Interpreting Confidence Intervals

The big idea of a confidence interval is that it presents a range of likely values for the population parameter, based on one random sample, with a certain confidence level (such as 95%).

Now coems the subtle but very important point rgarding how to interpret a confidence interval. When one particular confidence interval is calculated, **do not** include a probability statement about your particular result when you draw your conclusions. That is, it's wrong to say "I am 95% confident that the populartion mean is between XXX and YYY". Once your sample has been selected and your confidence interval is calculated, it either contains the population parameter or it doesn't; there is no probability involved.

Bottom line: The confidence level (in this case, 95%) doesn't apply to a single confidence interval.

Let's revisit the definition of a confidence level. A **confidence level** is the percentage of all possible samples of size n whose confidence intervals contain the population parameter. When taking many random samples form a population, you know that some samples (in this case, 95% of them) will epresent the population, and some won't (in this case, 5% of them) just by random chance. Random samples that represent the population will results in conficdence interals that contian the population parameter ( that is, they are correct); and those that do not represent the population will result in confidence intervals that are not correct.

Confidence level (such as 95%) represents the percentage of all possible random samples of size n that typify the population and hence results in correct confidence intervals. It is not the probability of  a single confidence interval being correct..

Another way of thinking about the confidence level is to say that if the organization took a sample of 1000 people over and over again a and made a confidence interval from its results each time, 95% of those confidence intervals wiould be ight. (You just have to hop that yours is one of those right results.).

To corectly interpret your particular confidence interval you can say "A range of likely values for the populariton mean is XXX to YYY, with a confidence level of 95%.". Alternatively, you can say, "For these results, one can say with 95% confidence that the maximum amount of sample (margin of ) error is plus or minux XXX."

**It's all about the sampling process, not a single sample.**


# ch08 Hypothesis Tests
Hypothesis testing is a statistician's way of trying to confirm or deny a claim about a **population** using data from a **sample**.

## General steps for a hypothesis test
1. Set up the null and alternative hypotheses: H_0 and H_a
2. Take a random sample of individuals from the population and calculate the sample statistics (means and standard deviations).
3. Convert the sample statistic to a test statistic by chaning it to a standard score .
4. Find the p-value for your test statistic.
5. Examine your p-value and make your decision.


![](https://www.dummies.com/wp-content/uploads/250714.image0.jpg)



## Errors in Hypothesis Testing
- A false alarm: Type-1 error
  - Rejecting H_0, when you shouldn't 
  - To minimize it: set a low cutoff probability for rejecting H_0
- A missed detection: Type-2 error
  - Not rejecting H_0, when you should
  - To minimize it: select a large sample size to ensure that any differences or departures that really exist won't be missed.


# ch09 The t-Distribution

Basics of the t-Distribution
- a cousin of the normal distribution
- bell-shaped
- shorter and flatter than a normal distribution
- its standard deviation is proportionally larger compared to the Z-distribution
- degrees of freedom
  - related to the sample size of the data set
  - given a sample size of n, the DOF is n-1
  - smaller DOF means flatter
  - larger DOF means closer to the Z-distribution. When n>30, they become very close.

t-Distributions and Hypothesis Tests

The most common use by far of the t-distribution is in hypothesis testing; in particular, the case where you do a hypothesis test for one population mean. You use a t-distribution when you don't know the standard deviation of the population $\sigma$ and you have to use the standard deviation of the sample $s$ to estimate it. Typically in these situations you also have a small sample size (but not always).


# ch10 Correlation and Regression

In this chapter, you analyze two numerical variables, X and Y, to look fo patterns, find the correlation, and make pedictions about Y from X, if appropriate, using simple linear regression.

- Scatterplot
- bivariate data


## Measuring (Linear) Relationships Using the Correlation

**Correlation coefficient** meansures the strength and direction of the linear relationship between two numerical variables X and Y.

The formula for the correlation (r) is
![](https://wikimedia.org/api/rest_v1/media/math/render/svg/9363d4a765bda05563bf32c9216e3cf250ac387d)

See more details at [Pearson correlation coefficient](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient)

The correlation r is always between +1 and -1.

- The correlation is a unitless measure. This means that if you change the unites of X or Y, the correlation doesn't change.
- The variables X and Y can be switched in the dataset, and the correlation doesn't change.
- X is the explanatory variable; Y is the response variable.

The best-fitting line is $y = m*x + b$
- $m = r * \frac{s_y}{s_x}$
- $b = \bar{y} - m * \bar{x}$

The big-five statistics
- The mean of the x values (denoted $\bar{x}$)
- The mean of the y values (denoted $\bar{y}$)
- The standard deviation of the x values (denoted $s_x$)
- The standard deviation of the y values (denoted $s_y$)
- The correlation between X and Y (denoted $r$)


Correlation doesn't necessarily mean Cause-and-Effect.










# Appendix
[Statistics For Dummies Cheat Sheet](https://www.dummies.com/article/academics-the-arts/math/statistics/statistics-for-dummies-cheat-sheet-208650/)

