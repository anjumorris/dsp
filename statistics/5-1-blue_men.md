[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> ```python
>> import numpy as np
>> import scipy.stats
>> %matplotlib inline
>> %config IPCompleter.greedy=True
>> ```
>>
>> ```python
>> mu = 178
>> sigma = 7.7
>> dist = scipy.stats.norm(loc=mu, scale=sigma)
>> 
>> ```
>>
>> ```python
>> h1 = 177.8 #5'10= 177.8 cm
>> h2 = 185.4  #6'1 = 185.4 cm
>> P1 = scipy.stats.norm.cdf(h1,loc=mu,scale=sigma)
>> P2 = scipy.stats.norm.cdf(h2,loc=mu,scale=sigma)
>> ```
>>
>> ```python
>> per_blue_man_range=P2-P1
>> per_blue_man_range
>> ```
