<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
R=\begin{pmatrix}I_k&0\end{pmatrix}\in\mathbb R^{k\times p},
\qquad
r=R\theta^*.
$$

Then the null hypothesis is $R\theta_0=r$. Define the [Wald statistic for linear restrictions](../../../../../../wald-statistic-for-linear-restrictions.md)

$$
W_{n,R}
=n(R\widehat\theta_n-r)^T
\left[R I(\widehat\theta_n)^{-1}R^T\right]^{-1}
(R\widehat\theta_n-r).
$$

Under $H_0$, part (a) and the continuous mapping theorem give

$$
\sqrt n(R\widehat\theta_n-r)
=\sqrt nR(\widehat\theta_n-\theta_0)
\xrightarrow d N_k(0,V_0),
$$

where

$$
V_0=R I(\theta_0)^{-1}R^T.
$$

The matrix $V_0$ is positive definite because $I(\theta_0)$ is positive definite and $R$ has full row rank. Consistency gives

$$
R I(\widehat\theta_n)^{-1}R^T\xrightarrow p V_0.
$$

Therefore [Slutsky theorem](../../../../../../slutsky-theorem.md) yields

$$
V_0^{-1/2}\sqrt n(R\widehat\theta_n-r)
\xrightarrow dN_k(0,I_k),
$$

and applying the continuous squared-norm map proves rigorously that

$$
\boxed{W_{n,R}\xrightarrow d\chi_k^2.}
$$

Let $q_{k,1-\alpha}$ be the $(1-\alpha)$ quantile of $\chi_k^2$. Rejecting $H_0$ when

$$
W_{n,R}>q_{k,1-\alpha}
$$

has rejection probability tending to $\alpha$ under every fixed parameter satisfying $H_0$, and is therefore an asymptotically valid level-$\alpha$ test.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
