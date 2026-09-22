<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix a primitive $\lambda$ of the [standard symplectic form](../../../../../../standard-symplectic-form.md) on $\mathbb R^{2n}$. With the coordinates of Question 2 one convenient choice is

$$
\lambda=\frac12\sum_j(q_j\,dp_j-p_j\,dq_j),\qquad d\lambda=\omega_0.
$$

For a [Lagrangian submanifold](../../../../../../lagrangian-submanifold.md) with inclusion $i:L\hookrightarrow\mathbb R^{2n}$, $d(i^*\lambda)=i^*\omega_0=0$. Its [Liouville class of a Lagrangian submanifold](../../../../../../liouville-class-of-a-lagrangian-submanifold.md) is

$$
\boxed{\ell_L=[i^*\lambda]\in H^1_{\mathrm{dR}}(L;\mathbb R)}.
$$

Any two primitives differ by a closed one-form on the contractible ambient space, hence by an exact form, so the class is independent of the primitive. The cotangent primitive convention $\theta=\sum_jp_jdq_j$, with $\omega_0=-d\theta$, gives the negative of this class; rationality, positive period size and nonvanishing do not depend on that sign.

The period homomorphism sends an integral one-cycle $c$ to $\int_c i^*\lambda$. Its image $\operatorname{Per}(L)\subset\mathbb R$ is an additive subgroup. A [rational Lagrangian submanifold](../../../../../../rational-lagrangian-submanifold.md) is one for which this subgroup is discrete. In the nonzero case it has a unique positive generator:

$$
\boxed{\operatorname{Per}(L)=\gamma(L)\mathbb Z,\qquad\gamma(L)>0}.
$$

Equivalently $\ell_L$ is a real multiple of an integral cohomology class. The invariant $\gamma(L)$ is its [least positive Liouville period](../../../../../../least-positive-liouville-period.md), also expressible as $\inf\{a>0:a\in\operatorname{Per}(L)\}$. If the period group is zero, that infimum is $+\infty$ by the empty-set convention; some treatments instead reserve “rational” for the nonzero discrete case. Because the ambient space is contractible, the [Stokes theorem](../../../../../../stokes-theorem.md) identifies these periods with signed symplectic areas of disks whose boundaries lie on $L$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
