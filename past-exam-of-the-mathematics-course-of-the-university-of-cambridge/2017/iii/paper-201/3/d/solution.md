<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the same [dyadic slope martingale](../../../../../../dyadic-slope-martingale.md) $G_n$ and dyadic [filtration](../../../../../../filtration-probability-theory.md) as in (c). Each $G_n$ is integrable, since it takes finitely many finite values. On each dyadic cell, the absolute slope is $2^n$ times the absolute endpoint increment. Consequently the hypothesis in the PDF is exactly

$$
\int_0^1|G_n(t)|\mathbf1_{\{|G_n(t)|\geq\lambda\}}dt=V_n(f,\lambda),
\qquad
\sup_n\int_0^1|G_n|\mathbf1_{\{|G_n|\geq\lambda\}}dt\longrightarrow0.
$$

Thus $(G_n)$ is [uniformly integrable](../../../../../../uniform-integrability.md). It is also bounded in [L1 norm](../../../../../../l1-norm.md): choose a finite $\lambda_0>0$ at which the supremum of the tails is finite, and use $\|G_n\|_1\leq\lambda_0+\sup_jV_j(f,\lambda_0)$. The [uniformly integrable martingale convergence theorem](../../../../../../uniformly-integrable-martingale-convergence-theorem.md) supplies $g\in L^1([0,1])$ with $G_n\to g$ in [L1 norm](../../../../../../l1-norm.md).

The functions $f_n(x)=f(0)+\int_0^xG_n(t)dt$ are again the dyadic [linear interpolations](../../../../../../linear-interpolation.md) of $f$. Since $f$ is continuous on a compact interval, it is [uniformly continuous](../../../../../../uniform-continuity.md), and $\|f_n-f\|_\infty\leq\omega_f(2^{-n})\to0$, where $\omega_f$ is its [modulus of continuity](../../../../../../modulus-of-continuity.md). On the other hand, the [integral](../../../../../../integral.md) of $G_n-g$ is uniformly bounded in absolute value by $\|G_n-g\|_1\to0$. Hence the [dyadic slope-tail criterion for absolute continuity](../../../../../../dyadic-slope-tail-criterion-for-absolute-continuity.md) gives

$$
\boxed{f(x)=f(0)+\int_0^xg(t)dt\quad\text{for every }x\in[0,1],\qquad g\in L^1([0,1]).}
$$

No boundedness of $g$ is asserted here; the tail condition permits integrable densities that are unbounded.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
