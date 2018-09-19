[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> ```python
>> from __future__ import print_function, division
>> import numpy as np
>> import nsfg
>> import thinkstats2
>> import thinkplot
>> %matplotlib inline
>> %config IPCompleter.greedy=True
>> ```
>>
>> Function to generate bias copied from thinkstats2
>>
>> ```python
>> def BiasPmf(pmf, label):
>>     new_pmf = pmf.Copy(label=label)
>> 
>>     for x, p in pmf.Items():
>>         new_pmf.Mult(x, x)
>>         
>>     new_pmf.Normalize()
>>     return new_pmf
>> ```
>>
>> Reading the nsfg file
>>
>> ```python
>> resp = nsfg.ReadFemResp()
>> ```
>>
>> PMF unbiased calculated using numkdhh col
>>
>> ```python
>> num_child = resp['numkdhh']
>> pmf_num_child_unbiased = thinkstats2.Pmf(num_child, label ='Unbiased PMF')
>> pmf_num_child_unbiased
>> ```
>>
>> PMF Biased calculated using the function
>>
>> ```python
>> pmf_num_child_biased = BiasPmf(pmf_num_child_unbiased, label='Biased PMF')
>> pmf_num_child_biased
>> ```
>>
>> Calculate means of both PMFs
>>
>> ```python
>> pmf_num_child_unbiased.Mean(), pmf_num_child_biased.Mean()
>> ```
>>
>> Plotting the PMFs
>>
>> ```python
>> thinkplot.PrePlot(2)
>> thinkplot.Pmfs([pmf_num_child_unbiased,pmf_num_child_biased])
>> thinkplot.Config(xlabel ='Number of children in Household',ylabel='PMF')
>> ```
>>
>>
