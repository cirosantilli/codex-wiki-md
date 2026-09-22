<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix an arbitrary finite $T$ and use the [Banach space](../../../../../../banach-space-split.md) of [bounded continuous functions](../../../../../../bounded-continuous-functions.md) $C_b([0,T]\times\mathbb R^{2d})$ with the [supremum norm](../../../../../../supremum-norm.md). Set $A=\|k_1\|_\infty\|k_2\|_1$. For $f$ in this space, the velocity [integral](../../../../../../integral.md)

$$
H_f(t,x)=\int k_2(v_*)f(t,x,v_*)\,dv_*
$$

is bounded by $\|k_2\|_1\|f\|_\infty$. If $(t_n,x_n)\to(t,x)$, the integrands converge pointwise and are bounded by the integrable function $\|f\|_\infty k_2$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) proves continuity. Thus the [rank-one gain on bounded continuous functions](../../../../../../rank-one-gain-on-bounded-continuous-functions.md), $Kf=k_1H_f$, is continuous and bounded. The same theorem applied to the time [integral](../../../../../../integral.md) shows that $\tau$ maps this space into itself, including at $t=0$.

Time ordering gives the [factorial bound for a Volterra iterate](../../../../../../factorial-bound-for-a-volterra-iterate.md):

$$
\|(\tau^n h)(t)\|_\infty\leq\frac{A^nt^n}{n!}\sup_{s\leq t}\|h(s)\|_\infty.
$$

Consequently the [Volterra series for the linear Boltzmann equation](../../../../../../volterra-series-for-the-linear-boltzmann-equation.md)

$$
\boxed{f=\sum_{n=0}^\infty\tau^nF(f_0)}
$$

converges uniformly on the whole finite time slab, so its sum is continuous and bounded and satisfies the [fixed point](../../../../../../fixed-point.md) equation. Tracking the damping factors gives the sharper pointwise bound $\|f(t)\|_\infty\leq e^{(A-1)t}\|f_0\|_\infty$. This proves existence for every finite $T$, without requiring $AT<1$ or uniform continuity of $f_0$. Boundedness on finite slabs does not assert a uniform bound over infinite time.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
