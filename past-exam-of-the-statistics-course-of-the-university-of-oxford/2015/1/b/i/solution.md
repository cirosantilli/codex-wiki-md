<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Continuity and strict increase make the [quantile function](../../../../../quantile-function.md) $F^{-1}$ well-defined on $(0,1)$. The endpoints of the [uniform distribution](../../../../../continuous-uniform-distribution.md) occur with [probability](../../../../../probability.md) zero and do not affect the construction. For every real $x$,

$$
\begin{aligned}
\Pr(X_i\leq x)
&=\Pr(F^{-1}(U_i)\leq x)\\
&=\Pr(U_i\leq F(x))=F(x).
\end{aligned}
$$

Thus each $X_i$ has [cumulative distribution function](../../../../../cumulative-distribution-function.md) $F$. Applying a fixed measurable function separately to [independent random variables](../../../../../independent-random-variables.md) preserves their independence; explicitly, joint lower-tail probabilities factor as

$$
\Pr(X_1\leq x_1,\ldots,X_n\leq x_n)=\prod_{i=1}^nF(x_i).
$$

Consequently

$$
\boxed{X_1,\ldots,X_n\text{ are independent and identically distributed with CDF }F.}
$$

This is [inverse transform sampling](../../../../../inverse-transform-sampling.md). Since $F^{-1}$ preserves order, it also sends the central [order statistic](../../../../../order-statistic.md) to the central [order statistic](../../../../../order-statistic.md), justifying $M_X=F^{-1}(M_U)$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
