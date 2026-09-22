<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [linear estimator in nonparametric regression](../../../../../linear-estimator-in-nonparametric-regression.md) at $x_0$ has the form $\widehat m_n(x_0)=\sum_iW_i(x_0)Y_i$, where the weights may depend on the design, $x_0$, $p$, $h$, and $K$, but not on the responses. Put

$$
K_i=\prod_{j=1}^dK\left(\frac{x_{ij}-x_{0j}}h\right),
\qquad Q_i=Q_h(x_i-x_0),
$$

and define the [local polynomial Gram matrix](../../../../../local-polynomial-gram-matrix.md)

$$
B_n(x_0)=\frac1{nh^d}\sum_iK_iQ_iQ_i^\top,
\qquad \lambda_0=\lambda_{\min}(B_n(x_0)).
$$

When $\lambda_0>0$, the [weighted least squares](../../../../../weighted-least-squares.md) normal equations have the unique solution

$$
\widehat\beta=B_n(x_0)^{-1}\frac1{nh^d}\sum_iK_iQ_iY_i.
$$

Therefore $\widehat m_n(x_0)=\sum_iW_iY_i$, where the [effective kernel weight](../../../../../effective-kernel-weight.md) is

$$
W_i=\frac1{nh^d}e_1^\top B_n(x_0)^{-1}Q_iK_i.
$$

The identity

$$
\sum_iW_iQ_i^\top=e_1^\top
$$

shows that these weights exactly reproduce at $x_0$ every [multivariate polynomial](../../../../../multivariate-polynomial.md) of total degree at most $p$. This is the required [polynomial reproduction property of local polynomial regression](../../../../../polynomial-reproduction-property-of-local-polynomial-regression.md).

Only grid points with $\lVert x_i-x_0\rVert_\infty\leq h$ have nonzero weight. There are at most $(2n_1h+1)^d\leq(4n_1h)^d=4^dnh^d$ such points because $n_1h\geq1/2$. On this support,

$$
\lVert Q_i\rVert_2^2
\leq\sum_{\alpha\in\mathbb N_0^d}\frac1{\alpha!}
=e^d,
$$

so the [operator norm](../../../../../operator-norm.md) bound $\lVert B_n^{-1}\rVert_{\mathrm{op}}=\lambda_0^{-1}$ gives

$$
|W_i|\leq\frac{e^{d/2}\lVert K\rVert_\infty^d}{\lambda_0nh^d}.
$$

Because the errors are [independent random variables](../../../../../independent-random-variables.md) with the stated variance bounds,

$$
\operatorname{Var}(\widehat m_n(x_0))
\leq\sigma^2\sum_iW_i^2
\leq\frac{(4e)^d\lVert K\rVert_\infty^{2d}\sigma^2}
{\lambda_0^2nh^d}.
$$

Thus $\gamma_1=d$.

Let $T_{x_0}$ be the [Multivariate Taylor polynomial](../../../../../multivariate-taylor-polynomial.md) of $m$ at $x_0$ through total degree $\beta_0$. The assumed [Hölder continuity](../../../../../holder-condition.md) of the derivatives and

$$
\sum_{|\alpha|=\beta_0}\frac1{\alpha!}=\frac{d^{\beta_0}}{\beta_0!}
$$

give the [Taylor remainder](../../../../../taylor-remainder.md) bound

$$
|m(x)-T_{x_0}(x)|
\leq\frac{d^{\beta_0}L}{\beta_0!}\lVert x-x_0\rVert_\infty^\beta.
$$

Polynomial reproduction cancels $T_{x_0}$ in the bias. The same support count and weight bound give

$$
\sum_i|W_i|
\leq\frac{(4e^{1/2})^d\lVert K\rVert_\infty^d}{\lambda_0}.
$$

Consequently

$$
|\operatorname{Bias}(\widehat m_n(x_0))|
\leq
\frac{(4e^{1/2})^dd^{\beta_0}L\lVert K\rVert_\infty^d}
{\lambda_0\beta_0!}h^\beta,
$$

so $\gamma_2=\beta$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
