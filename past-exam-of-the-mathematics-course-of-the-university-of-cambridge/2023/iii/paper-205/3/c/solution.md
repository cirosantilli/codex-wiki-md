<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Two applications of the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
\left|\frac1n\sum_iF_iG_i\varepsilon_i\xi_i\right|
\leq
\left(\frac1n\sum_iF_i^2G_i^2\right)^{1/2}
\left(\frac1n\sum_i\varepsilon_i^2\xi_i^2\right)^{1/2}
\xrightarrow{p}0
$$

and

$$
\frac1n\sum_i|\varepsilon_iF_i|G_i^2
\leq
\left(\frac1n\sum_iF_i^2G_i^2\right)^{1/2}
\left(\frac1n\sum_i\varepsilon_i^2G_i^2\right)^{1/2}
\xrightarrow{p}0.
$$

Here the empirical residual second moment is again $O_p(1)$ by the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md), while the assumed product error and the conclusion of part b are $o_p(1)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
