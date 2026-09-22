<h1 id="6h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The density is an equal mixture of the uniform distributions on $[0,1]$ and $[0,\theta]$. Hence

$$
\mathbb E_\theta X
=\frac12\cdot\frac12+\frac12\cdot\frac\theta2
=\frac{1+\theta}{4},
$$

so

$$
\boxed{\mathbb E_\theta(4\overline X-1)=\theta}.
$$

Thus $\widetilde\theta$ is unbiased.

Also,

$$
\mathbb E_\theta X^2=\frac{1+\theta^2}{6},
\qquad
\operatorname{Var}_\theta X
=\frac{5\theta^2-6\theta+5}{48}.
$$

The [central limit theorem](../../../../../../central-limit-theorem.md) gives

$$
\sqrt n(\widetilde\theta-\theta)
\xrightarrow{d}
N\left(0,\frac{5\theta^2-6\theta+5}{3}\right).
$$

Replacing $\theta$ in the asymptotic standard error by the consistent estimator $\widetilde\theta$ gives the [Wald confidence interval](../../../../../../wald-confidence-interval.md)

$$
\boxed{
\widetilde\theta
\mathbin{\pm}
z_{1-\alpha/2}
\sqrt{\frac{5\widetilde\theta^2-6\widetilde\theta+5}{3n}}}.
$$

It may be intersected with the parameter space $(0,1)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6H](../../6h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
