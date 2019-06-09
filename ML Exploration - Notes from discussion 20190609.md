ML Exploration - Notes from Discussion 20190609
--------------------------

#### Participants:
- Nathan Leiby, Paul Leiby

### Agenda
1. [x] [Recurrent Neural Networks - Mihail Eric](https://www.mihaileric.com/posts/recurrent-neural-networks/) May 2019
2. [x] [Basics of Support Vector Machines - Mihail Eric](https://www.mihaileric.com/posts/support-vector-machines/) April 2019
3. [x] [Introduction to Statistical Learning - With Applications in R](http://www-bcf.usc.edu/~gareth/ISL/) 2014 Chapter 9 on SVM [PL]
4. Admin

### Recurrent Network
- Q: can we get a better understanding of the basis of the "problem called vanishing gradients?"
- Recurrent has feedback of prior state variable $S_{t-1}$, leading to a "Koyck Lag" type difference equation

$$S_t = F(U X_t + W S_{t-1})$$

- This 1st order lagged difference equation implies a repeated compostion of the function F on previous observations. I.e., n compositions of F  for the nth-lagged observation $X_{t-n}$. 

$$S_t = F(U X_t + W (F(U X_{t-1} + W S_{t-2}))$$

If F is linear, doesn;t this also imply an infinite, but geometrically declining weighted history or all previous observations *X*? Something like:
$$S_t = F(U X_t + \sum_{i=1}^{\inf} W^i (F(U X_{t-i}))$$

### SVM
- interesting issues relate to the meaning and role of the Kernal (James et al. ISL says kernel is a generalized similarity measure for pairs of observations).
- interesting treatment of margin-violating (and even separating plane-violating) observations
- nice discussion in James et al. ISL Chap. 9.

### Discussion Topics
- Mechanics of ML discussion
  1. Identifying topics and selecting priorities for discussion
  2. Repository of notes, other files?
  3. Agreed tool set (code/environment) for experimentation (Python + ??? ), or different paths (Python/xxx and R/RStudio)

- Q: What is difference between feedforward and recurrent networks, and when to use each?

### Next Call and Topic: 
- 6/16/2019, 1 pm ET
- Topic: SVMs and exercises in ISL Chapter 9

### References of Interest

#### Time Series Analysis

- [How (not) to use Machine Learning for time series forecasting: Avoiding the pitfalls](https://towardsdatascience.com/how-not-to-use-machine-learning-for-time-series-forecasting-avoiding-the-pitfalls-19f9d7adf424) Jun 6, 2018
- [3 reasons to add deep learning to your time series toolkit](https://www.oreilly.com/ideas/3-reasons-to-add-deep-learning-to-your-time-series-toolkit) February 26, 2019
