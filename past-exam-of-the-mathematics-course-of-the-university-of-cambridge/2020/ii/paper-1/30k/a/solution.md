<h1 id="30k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The time-zero budget constraint is

$$
\theta^0+\theta^TS_0=w_0,
$$

so $\theta^0=w_0-\theta^TS_0$. The terminal wealth is therefore

$$
W_1=\overline\theta^T\overline S_1
=(1+r)w_0+\theta^T\bigl(S_1-(1+r)S_0\bigr).
$$

Put

$$
b=\mu-(1+r)S_0,
\qquad
c=w_1-(1+r)w_0.
$$

Then

$$
\mathbb EW_1=(1+r)w_0+\theta^Tb,
\qquad
\operatorname{Var}(W_1)=\theta^TV\theta,
$$

and the target mean is the linear constraint $\theta^Tb=c$.

Since the invertible [covariance matrix](../../../../../../covariance-matrix.md) $V$ is positive definite, the [Lagrange multiplier](../../../../../../lagrange-multiplier.md) equation for minimizing $\theta^TV\theta$ is

$$
2V\theta-\eta b=0.
$$

Thus

$$
\theta=\lambda V^{-1}b=\lambda\theta_m,
\qquad
\theta_m=V^{-1}\bigl(\mu-(1+r)S_0\bigr).
$$

The constraint determines

$$
\boxed{
\lambda=\frac{w_1-(1+r)w_0}
{\bigl(\mu-(1+r)S_0\bigr)^TV^{-1}
\bigl(\mu-(1+r)S_0\bigr)}.
}
$$

This is the [one-period Gaussian minimum-variance portfolio](../../../../../../one-period-gaussian-minimum-variance-portfolio.md); the riskless holding is then $\theta^0=w_0-\theta^TS_0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
