ML Exploration - Notes from Discussion 20190609
--------------------------

#### Participants:
- Nathan Leiby, Paul Leiby

### Agenda
1. [x] [Recurrent Neural Networks - Mihail Eric](https://www.mihaileric.com/posts/recurrent-neural-networks/) May 2019
2. [x] [Basics of Support Vector Machines - Mihail Eric](https://www.mihaileric.com/posts/support-vector-machines/) April 2019
3. [x] [Introduction to Statistical Learning - With Applications in R](http://www-bcf.usc.edu/~gareth/ISL/) 2014 Chapter 9 on SVM [PL]
4. Admin


$$S_t = F(U X_t + W S_{t-1})$$
$$S_t = F(U X_t + W (F(U X_{t-1} + W S_{t-2}))$$
$$S_t = F(U X_t + \sum_{i=1}^{\inf} W^i (F(U X_{t-i}))$$


### Discussion Topics
- Mechanics of ML discussion
  1. Identifying topics and selecting priorities for discussion
  2. Repository of notes, other files?
  3. Agreed tool set (code/environment) for experimentation (Python + ??? ), or different paths (Python/xxx and R/RStudio)

- Q: What is difference between feedforward and recurrent networks, and when to use each?

### Next Call: 
- 6/16/2019, 1 pm ET
- Topic: SVMs and exercises in ISL Chapter 9

### References of Interest

#### Time Series Analysis

- [How (not) to use Machine Learning for time series forecasting: Avoiding the pitfalls](https://towardsdatascience.com/how-not-to-use-machine-learning-for-time-series-forecasting-avoiding-the-pitfalls-19f9d7adf424) Jun 6, 2018
- [3 reasons to add deep learning to your time series toolkit](https://www.oreilly.com/ideas/3-reasons-to-add-deep-learning-to-your-time-series-toolkit) February 26, 2019

- PL SSH public key: 
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDp7Tp8LSHMhMmz0oCRZifVM2bvJ19OMkPu/cLkvYZ9WlVSbzg/qyWNTcDG+AsVnsAhmTNtjwNzZhfrsmJGOT9BR+7aYR6LalMCkRrCvjQXuAZd9+k9DOHIKCkfk9JO2PTyjNqmGrcSdmpL36me+rMjt2Shca1iEEnxrqSuK1z9S44YQegTdt0hhQxr9+k6Z/rhIYgSyKAQ6xG2O5Af9Hx6K+RFXYnVMyPrLvAHrn7HM+dJYpQU44TKkhOfw2Gb+fDt5cEAdjW4u0R33qeYca8HmaX0+ECOPgSfuagV/9/C1wkJoYvIH+fYxaNGQMfT65qs10adxD14kPr8vIbu1E9p Generated-by-Nova