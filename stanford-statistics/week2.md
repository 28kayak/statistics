# Intorduction  
## Statistical Inference 
### what is statistical inference?
> What percentage of voers approve of the way the U.S. President is handling his job?

This is difficult to determine `EXACTLY` as there are more than 250 million people of voting age in the U.S. 

However, it is not difficult to `estimate` this percentage.

Pick a sample voters at random.
Then, use the approval percentage among those voters as an estimate for the approval percentage of all voters.

### Technical Terms
<mark>Population</mark>: the entire group of subjects about which we want information.
- all U.S. voters 

<mark>Parameter</mark>: the quantity about the population we are interested in. 
- approval percentage among all U.S. voters

<mark>Sample</mark>: the part of the population from which we collect information. 
- the $N$ voters selected random

<mark>Statistic (estimate)</mark>: the quantity we are interested in as measured in the sample.
- approval percentage among the smapled voters

**Key Point**
even  a relatively small sample (100 or 1000) will produce an estimate that is close to the parameter of very larger population of 250 million subjects.

--- 
# Simple Random Sampling and Other Sampling Plans
## Sample Random Sampling and Stratified Random Sampling
### Sampling Correctly 
It's tempting to sample 1,000 voters in your hometown. 
This is a **sample of convenience**.
This is not a good way to sample because the voters will be different from the population of U.S voters.

![voter_map_us](https://raw.githubusercontent.com/28kayak/statistics/main/stanford-statistics/img/voter_map_us.png)

As you see, the Midwest tends to vote more Repulican.
On the other hand, the West Coast and the East Coast tends to be Democrates. 

This will introduce **bias**, i.e. this sampling will favor a certain outcome.

<mark>selection bias</mark>: a sample of convenience makes it more likely to smaple certain subjects then others. 

<mark>non-response bias</mark>: parents are less likely to answer a survey request at 6pm because they are busy with childrent and dinner. 

<mark>voluntary response bias</mark>: websites that post reviews of businesses are more likely to get response from customers who had very bad or very good experience. 


>Imagine you are working for a large retail company. 
You would like to see how your customers like the new product your company launched a month ago. 
Your colleague suggests that you can go to a shopping center in the weekend to collect the reviews. 
What bias(es) could result from this decision?

## Sampling Designs 
the best methods for sampling use change in a planned way:
a **simple randome sample** selects subject at random without replacement.

a **stratified random sample** devides the population into groups of similar subjects called `strata` (e.g. urban, suburban, and rural voters).
Then one chooses a simple randome sample in each stratum and combined these.

## Bias and Chance Error
