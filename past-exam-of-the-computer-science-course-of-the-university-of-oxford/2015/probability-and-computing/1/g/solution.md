<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The [independence](../../../../../independent-random-variables.md) of $X$ and $Y$ permits factoring the [expectation](../../../../../expected-value-split.md) of the product $e^{tX}e^{tY}$. The [moment-generating function of a binomial distribution](../../../../../moment-generating-function-of-a-binomial-distribution.md) from the previous part therefore gives

$$
\begin{aligned}
M_{X+Y}(t)&=\mathbb E[e^{t(X+Y)}]
=\mathbb E[e^{tX}]\mathbb E[e^{tY}]\\
&=(1-p+pe^t)^n(1-p+pe^t)^m
=\boxed{(1-p+pe^t)^{n+m}}.
\end{aligned}
$$

This is the [moment-generating function](../../../../../moment-generating-function.md) of $B(n+m,p)$. Both [moment-generating functions](../../../../../moment-generating-function.md) are finite on a neighbourhood of zero, so the [uniqueness theorem for moment-generating functions](../../../../../uniqueness-theorem-for-moment-generating-functions.md) identifies the [probability distribution](../../../../../probability-distribution-split.md):

$$
\boxed{X+Y\sim B(n+m,p).}
$$

The common success [probability](../../../../../probability.md) $p$ and [independence](../../../../../independent-random-variables.md) are both used in this argument.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
