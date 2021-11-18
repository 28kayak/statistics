
# Descriptive Statistics Importance 
## Example 
In January 1986, the spcae shuttle Challenger broke a part shortly after liftoff. 
The accident was caused by a part that was not desgined to fly at the unusually cold temperature of 29 degree in F at launch.
Here are the launch-temperatures of the first 25 huttle missions (in degree F):


```
66,70,69,80,68,67,72,70,70,57,63,70,78,67,53,67,75,70,81,76,79,75,76,58,29
```
```python
import seaborn as sns
import pandas as pd
import numpy as np

temp = [66,70,69,80,68,67,72,70,70,57,63,70,78,67,53,67,75,70,81,76,79,75,76,58,29]
# Plot the histogram thanks to the distplot function
sns.distplot( a=temp, hist=True, kde=False, rug=False )
```

![distplot_1.png](https://raw.githubusercontent.com/28kayak/statistics/main/stanford-statistics/img/distplot_1.png)

As seeing the hist graph, we could quickly figure out that `29F is extremly cold temperature`
## the 2 most important functions of descriptive statistics 
- Communicate information
- Support reasoning about data

---
# Pie Chart, Bar Graph, and Histograms 
## Graphical Summaries of Data
It is the best to use graphical summary to communicate information, because people prefer to look at pictures rather than at numbers.
There are many ways to visualize data.
The nature of the data and the goal of the visualization determine which method to choose.
### Qualitative Data (i.e. colors, car types, ...)
#### Pie Chart
  - each slice represents percentage.
  - pie chart allows more easily to eyeball what fraction of the total a category corresponds to.

#### Dot Plot  
  - the position of the dot corresponds to the percentage.
    - x-axis represents percent
    - y-axis represents categories 
  - dot plot makes it easier to compare frequencies of various categories 

### Quantitative (i.e numbers) 
#### Histogram
- if the data are quantitative, then they should be put on a number line 
- the ordering and the distance between the numbers convey important information. 
- `bar graph` is essentially a dot plot put on its side.
- `histogram` allows to use blocks with different width.
  - Key Point: the areas of the blocks are propotional to frequency
  - the total area = 100% 
  - it is helpful to have a vertical scale (density scale)
    - its unit is `% per unit` 
  - `histogram` gives two kinds of information about the data
    - `Density(Crowding)`: the height of the bar tells how many subjects there are for one unit on the horizontal scale. 
    - EX: the hightest density is around age 19 as 0.04 = 4% of all subjects are age 19. In contrast, only about 0.7% of subjects fall into each one year range for ages 60-80.
    - `Percentage(relative frequences)`: those are given by 
    `are = height * width`
    - EX: about 14% of all subjects fall into the age range 60-80, ebcause the corresponding area is `(20years)*(0.7% per year)=14%`
    - Alternatively, you can find this answer by eyeballing that this area makes up roughly 1/7 of the total area of histogram. So, roughly 1/7 = 14% of all subjects fall in that range. 

For histogram, it is very important to select `interval` for ractangles. 
#### Method 1
if you have n data in your dataset,
$interval = \sqrt{n} $
#### Method 2
if you have n data in your dataset, 
$interval = 1 + \frac{\log_{10} n}{\log_{10} 2} $

--- 
# Box-and-Whisker Plot and Scatter Plot
boxplot (i.e. box-and-whisker plot)
the box plot depicts five key numbers of data

![boxplot_1](https://raw.githubusercontent.com/28kayak/statistics/main/stanford-statistics/img/boxplot_1.png)

--- 

When the histogram is skewed to the right, then the mean can be much larger than the median.
So, if the histogram is very skewed, then use the median.
#### theoritical example
if the median sales price of 10 homes is 1 doller million, then we know that 5 homes sold for 1 doller million or more.
if we sold that the average sales price is 1 doller million, then we can't draw such a conclusion

if average is 1 doller million, the sume of the 10 sales price is 10 doller million.
Let's assume that 1 house sold for 8 doller million.
Then the total of sales price of other 9 houses is 2 doller million.
The average of the other 9 houses is 2 million doller / 9 = 200,000

if we think that the average of sales price of 1 doller million means that most houses sold for roughly 1 doller million.
--> it does not make sence.
### Percentile 
The 90th percentile of incomes is $135,00
90% of households report an icome of $135,000 or less, and 10% report more.

The 75th percentile is called `3rd quartile`:  $85,000.

The 50th percentile is called `median` (also `2nd quartile`) : $50,000

The 25th percentile is called `1st quartile`

---
# Percentile, the Five Number Summery, and Standard Deviation
## Five-number Summary
Recall that the boxplot gives a five number summary of data:
- the smallest number (lower wisker)
- 1st quartile
- median
- 34d quartile 
- the largest number
![interquartile_range.png](https://raw.githubusercontent.com/28kayak/statistics/main/stanford-statistics/img/interquartile_range.png)

The interquartile range = 3rd quartile - 1st quartile
It measures how spread out the data are. 

## The standard deviation
A more commonly used measure of spread is the `standard deviation`. 

$\bar{x}$ stands for the average of the numbers  $ x_1, x_2, ... x_n$

The standard deviation of these numbers is:

$s = \sqrt{\frac{1}{n} \sum_{i=1}^{n}(x_i - \bar{x})^2}$

OR

$s = \sqrt{\frac{1}{n-1} \sum_{i=1}^{n}(x_i - \bar{x})^2}$

The two numbers $\bar{x}$ and $s$ are often used to summarize data.
Both are sensitive to a few large or small data.
If that is concern (i.e. the histgram is skewed), then it is better to use the `median` and the `interquartile range`.  

--- 
# [EXTRA] Industry Insight: Introduction to Abdrew Radin


