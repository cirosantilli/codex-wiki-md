<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For fixed $\beta$, conditional least squares is minimized by

$$
g_\beta(X)=\mathbb E[Y-\beta A\mid X]
=\mu(X)-\beta e(X).
$$

Therefore the remaining objective is

$$
\mathbb E\left[
\{Y-\mu(X)-\beta(A-e(X))\}^2
\right],
$$

whose [normal equation](../../../../../../normal-equation.md) gives

$$
\beta_3
=\frac{\mathbb E[(A-e(X))(Y-\mu(X))]}
{\mathbb E[(A-e(X))^2]}.
$$

Let

$$
\tau(X)=\mathbb E[Y(1)-Y(0)\mid X]
$$

be the [conditional average treatment effect](../../../../../../conditional-average-treatment-effect.md). Since $A$ is binary, conditional exchangeability implies

$$
\operatorname{Cov}(A,Y\mid X)
=e(X)\{1-e(X)\}\tau(X),
$$

and $\operatorname{Var}(A\mid X)=e(X)\{1-e(X)\}$. Hence

$$
\beta_3
=\frac{\mathbb E[e(X)\{1-e(X)\}\tau(X)]}
{\mathbb E[e(X)\{1-e(X)\}]}.
$$

Thus $\beta_3$ is the [overlap-weighted average treatment effect](../../../../../../overlap-weighted-average-treatment-effect.md). It weights covariate strata by the [overlap weight](../../../../../../overlap-weight.md) and generally differs from the ordinary ATE $\beta_1=\mathbb E[\tau(X)]$ when treatment effects are heterogeneous and overlap varies with $X$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
