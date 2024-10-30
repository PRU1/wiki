# Lecture Notes
- given a data set and it is organized as pairs
$$\mathcal{D}_{n} = \{(x^{(1)},y^{(1)}), (x^{(n)},y^{(n)})\}$$
- think of each $x$ as an input and each $y$ as an output
- learn a relationship that given an $x$, you can predict $y$
- called supervised because we are given question answer pairs
$$x^{(i)} \in \mathbb{R}^{d}, y^{(i)} \in \{+1,-1\}$$
we got to think of a representation of data
there's something called feature representation
- i.e. take a song and turn it into a numbers ($\mathbb{R}^{d}$)
# Reading Notes
classification problem: binary output is called binary; otherwise called *multi-class*
goal of classification problem; if given some new input value $x^{(n+1)}$, predict the value of $y^{(n+1)}$

## Unsupervised Learning
does not deal with creating a function that maps inputs to outputs based on input-output pairs. Give it a data set and it's supposed to find patterns in it

### Density estimation
- describe some set of data as a probability distribution
- "give samples $x^{(1)},...,x^{(n)} \in \mathbb{R}^D$, drawn IID" --> IID means (independent and identically distributed) for some distribution $\textrm{Pr}(X)$, the goal is to predict $\textrm{Pr}(x^{(n+1)})$
### Dimensionality Reduction
Given samples $x^{(1)},...,x^{(n)}\in \mathbb{R}^D$, represent them as points in $d$ dimensional space, where $d<D$.
Goal is to retain information in a data set that's difficult to compute in higher dimensions.

### Clustering
In a data set $x^{(1)},...,x^{(n)}\in \mathbb{R}^D$, you have to split the samples into similar groups. You sometimes use clustering as a first step in density estimation

## Reinforcement Learning
map input some input $x$ to its output $y$
![[Pasted image 20240308104322.png]]

## Sequence Learning
map input sequence ($x_0,...,x_n$) to output sequence $y_1,...,y_m$
 