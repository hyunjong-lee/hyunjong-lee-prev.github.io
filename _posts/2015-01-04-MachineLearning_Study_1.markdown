---
layout: post
title:  Machine Learning Chapter 1
date:   2015-01-04 15:23:00
categories: Study
---

약 한달간 [Pattern Recognition and Machine Learning] (이하 PRML) 을 읽고 있는데 1장을 한번 보는데도 꽤 시간이 걸렸습니다.
Introduction 챕터인데도 다루는 주제가 광범위하고 깊은 것 같습니다. 저자이신 [Bishop] 님은 정말 천재의 지니어스인 것 같습니다.
이렇게 방대한 분량을 정리하시다니 -_-; 수학의 정석 이후로 이렇게 정리 잘 되어있는 수학책은 처음봅니다. 인간의 범주를 한참 벗어나신듯.

1장에서 본 **주요 키워드 - 대략 60개 -**만 나열해보면 다음과 같습니다.

## Keywords ##

  * **training set**: 모델의 파라메터 학습을 위해 훈련에 사용하는 데이터
  * **test set**: 훈련된 파라메터가 올바른지 테스트 하기 위해 사용하는 데이터
  * **feature extraction**: preprocessing 단계이며 주어진 데이터를 다른 공간으로 변형시키는 걸 의미

### Supervised Learning ###

* training set과 그에 대응하는 목표값도 같이 알 경우 [지도 학습] 방법을 적용
* **classification**: 유한한 갯수의 class에 대해서 주어진 데이터가 어떤 class에 속하는지 예측하는 것을 classification problem이라 부름
* **regression**: 실수와 같이 유한한 클래스로 제한할 수 없는 데이터에 대해 예측하는 것을 regression problem이라 부름
  
### Unsupervised Learning ###

* training set이 주어져 있지만 대응하는 목표값이 주어지지 않을 때 [자율 학습] 방법을 적용
* **clustering**: 비슷한 특징을 보이는 데이터를 그룹화
* **density estimation**: 데이터의 분포를 파악
  
### Reinforcement Learning ###

* [강화 학습]은 주어진 환경에서 어떤 행동을 취해야 보상을 최대화 할 수 있을지 찾아내는 방법
* 에이전트가 어떤 행위를 하였을 때 그에 대응하는 보상의 피드백으로 최적화 된 행동을 찾아가는 학습 방법, 하지만 이 책은 다루지 않는다!

### Polynomial Curve Fitting ###

* Goal is to achieve good generalization by making accurate predictions for new data
* random noise
* polynomial function
* linear model
* error function
* RMSE (root-mean-square-error)
* model complexity
* over-fitting
* maximum likelihood
* Bayesian approach, Bayesian model
* Regularization
* shrinkage
* ridge regression, weight decay
* validation set, hold-out set

### Probability Theory ###

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

### Model Selection ###

 * validation set
 * cross-validation
 * leave-one-out
 * information criteria
 * AIC (Akaike information criteria)
 * BIC (Bayesian information criteria)

### The Curse of Dimensionality ###

### Decision Theory ###

* decision boundaries, decision surfaces
* loss function, cost function
* loss matrix
* reject option
* inference stage, decision stage
* discriminant function
* three distinct approaches to solving decision problem
* generative models: solve inference problem for each class individually + infer prior class probabilities, then use Bayes' theorem
* discriminative models: solve inference problem of posterior class probabilities directly
* find a function f(X), called a discriminant function
* outlier detection, novelty detection
* naive Bayes model
 
### Information Theory ###
 
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
[지도 학습]: http://ko.wikipedia.org/wiki/%EC%A7%80%EB%8F%84_%ED%95%99%EC%8A%B5
[자율 학습]: http://ko.wikipedia.org/wiki/%EC%9E%90%EC%9C%A8_%ED%95%99%EC%8A%B5_(%EA%B8%B0%EA%B3%84_%ED%95%99%EC%8A%B5)
[강화 학습]: http://ko.wikipedia.org/wiki/%EA%B0%95%ED%99%94_%ED%95%99%EC%8A%B5