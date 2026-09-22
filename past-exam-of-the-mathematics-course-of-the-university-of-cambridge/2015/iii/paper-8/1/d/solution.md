<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume $\omega\ne0$. With $h=0$, the [method of characteristics](../../../../../../method-of-characteristics.md) gives $f(t,\Phi(t,0,z))=f_0(z)$. Hence

$$
\operatorname{supp}f_t=\Phi(t,0,\operatorname{supp}f_0).
$$

Let $K=\operatorname{supp}f_0$ and $E_*=\max_KH_\omega$; if $f_0=0$, the conclusion is immediate. By the [Hamiltonian energy balance](../../../../../../hamiltonian-energy-balance.md), every image point of $K$ remains in the [energy](../../../../../../energy.md) sublevel

$$
\mathcal K=\{(x,v):|v|^2+\omega^2|x|^2\leq2E_*\}.
$$

This is a fixed compact [ellipsoid](../../../../../../ellipsoid.md) in [phase space](../../../../../../phase-space.md). Therefore **the [support](../../../../../../support.md) bound is uniform in time**:

$$
\boxed{\operatorname{supp}f_t\subseteq\mathcal K,\qquad
|v|\leq\sqrt{2E_*},\quad |x|\leq\frac{\sqrt{2E_*}}{|\omega|}.}
$$

This [uniform support bound from a coercive conserved energy](../../../../../../uniform-support-bound-from-a-coercive-conserved-energy.md) requires no explicit solution of the curves.

The nonzero-frequency qualification is necessary. At $\omega=0$ the [energy](../../../../../../energy.md) does not control $x$, and the equation is [free transport equation](../../../../../../free-transport-equation.md). Choose a smooth [compactly supported](../../../../../../compact-support.md) $f_0$ that is nonzero at $(x_0,v_0)$ with $v_0\ne0$. Its transported value at $(x_0+tv_0,v_0)$ stays nonzero, so the union of the supports is unbounded. Each individual [support](../../../../../../support.md) is compact, but there is no fixed [compact support](../../../../../../compact-support.md) for all times.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
