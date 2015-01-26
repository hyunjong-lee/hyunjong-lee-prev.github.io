---
layout: post
title:  Machine Learning Study Chapter 1
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
: $$ p(x) = \sum_{Y} p(X, Y) $$

product rule
: $$ p(X, Y) = p(Y|X)p(X) $$

$$
\begin{align*}
 posterior \propto likelihood \times prior
\end{align*}
$$



> Model Selection

> The Curse of Dimensionality

> Decision Theory

> Information Theory


$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

[Pattern Recognition and Machine Learning]: http://www.amazon.com/Pattern-Recognition-Learning-Information-Statistics/dp/0387310738
[Bishop]: http://en.wikipedia.org/wiki/Christopher_Bishop