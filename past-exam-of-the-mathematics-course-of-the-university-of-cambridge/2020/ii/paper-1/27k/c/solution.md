<h1 id="27k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\mu_f=\int_0^1f\,d\lambda$. Subtracting this constant does not affect [variance](../../../../../../variance-split.md), and [pairwise independent random variables](../../../../../../pairwise-independent-random-variables.md) have zero pairwise covariance. Therefore

$$
\begin{aligned}
D(f)
&=\operatorname{Var}\left(\frac1n\sum_{i=1}^nf(Z_i)\right)\\
&=\frac1{n^2}\sum_{i=1}^n\operatorname{Var}(f(Z_i))
=\boxed{\frac{\operatorname{Var}(f)}n}.
\end{aligned}
$$

Only pairwise independence is needed for the off-diagonal covariance terms to vanish.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27K](../../27k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
