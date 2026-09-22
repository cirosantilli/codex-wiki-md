<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume independent individuals and [independent censoring](../../../../../../independent-censoring.md): conditional on any modelled covariates, the censoring mechanism gives no additional information about the latent event time and has no parameter shared with its [survival distribution](../../../../../../survival-distribution.md). An observed event at $x_i$ contributes the [probability density function](../../../../../../probability-density-function.md) $f(x_i)$. A [right-censored](../../../../../../right-censoring.md) observation contributes the [survivor function](../../../../../../survival-function.md) $F(x_i)$, since it establishes only $T_i>x_i$.

More formally, let $C_i$ be an independent censoring time with density $c_i$ and [survivor function](../../../../../../survival-function.md) $G_i$. The observed pair $X_i=\min(T_i,C_i)$, $v_i=\mathbf1_{\{T_i\leq C_i\}}$ has a parameter-dependent factor $f(x_i)G_i(x_i)$ if $v_i=1$ and $F(x_i)c_i(x_i)$ if $v_i=0$. The factors involving only the censoring distribution can be omitted from the event-time [likelihood](../../../../../../likelihood-function.md). Thus

$$
L=\prod_{i=1}^n f(x_i)^{v_i}F(x_i)^{1-v_i},
\qquad
\boxed{\ell=\sum_{i=1}^n\{v_i\log f(x_i)+(1-v_i)\log F(x_i)\}.}
$$

Using $f=hF$ also gives the useful [survival likelihood](../../../../../../survival-likelihood.md) form

$$
\ell=\sum_i\{v_i\log h(x_i)-H(x_i)\}.
$$

Every individual therefore contributes survival exposure, whether or not an event is observed. These formulas do not justify ignoring [informative censoring](../../../../../../informative-censoring.md); that situation requires a model for the observation mechanism as well.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
