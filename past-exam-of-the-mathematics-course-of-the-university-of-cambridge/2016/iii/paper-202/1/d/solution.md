<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [simple predictable process](../../../../../../simple-predictable-process.md) from part (a), define its **[stochastic integral](../../../../../../stochastic-integral.md)** by

$$
\boxed{(H\cdot M)_t=\sum_i h_i\bigl(M_{t\wedge t_{i+1}}-M_{t\wedge t_i}\bigr).}
$$

The time-zero value contributes nothing. Write $D_i=M_{t\wedge t_{i+1}}-M_{t\wedge t_i}$. If $i<j$ and $t>t_j$, then $h_iD_i h_j$ is $\mathcal F_{t_j}$-[measurable](../../../../../../measurability.md) and $\mathbb E[D_j\mid\mathcal F_{t_j}]=0$. If $t\leq t_j$, then $D_j=0$. Boundedness ensures [integrability](../../../../../../integrability.md), so all off-diagonal terms vanish by [conditional expectation](../../../../../../conditional-expectation.md). Consequently

$$
\boxed{\mathbb E[(H\cdot M)_t^2]=\sum_i\mathbb E[h_i^2D_i^2].}
$$

The [quadratic variation](../../../../../../quadratic-variation.md) theorem says $M^2-[M]$ is a [local martingale](../../../../../../local-martingale.md). A bounded continuous [martingale](../../../../../../martingale-split.md) is [square-integrable](../../../../../../square-integrable-function.md), and localization gives the conditional second-moment identity

$$
\mathbb E[D_i^2\mid\mathcal F_{t_i}]=\mathbb E\bigl([M]_{t\wedge t_{i+1}}-[M]_{t_i}\mid\mathcal F_{t_i}\bigr)\qquad(t\geq t_i).
$$

Multiplication by $h_i^2$ and summation therefore give the **[Itô isometry](../../../../../../ito-isometry.md)**

$$
\boxed{\mathbb E\left|\int_0^t H_s\,dM_s\right|^2=\mathbb E\int_0^t H_s^2\,d[M]_s.}
$$

For [Brownian motion](../../../../../../brownian-motion-split.md), $[M]_s=s$. More generally the [Itô isometry](../../../../../../ito-isometry.md) holds for every [predictable process](../../../../../../predictable-process.md) with finite right-hand side, against a continuous [square-integrable](../../../../../../square-integrable-function.md) [martingale](../../../../../../martingale-split.md). Indeed, on a fixed horizon the [quadratic-variation measure](../../../../../../quadratic-variation-measure.md) $\mu_M(E)=\mathbb E\int_0^t\mathbf1_E\,d[M]$ is finite. Part (c) approximates the integrand by [simple predictable processes](../../../../../../simple-predictable-process.md); the displayed equality makes the elementary integrals Cauchy in $L^2$ and defines their unique limit. The finite sum is exactly the elementary case of the [Itô isometry](../../../../../../ito-isometry.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
