<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write the standard complex coordinates as $z_j=q_j+ip_j$ and let $J$ denote multiplication by $i$. Use the [standard symplectic form](../../../../../standard-symplectic-form.md) $\omega_0=\sum_jdq_j\wedge dp_j$, for which $\omega_0(v,Jv)=|v|^2$. In real coordinates $s,t$ on the disk, holomorphicity and the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) imply

$$
\partial_t h=J\partial_s h.
$$

Therefore the pulled-back two-form is

$$
h^*\omega_0=\omega_0(\partial_sh,\partial_th)\,ds\wedge dt=|\partial_s h|^2\,ds\wedge dt.
$$

If this integral were zero, the continuous nonnegative integrand would vanish everywhere in the interior. The displayed Cauchy-Riemann relation would then make both first derivatives zero, forcing $h$ to be constant on the connected disk and, by continuity, on its boundary. For the nonconstant map under consideration the [symplectic area](../../../../../symplectic-area.md) is consequently strictly positive:

$$
\int_{D^2}h^*\omega_0=\int_{D^2}|\partial_sh|^2\,ds\,dt>0.
$$

Take the primitive $\lambda=\tfrac12\sum_j(q_jdp_j-p_jdq_j)$ from Question 3. Let $c=h|_{\partial D^2}$, oriented as the boundary of the disk. Since $c$ lies in $L$, the [Stokes theorem](../../../../../stokes-theorem.md) gives

$$
\boxed{\int_c\lambda|_L=\int_{\partial D^2}h^*\lambda=\int_{D^2}h^*\omega_0>0}.
$$

The restriction $\lambda|_L$ is closed because $L$ is a [Lagrangian submanifold](../../../../../lagrangian-submanifold.md). If its [Liouville class of a Lagrangian submanifold](../../../../../liouville-class-of-a-lagrangian-submanifold.md) were zero, it would be an [exact differential form](../../../../../exact-differential-form.md), and its integral along every closed curve in $L$ would vanish. The boundary loop above contradicts this. **The Liouville class is therefore nonzero.** This proves that a [holomorphic disk detects a nonzero Liouville class](../../../../../holomorphic-disk-detects-a-nonzero-liouville-class.md) directly by positivity and Stokes; no disk-existence theorem is being assumed beyond the disk given here.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
