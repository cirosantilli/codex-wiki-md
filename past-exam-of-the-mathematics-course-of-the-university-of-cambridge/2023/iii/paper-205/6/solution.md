<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

With the convention matching the constants below, the [Lasso](../../../../../lasso.md) estimator is any minimizer

$$
\widehat\beta\in\underset{\beta\in\mathbb R^p}{\operatorname{argmin}}
\left\{\frac1n\|Y-X\beta\|_2^2+2\lambda\|\beta\|_1\right\}.
$$

Because $X^T\mathbf1=0$, the centered noise has the same score as $\varepsilon$: $X^T(\varepsilon-\overline\varepsilon\mathbf1)=X^T\varepsilon$. Each $X_j^T\varepsilon/n$ is sub-Gaussian with scale $1/\sqrt n$, so

$$
\mathbb P\!\left(\frac{2|X_j^T\varepsilon|}{n}>\lambda\right)
\leq2e^{-n\lambda^2/8}.
$$

For $\lambda=A\sqrt{\log p/n}$, a [union bound](../../../../../boole-s-inequality.md) over the $p$ columns yields

$$
\mathbb P\!\left(\frac{2\|X^T\varepsilon\|_\infty}{n}\leq\lambda\right)
\geq1-2p^{-(A^2/8-1)}.
$$

Call this event $\mathcal T$.

The [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) for the Lasso say that there is $\widehat z\in\mathbb R^p$ such that

$$
\frac1nX^T(Y-X\widehat\beta)=\lambda\widehat z,
\qquad
\widehat z_j=
\begin{cases}
\operatorname{sgn}(\widehat\beta_j),&\widehat\beta_j\ne0,\\
[-1,1],&\widehat\beta_j=0.
\end{cases}
$$

Equivalently, $\widehat z$ belongs to the [subdifferential](../../../../../subdifferential.md) of the $\ell^1$ norm at $\widehat\beta$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
