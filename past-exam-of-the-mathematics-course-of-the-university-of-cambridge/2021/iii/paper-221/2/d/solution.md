<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
d=\mathbb E[X^2],\qquad q=\mathbb E[XZ],\qquad
R_0=Z-\gamma_0X.
$$

Assumption 2 implies $\gamma_0=q/d$. Although the printed $\widehat\gamma$ need not converge to $\gamma_0$, its first-order effect vanishes because $\mathbb E[VX]=0$. Inverting the $2\times2$ Jacobian of the remaining [estimating equations](../../../../../../estimating-equation.md) gives the influence function

$$
\operatorname{IF}_\beta
=\frac{V\{dW-\mathbb E[XW]X\}}
{d\mathbb E[AW]-\mathbb E[XW]\mathbb E[AX]}
=\frac{VR_0}{\mathbb E[AR_0]}.
$$

The first-stage condition yields

$$
\mathbb E[AR_0]
=\mathbb E[\mathbb E[A\mid X,Z]R_0]
=\lambda\mathbb E[R_0^2].
$$

Hence the asymptotic variance of $\sqrt n(\widehat\beta-\beta_0)$ is the [sandwich](../../../../../../sandwich-covariance-matrix.md) expression

$$
\boxed{
\mathcal V_\beta
=\frac{\mathbb E[V^2R_0^2]}
{\lambda^2\{\mathbb E[R_0^2]\}^2}}.
$$

There is a defect in the printed assumptions: $\operatorname{Var}(V\mid A,X)=\sigma^2$ alone does not determine $\mathbb E[V^2R_0^2]$, because $R_0$ depends on $Z$ and $V$ can have a nonzero conditional mean given $(A,X)$ under unmeasured confounding. Under the standard intended strengthening $\mathbb E[V^2\mid X,Z]=\sigma^2$, the formula simplifies to

$$
\boxed{
\mathcal V_\beta=\frac{\sigma^2}{\lambda^2\mathbb E[(Z-\gamma_0X)^2]}}.
$$

The asymptotic variance of $\widehat\beta$ itself is $\mathcal V_\beta/n$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
