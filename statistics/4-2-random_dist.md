[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> ```
nums = np.random.random_sample((1000,))
numspmf = thinkstats2.Pmf(nums)
thinkplot.Pmf(numspmf)
thinkplot.Config(xlabel='random number', ylabel='probability')

numscdf = thinkstats2.Cdf(nums)
thinkplot.Cdf(numscdf)
thinkplot.Config(xlabel='random number', ylabel='probability')
```
