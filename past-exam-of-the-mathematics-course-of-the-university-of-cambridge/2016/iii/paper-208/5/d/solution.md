<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The printed identity needs an expectation on its right-hand side. For fixed $r\geq1$, condition on $X_2,\ldots,X_r$ and use [independence](../../../../../../independent-random-variables.md) of $X_1$:

$$
\boxed{P(S_r\leq x)=E\left[F\left(x-\sum_{i=2}^rX_i\right)\right].}
$$

The expression inside this expectation is generally random and cannot equal the unconditional probability by itself.

For each independent [Monte Carlo method](../../../../../../monte-carlo-method.md) replicate, draw $R_j$ from its given distribution. If $R_j=r\geq1$, draw $r-1$ independent $F$-variables, form $W_j=\sum_{i=2}^rX_{j,i}$ and set $H_j=F(x-W_j)$. For $r=1$ the empty sum is $0$. If $R$ may equal zero, use $H_j=\mathbf1_{\{x\geq0\}}$ when $R_j=0$, since $S_0=0$. The [law of total expectation](../../../../../../law-of-total-expectation.md) gives

$$
\boxed{\widehat l_N=N^{-1}\sum_{j=1}^NH_j,\qquad E\widehat l_N=P(S_R\leq x).}
$$

Since $0\leq H_j\leq1$, the estimator has [statistical consistency](../../../../../../consistency-statistics.md) by the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md). It is the [conditional Monte Carlo](../../../../../../conditional-monte-carlo.md) estimator obtained by [Rao-Blackwellization](../../../../../../rao-blackwellization.md) of the direct indicator $\mathbf1_{\{S_R\leq x\}}$, and the [law of total variance](../../../../../../law-of-total-variance.md) gives $\operatorname{Var}(H_j)\leq l(1-l)$.

This version assumes that the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) $F$ can be evaluated. An easy sampler alone does not automatically supply an easy [cumulative distribution function](../../../../../../cumulative-distribution-function.md) evaluation. If only sampling is available, use the direct indicator estimator, or replace each conditional [cumulative distribution function](../../../../../../cumulative-distribution-function.md) by the average of several independent indicators $\mathbf1_{\{X_{j,1,k}\leq x-W_j\}}$; the nested version remains an [unbiased estimator](../../../../../../unbiased-estimator.md). With $L$ such inner draws its [variance](../../../../../../variance-split.md) per outer replicate is $\operatorname{Var}(H_j)+L^{-1}E[H_j(1-H_j)]$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
