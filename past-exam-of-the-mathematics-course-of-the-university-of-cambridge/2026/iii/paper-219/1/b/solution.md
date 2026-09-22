<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Ignoring terms independent of $r_0$, the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(r_0)=-3N\log r_0-\frac1{r_0}\sum_{s=1}^Nr_s.
$$

Its score vanishes at

$$
\widehat r_0=\frac1{3N}\sum_{s=1}^Nr_s.
$$

The expected [Fisher information](../../../../../../fisher-information-matrix.md) is

$$
\mathcal I_N(r_0)=-\mathbb E\ell''(r_0)=\frac{3N}{r_0^2}.
$$

Because a shape-three gamma variable has mean $3r_0$ and variance $3r_0^2$,

$$
\mathbb E\widehat r_0=r_0,
\qquad
\operatorname{Var}(\widehat r_0)=\frac{r_0^2}{3N}.
$$

The estimator is unbiased and attains the [Cramér-Rao lower bound](../../../../../../cramer-rao-bound.md) $\mathcal I_N(r_0)^{-1}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
