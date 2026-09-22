<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\{v_i\}$ be an orthonormal [eigenbasis](../../../../../../eigenbasis.md) of $C$, with $\lambda_1\geq\lambda_2\geq\cdots\geq0$. Expand $w=\sum_i b_iv_i$. At the normalized length imposed on positive-output equilibria,

$$
\sum_i b_i^2=\frac1\alpha,\qquad
\langle y^2\rangle=w^TCw=\sum_i\lambda_i b_i^2\leq\frac{\lambda_1}{\alpha}.
$$

Equality holds exactly when $w$ lies in the largest-eigenvalue eigenspace. If $\lambda_1$ is simple,

$$
\boxed{w=\pm\frac{v_1}{\sqrt\alpha},\qquad
\max\langle y^2\rangle=\frac{\lambda_1}{\alpha}.}
$$

The norm constraint is essential: without it, scaling a direction with positive eigenvalue makes the output second moment arbitrarily large, so the printed maximization statement would have no finite maximum. When $\alpha=1$, this is the usual unit-length formulation.

For centered inputs, maximizing this quantity maximizes output variance. The unit therefore selects the first [principal component analysis](../../../../../../principal-component-analysis.md) direction: a stimulus feature with the greatest variation in the input ensemble. Biologically, learned synaptic weights become selective to that dominant correlated pattern, rather than to a teacher-supplied label. For uncentered inputs it maximizes a second moment including the mean response, which is not the same as maximizing variance. If the top eigenvalue is repeated, any normalized vector in its eigenspace attains the same maximum.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
