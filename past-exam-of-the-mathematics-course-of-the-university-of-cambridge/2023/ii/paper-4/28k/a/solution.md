<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume that $f(x)=0$ wherever $h(x)=0$ on the part of the space relevant to $g$. The [importance sampling](../../../../../../importance-sampling.md) algorithm draws [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) $Y_1,\ldots,Y_m$ from $h$, forms the weights

$$
w(Y_i)=\frac{f(Y_i)}{h(Y_i)},
$$

and returns

$$
\widehat\mu_m=\frac1m\sum_{i=1}^m g(Y_i)w(Y_i).
$$

A [change of measure](../../../../../../change-of-measure.md) gives

$$
\mathbb E_h[g(Y)w(Y)]
=\int_{\mathcal X}g(y)\frac{f(y)}{h(y)}h(y)\,dy
=\mathbb E_f[g(X)].
$$

**Hence the estimator is unbiased whenever the expectation exists, and, if $\mathbb E_h|g(Y)w(Y)|<\infty$, the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $\widehat\mu_m\to\mathbb E_f[g(X)]$ almost surely.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28K](../../28k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
