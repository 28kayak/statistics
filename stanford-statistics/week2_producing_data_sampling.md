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
Since the sample is drawn at random, the estimate will be different from the parameter due to **chance error**.
Drawing another sample will result in a different chance error. 
```
estimate = parameter + bias + chance error
```
The chance error (sampling error) will get smaller as the sample size is bigger.
Moreover, we can compute how large the chance error will be.

This is not the case for the bias (systematic error): 
Increasing the sample size just repeats the error on a larger scale, and typically we don't know how large the bias is.

## Observation vs. Experiment, Confounding, and the Placebo Effect
### Observational Studies 
> People who eat read meat have higher rates of certain cancers than people who don't eat read meat.

- this means that there is an <mark>association</mark> between red meat consumption and cancer:

    There is a link between these two.

- This does <mark>NOT</mark> mean that eating read meant *causes* a cancer: 
    People who don't eat red meat are known to exercise more and drink less alcohol, and it could be the latter two isues that cause the difference in cancer rate.

This is an **observational study**: It measures outcomes of interest and this can be used to establish asociation.

But, **association is not causation**, because there maybe **confounding factors** such as exercise that are associated both with red meat consumption and cancer.

### Randomized Controlled Experiments 
To establish causation, an **experiment** is required:
A **treatment** (e.g. eating red meat) is *assigned* to poeple in the **treatment gorup** but not to people in **contorl group**. 

Then, the outcomes in the two groups are compared.
To rule out confounders, both groups should be similar, apart from the reatment.
To this end:
- The subjects are assigned into treatment group and control group at **random**.
- When possible, subjects in the control group get a **placebo**: it resembles the treatment but is neutral.
    Assigning a placebo makes sure that both groups are equally affected by the **placebo effect**: the idea of being treated may have an effect by itself.

- The experiment is **double-blind**: neither the subjects nor the evaluators know the assignments to treatment and control.

### The placebo effect
The placebo effect is still not fully understood and is one of the most interesting phenomena in science. 

## The Logic of Randomized Controlled Experiments

Randomization serves two purpose:
- It makes the treatment gorup similar to the control group.
    Therefore, influences other than the treatment operate equally on both groups, apart from differences due to chance.
- It allows to assess how relevant the treatment effect is, by calculating the size of chance effects when comparing the outcomes in the two groups.