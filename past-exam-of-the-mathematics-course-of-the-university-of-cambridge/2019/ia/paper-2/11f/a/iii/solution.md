<h1 id="11f/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [covariance matrix](../../../../../../../covariance-matrix.md) is

$$
\boxed{V=\begin{pmatrix}
\sigma_1^2&\rho\sigma_1\sigma_2\\
\rho\sigma_1\sigma_2&\sigma_2^2
\end{pmatrix}}.
$$

If $\operatorname{Cov}(X_1,X_2)=0$, the moment-generating function in part (ii) factors into the product of the two marginal moment-generating functions. Thus $X_1$ and $X_2$ are [independent random variables](../../../../../../../independent-random-variables.md); this is the [independence of uncorrelated jointly normal variables](../../../../../../../independence-of-uncorrelated-jointly-normal-variables.md).

By bilinearity of [covariance](../../../../../../../covariance.md),

$$
\operatorname{Cov}(X_1,X_2-aX_1)
=\rho\sigma_1\sigma_2-a\sigma_1^2.
$$

Choose

$$
\boxed{a=\rho\frac{\sigma_2}{\sigma_1}},
\qquad Y=X_2-aX_1.
$$

Then $(X_1,Y)$ is bivariate normal by part (i) and has zero covariance, so $Y$ is a normal random variable independent of $X_1$. Hence $X_2=aX_1+Y$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [11F](../../../11f.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
