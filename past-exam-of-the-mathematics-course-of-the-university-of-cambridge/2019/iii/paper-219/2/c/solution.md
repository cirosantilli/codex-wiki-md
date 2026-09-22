<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For arbitrary nonnegative raw weights $W_i$, let $\bar W=K^{-1}\sum_iW_i$. The empirical squared [coefficient of variation](../../../../../../coefficient-of-variation.md), using variance divisor $K$, is

$$
\widehat{\operatorname{CV}}^2(W)
=\frac{K^{-1}\sum_i(W_i-\bar W)^2}{\bar W^2}
=\frac{K\sum_iW_i^2}{(\sum_iW_i)^2}-1.
$$

Substitution into the stated definition gives the usual [effective sample size of importance sampling](../../../../../../effective-sample-size-of-importance-sampling.md)

$$
\boxed{\widehat{\operatorname{ESS}}
=\frac{(\sum_iW_i)^2}{\sum_iW_i^2}.}
$$

For normalized weights $w_i=W_i/\sum_jW_j$, this reduces to $\boxed{\widehat{\operatorname{ESS}}=1/\sum_iw_i^2}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
