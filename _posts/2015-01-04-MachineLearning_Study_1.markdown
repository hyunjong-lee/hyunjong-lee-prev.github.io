---
layout: post
title:  Machine Learning Study (1)
date:   2015-01-04 15:23:00
categories: Study
---

현재 [Pattern Recognition and Machine Learning](http://www.amazon.com/Pattern-Recognition-Learning-Information-Statistics/dp/0387310738)
을 읽고 있는데 Chapter 1을 곧 정리할 예정입니다.
아래는 수식 입력 테스트를 위해 latex를 붙여본 예제입니다.

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
