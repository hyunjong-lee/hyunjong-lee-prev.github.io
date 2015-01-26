---
layout: post
title:  Machine Learning Chapter 1
date:   2015-01-04 15:23:00
categories: Study
---

약 한달간 [Pattern Recognition and Machine Learning] (이하 PRML) 을 읽고 있는데 1장을 한번 보는데도 꽤 시간이 걸렸습니다.
Introduction 챕터인데도 다루는 주제가 광범위하고 깊은 것 같습니다. 저자이신 [Bishop] 님은 정말 천재의 지니어스인 것 같습니다.
이렇게 방대한 분량을 정리하시다니 -_-; 수학의 정석 이후로 이렇게 정리 잘 되어있는 수학책은 처음봅니다. 인간의 범주를 한참 벗어나신듯.

1장에서 본 주요 키워드만 나열해보면 다음과 같습니다.

> Supervised Learning

  - classification
  - regression
  
> Unsupervised Learning

  - clustering
  - density estimation
  
> Reinforcement Learning

> Polynomial Curve Fitting

* Goal is to achieve good generalization by making accurate predictions for new data
  - training set
  - test set
  - random noise
  - polynomial function
  - linear model
  - error function
  - RMSE (root-mean-square-error)
  - model complexity
  - over-fitting
  - maximum likelihood
  - Bayesian approach, Bayesian model
  - Regularization
  - shrinkage
  - ridge regression, weight decay
  - validation set, hold-out set

> Probability Theory

 * The Rules of Probability

sum rule
: \$$ p(X) = \sum_{Y} p(X, Y) $$

product rule
: \$$ p(X, Y) = p(Y \mid X) p(X) $$

$$
\begin{align*}
 posterior \propto likelihood \times prior
\end{align*}
$$

 * Gaussian distribution
 * Bayesian curve fitting

> Model Selection

 * validation set
 * cross-validation
 * leave-one-out
 * information criteria
 * AIC (Akaike information criteria)
 * BIC (Bayesian information criteria)

> The Curse of Dimensionality

> Decision Theory

 * decision boundaries, decision surfaces
 * loss function, cost function
 * loss matrix
 * reject option
 * inference stage, decision stage
 * discriminant function
 * three distinct approaches to solving decision problem
   - generative models: solve inference problem for each class individually + infer prior class probabilities, then use Bayes' theorem
   - discriminative models: solve inference problem of posterior class probabilities directly
   - find a function f(X), called a discriminant function
 * outlier detection, novelty detection
 * naive Bayes model
 
> Information Theory
 
 * entropy
 * noiseless coding theorem
 * multiplicity
 * microstate, macrostate
 * Lagrange multiplier
 * mean value theorem
 * differential entropy
 * conditional entropy
 * KL divergence, Kullback-Leibler divergence, relative entropy
 * convex function, convexity
 * strictly convex
 * concave
 * strictly concave
 * Jensen's inequality
 * mutual information

[Pattern Recognition and Machine Learning]: http://www.amazon.com/Pattern-Recognition-Learning-Information-Statistics/dp/0387310738
[Bishop]: http://en.wikipedia.org/wiki/Christopher_Bishop