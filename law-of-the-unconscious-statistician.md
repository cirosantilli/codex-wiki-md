# Law of the unconscious statistician

↑ **Parent:** [Expected value](expected-value.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Law_of_the_unconscious_statistician)

The [law of the unconscious statistician](law-of-the-unconscious-statistician.md) computes the [expected value](expected-value.md) of a [measurable function](measurable-function.md) of a [random variable](random-variable-split.md) directly from the original [probability distribution](probability-distribution.md). If $g(X)$ is an [integrable random variable](integrable-random-variable.md), then

$$
\mathbb E[g(X)]=\int_{\mathbb R}g(x)\,d\mu_X(x).
$$

Use $\sum_xg(x)p_X(x)$ for a [probability mass function](probability-mass-function.md), or $\int_{\mathbb R}g(x)f_X(x)\,dx$ for a [probability density function](probability-density-function.md). There is no need to derive the [probability distribution](probability-distribution.md) of $g(X)$ first. The identity is the integration rule for a [pushforward measure](pushforward-measure.md), and also holds with an infinite value when $g$ is nonnegative. [Tsitsiklis, Introduction to Probability, Lecture 5: the expected value rule](https://ocw.mit.edu/courses/res-6-012-introduction-to-probability-spring-2018/pages/part-i-the-fundamentals/).

For $X$ taking $-1,2,8$ with [probabilities](probability.md) $1/2,3/10,1/5$, choosing $g(x)=x^2$ gives $\mathbb E[X^2]=\tfrac12+4\tfrac3{10}+64\tfrac15=14.5$. Its [variance](variance-split.md) is therefore $14.5-1.7^2=11.61$. Squaring the [expected value](expected-value.md) would instead give $2.89$, because squaring does not commute with averaging.

## ↑ Ancestors (6)

1. [Expected value](expected-value.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Law of the unconscious statistician](law-of-the-unconscious-statistician.md)
- [Linearity of expectation](linearity-of-expectation.md)
