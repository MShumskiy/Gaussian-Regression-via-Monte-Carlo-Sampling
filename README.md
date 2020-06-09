# Gaussian Regression via Monte Carlo Sampling
#### Gaussian Regression via Monte Carlo Sampling.  A different method for extracting values of a gaussian distribution.

## Problem  
This problem arose from a need to calculate the width of a laser spectrum after it passes through an interference filter multiple
times.
I needed to calculate whether it's width would be shortened after multiple passes. Through simple graphical analysics I could not 
see if it was happening or not. To overcome this problem I needed to find a regression. Once I had the regression and
the equation of the curve, I would be able to access whether it's width was shorterened or not.  
To find the regression I decided to use pseudo random numbers to extract the equation of a normal distribution that fits the lab
data and also gives me full control over the precision of the fit curve.  

## Method  
### Benefits of this method  
- Easy to implement;
- Fast to calculate;
- Fully controlled precision;
- Gives the precision of the method.  
### Procedure  
This method consists of 7 steps:  
1. Import excel data into python readable data;  
2. Transform data into probabilistic data using normalization;
3. Draw *m* samples, each of size *n*, of the probabilistic data;
4. For each sample calculate its average and standard deviation;
5. Store these values in a list of average values and in a list of stadard deviations;
6. Now that we can apply *Central Limit Theorem*, calculate the average value of each of the previously mentioned lsits;
7. For each case, calculate the confidence interval.  

The code itself is well documented and explains every step, as well as the mathematical explanation.
  

