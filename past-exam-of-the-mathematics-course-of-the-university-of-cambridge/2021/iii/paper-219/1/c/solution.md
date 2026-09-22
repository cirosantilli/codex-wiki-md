<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Writing $r_s=1/\alpha_s$, the log likelihood is

$$
\ell(r_0)=\text{constant}-3N\log r_0-\frac1{r_0}\sum_sr_s.
$$

Hence

$$
\boxed{\widehat r_0=\frac1{3N}\sum_{s=1}^N\frac1{\alpha_s}}.
$$

The score variance and negative expected Hessian give [Fisher information](../../../../../../fisher-information-matrix.md)

$$
\mathcal I_N(r_0)=\frac{3N}{r_0^2}.
$$

Since $r_s$ is Gamma with mean $3r_0$ and variance $3r_0^2$,

$$
\mathbb E\widehat r_0=r_0,\qquad
\operatorname{Var}(\widehat r_0)=\frac{r_0^2}{3N}.
$$

The estimator is unbiased and attains the [Cramér-Rao lower bound](../../../../../../cramer-rao-bound.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
