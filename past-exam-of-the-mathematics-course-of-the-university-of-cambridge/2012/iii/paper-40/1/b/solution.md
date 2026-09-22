<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [exponential distribution](../../../../../../exponential-distribution.md) of mean $\mu$, $M_X(t)=(1-\mu t)^{-1}$. Substitution into the [geometric-sum moment-generating function](../../../../../../geometric-sum-moment-generating-function.md) gives

$$
M_S(t)=\frac{p}{p-\mu t}\qquad(t<p/\mu).
$$

This is the [moment-generating function](../../../../../../moment-generating-function.md) of an [exponential distribution](../../../../../../exponential-distribution.md) with rate $p/\mu$. By the [uniqueness theorem for moment-generating functions](../../../../../../uniqueness-theorem-for-moment-generating-functions.md), the [geometric sum of exponential variables](../../../../../../geometric-sum-of-exponential-variables.md) therefore has [probability density function](../../../../../../probability-density-function.md)

$$
\boxed{f_S(s)=\frac p\mu e^{-ps/\mu}\quad(s>0),\qquad f_S(s)=0\quad(s<0).}
$$

Its [expected value](../../../../../../expected-value.md) is $\mu/p$, agreeing with $\mathbb E[N]\mathbb E[X]=\mu/p$ in the [random sum of independent claims](../../../../../../random-sum-of-independent-claims.md) formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
