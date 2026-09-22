<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $A=V^{1/2}$ be the symmetric positive square root of the [covariance matrix](../../../../../../covariance-matrix.md), and write $S_1=\mu+AZ$ with $Z$ having the [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) $N_d(0,I)$. Bounded gradient makes $g$ globally Lipschitz, so $g(S_1)$ has at most linear growth and is square integrable. This also justifies the permitted [Gaussian integration by parts](../../../../../../stein-s-lemma-probability.md) formula for each coordinate.

By the [chain rule](../../../../../../chain-rule.md), $\nabla_z g(\mu+Az)=A^T\nabla g(\mu+Az)$. Applying Gaussian integration by parts gives

$$
c=\mathbb E[(S_1-\mu)g(S_1)]
=A\,\mathbb E[Zg(\mu+AZ)]
=AA^T\mathbb E[\nabla g(S_1)]
=V\mathbb E[\nabla g(S_1)].
$$

Thus the [Gaussian quadratic hedge](../../../../../../gaussian-quadratic-hedge.md) holds $\pi^*=\mathbb E[\nabla g(S_1)]$. Substitution into its initial capital formula yields

$$
\boxed{X_0^*=\frac1{1+r}\mathbb E[g(S_1)]
+\left(S_0-\frac\mu{1+r}\right)\cdot\mathbb E[\nabla g(S_1)].}
$$

Only the hedge calculation is being used here; the Gaussian model need not possess a positive pricing weight for this least-squares identity.

## ↑ Ancestors (11)

1. [D](../d.md)
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
