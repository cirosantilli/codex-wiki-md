<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The centered term in $\rho^*$ has zero mean, giving $\mathbb E\rho^*=1/R$ and hence $\mathbb E[\rho^*B_1]=1=B_0$. For the risky assets, symmetry of the [covariance matrix](../../../../../../covariance-matrix.md) gives

$$
\mathbb E[\rho^*S_1]
=\frac\mu R+\mathbb E[(S_1-\mu)(S_1-\mu)^T]V^{-1}h
=\frac\mu R+h=S_0.
$$

Therefore **$\rho^*$ reproduces every asset's initial price**.

For another square-integrable $\rho$ satisfying the price moment constraints, set $\delta=\rho-\rho^*$. The bank equation and $R\ne0$ give $\mathbb E\delta=0$, while the risky equations give $\mathbb E[\delta S_1]=0$. Since $\rho^*$ is an affine combination of $1$ and the coordinates of $S_1$,

$$
\mathbb E[\delta\rho^*]
=\frac1R\mathbb E\delta+h^TV^{-1}\mathbb E[\delta(S_1-\mu)]=0.
$$

The [Pythagorean theorem in an inner-product space](../../../../../../pythagorean-theorem-in-an-inner-product-space.md) now gives

$$
\boxed{\mathbb E[\rho^2]=\mathbb E[(\rho^*)^2]+\mathbb E[(\rho-\rho^*)^2]
\geq\mathbb E[(\rho^*)^2].}
$$

Equality holds exactly when $\rho=\rho^*$ almost surely. If a competing weight has infinite second moment, the inequality is immediate in the extended sense. The minimum itself is

$$
\mathbb E[(\rho^*)^2]=\frac1{R^2}+h^TV^{-1}h.
$$

Thus $\rho^*$ is the orthogonal projection of any feasible square-integrable pricing weight onto the linear span of the traded payoffs.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
