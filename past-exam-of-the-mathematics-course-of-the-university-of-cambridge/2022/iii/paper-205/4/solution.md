<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Group Lasso](../../../../../group-lasso.md) penalty is

$$
\lambda P(\beta),
\qquad
P(\beta)=\sum_{j=1}^qm_j\|\beta_{G_j}\|_2.
$$

By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) within each group,

$$
|u^Tv|
\leq\sum_j\|u_{G_j}\|_2\|v_{G_j}\|_2
\leq
\max_km_k^{-1}\|v_{G_k}\|_2
\sum_jm_j\|u_{G_j}\|_2.
$$

Put $\delta=\widehat\beta-\beta^0$. Comparing the objective at $\widehat\beta$ and $\beta^0$ gives

$$
\frac1{2n}\|X\delta\|_2^2
\leq\frac1n\epsilon^TX\delta
+\lambda\{P(\beta^0)-P(\widehat\beta)\}.
$$

On $\Omega$, the preceding duality inequality gives

$$
\frac1n|\epsilon^TX\delta|\leq\lambda P(\delta).
$$

The triangle inequality $P(\delta)\leq P(\beta^0)+P(\widehat\beta)$ then yields

$$
\frac1n\|X(\beta^0-\widehat\beta)\|_2^2
\leq4\lambda P(\beta^0).
$$

When $m_j=\sqrt r$ and $X_{G_j}^TX_{G_j}=nI_r$,

$$
\frac{\|X_{G_j}^T\epsilon\|_2^2}{n}\sim\chi_r^2.
$$

Writing $\delta_0=n\lambda^2-1\in(0,1)$, the exponential Markov inequality and the supplied chi-square moment-generating-function bound give

$$
\mathbb P(\chi_r^2>r(1+\delta_0))
\leq\exp(-r\delta_0^2/8).
$$

The prescribed equation makes this $q^{-(A+1)}$. A [union bound](../../../../../boole-s-inequality.md) over the $q$ groups therefore gives

$$
\boxed{\mathbb P(\Omega)\geq1-q^{-A}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
