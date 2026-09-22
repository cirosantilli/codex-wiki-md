<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the convention $\mathbb E e^{sX}\leq e^{\sigma^2s^2/2}$ for the centered [sub-Gaussian random variable](../../../../../../sub-gaussian-distribution.md). Applying the two-sided [Chernoff bound](../../../../../../chernoff-bound.md) to $X$ gives $\mathbb P(|X|>x)\leq2e^{-x^2/(2\sigma^2)}$. Since $\mathbb E X^2\geq0$, this already supplies the requested bound:

$$
\boxed{\mathbb P(X^2-\mathbb E X^2>t)\leq\min\{1,2e^{-t/(2\sigma^2)}\},\qquad t>0.}
$$

For averages of [independent random variables](../../../../../../independent-random-variables.md), the stronger useful statement is that the [centered square of a sub-Gaussian random variable](../../../../../../centered-square-of-a-sub-gaussian-random-variable.md) is a [sub-exponential random variable](../../../../../../subexponential-distribution-light-tailed.md). The [Bernstein bound for independent sub-exponential variables](../../../../../../bernstein-bound-for-independent-sub-exponential-variables.md) then give $\mathbb P(n^{-1}\sum_i(X_i^2-\mathbb E X_i^2)>t)\leq2\exp[-c n\min\{t^2/\sigma^4,t/\sigma^2\}]$ for a universal positive $c$. These are the concentration theorems used for quadratic [scan statistics](../../../../../../scan-statistic.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
