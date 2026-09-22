<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\delta=\widehat\beta-\beta^0$. Comparing the Lasso objective at $\widehat\beta$ and $\beta^0$ gives the [Basic inequality for the Lasso](../../../../../../basic-inequality-for-the-lasso.md). On $\mathcal T$ it implies

$$
\frac1n\|X\delta\|_2^2
+2\lambda(\|\beta^0+\delta\|_1-\|\beta^0\|_1)
\leq\lambda\|\delta\|_1.
$$

Since

$$
\|\beta^0+\delta\|_1-\|\beta^0\|_1
\geq\|\delta_N\|_1-\|\delta_S\|_1,
$$

we obtain the [Lasso cone condition](../../../../../../lasso-cone-condition.md)

$$
\|\delta_N\|_1\leq3\|\delta_S\|_1.
$$

The [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) also give

$$
\widehat\Sigma\delta
=\frac1nX^T\varepsilon-\lambda\widehat z,
$$

so on $\mathcal T$,

$$
\|\widehat\Sigma\delta\|_\infty
\leq\frac\lambda2+\lambda=\frac{3\lambda}{2}.
$$

The assumed cone invertibility condition therefore yields

$$
\|\delta_S\|_\infty\leq\frac{3\lambda}{2\psi}.
$$

If $\min_{j\in S}|\beta_j^0|>3\lambda/(2\psi)$, then every active coefficient remains nonzero and retains its sign. Substituting $\lambda=A\sqrt{\log p/n}$ proves

$$
\operatorname{sgn}(\widehat\beta_S)=\operatorname{sgn}(\beta_S^0)
$$

on an event of the required probability. This is [Lasso sign recovery from cone invertibility](../../../../../../lasso-sign-recovery-from-cone-invertibility.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
