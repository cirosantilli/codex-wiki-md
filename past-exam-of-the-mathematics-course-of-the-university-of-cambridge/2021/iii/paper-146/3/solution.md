<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

With the convention

$$
\iota_{X_{f_t}}\omega=-df_t,
$$

the time-dependent [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) is uniquely determined because $\omega$ is [nondegenerate](../../../../../nondegenerate-bilinear-form.md). If $\phi_t$ is its local flow, [Cartan's magic formula](../../../../../cartan-s-magic-formula.md) gives

$$
\frac d{dt}\phi_t^*\omega
=\phi_t^*\mathcal L_{X_{f_t}}\omega
=\phi_t^*\left(d\iota_{X_{f_t}}\omega+\iota_{X_{f_t}}d\omega\right)
=0.
$$

Thus $\phi_t^*\omega=\omega$ wherever the flow is defined, which is the [Hamiltonian flow preserves the symplectic form](../../../../../hamiltonian-flow-preserves-the-symplectic-form.md) property.

Write $v=(a,b)$ and $\omega_0=dx\wedge dy$. The linear Hamiltonian

$$
H_0(x,y)=bx-ay
$$

has Hamiltonian vector field $X_{H_0}=v$. Choose a smooth cutoff $\rho$ that is one on $B(r+|v|)$ and zero outside $B(r+|v|+\epsilon)$, and put $H=\rho H_0$. Every trajectory beginning in $B(r)$ and following $v$ remains in $B(r+|v|)$ for time $0\leq t\leq1$, so the time-one map translates that ball by $v$. Outside $B(r+|v|+\epsilon)$ its vector field vanishes, so the map is the identity. This is a [compactly supported Hamiltonian translation](../../../../../compactly-supported-hamiltonian-translation.md) and hence a compactly supported [symplectomorphism](../../../../../symplectomorphism.md).

For the connected-sum construction, choose a [Darboux chart](../../../../../darboux-chart.md) about the unique transverse intersection and straighten the two Lagrangian sheets to $\mathbb R^2$ and $i\mathbb R^2$ in $\mathbb C^2$. Remove small disks from the two sheets and join their boundary circles by the standard Lagrangian neck

$$
(t,u)\longmapsto\bigl(a(t)u,b(t)u\bigr),
\qquad u\in S^1,
$$

in $\mathbb R_x^2\oplus\mathbb R_y^2$, where $(a(t),b(t))$ follows a smooth arc from one positive coordinate ray to the other and agrees with those rays near its ends. Its pullback of $\sum_jdx_j\wedge dy_j$ vanishes because $u\mathbin{\cdot}u'=0$. Gluing this neck to the unchanged surfaces performs [Lagrangian surgery](../../../../../lagrangian-surgery.md). Topologically it is their connected sum, so it gives a [Lagrangian connected sum](../../../../../lagrangian-connected-sum.md)

$$
\Sigma_{g_1}\mathbin\#\Sigma_{g_2}\cong\Sigma_{g_1+g_2}.
$$

Finally, choose an immersed circle $\gamma_l:S^1\to\mathbb R^2$ with exactly $l$ transverse double points and no other multiple points; one may add $l$ small figure-eight kinks to an embedded circle. Let $c:S^1\to\mathbb R^2$ be an embedded circle and define

$$
\iota(s,t)=\bigl(\gamma_l(s),c(t)\bigr).
$$

This [Product Lagrangian immersion](../../../../../product-lagrangian-immersion.md) satisfies $\iota^*\omega_0=0$. If $p$ is a double point of $\gamma_l$, its two local branches times $c(S^1)$ meet along $\{p\}\times c(S^1)$. Their tangent spaces intersect precisely in the tangent line to that circle, so the intersection is clean. The $l$ double points therefore give exactly $l$ disjoint clean self-intersection circles.

Near each clean circle, perturb one Lagrangian sheet by the graph of $\delta dh$ in its [Weinstein neighborhood](../../../../../weinstein-neighborhood-theorem.md), where $h:S^1\to\mathbb R$ is a [Morse function](../../../../../morse-function.md) with one minimum and one maximum. The clean circle is replaced by two transverse double points. Resolve both by [Lagrangian surgery](../../../../../lagrangian-surgery.md). Each resolution attaches one one-handle and lowers the Euler characteristic by two, so resolving all $l$ clean circles changes the Euler characteristic of the original torus from zero to

$$
0-2(2l)=-4l.
$$

Choose the orientation-reversing neck at one double point; the resulting connected surface is nonorientable, while all the surgeries remove their double points and leave an embedding. Thus the [Givental construction of nonorientable Lagrangian surfaces](../../../../../givental-construction-of-nonorientable-lagrangian-surfaces.md) gives a closed connected nonorientable surface of Euler characteristic $-4l$ Lagrangian embedded in $(\mathbb R^4,\omega_0)$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 146](../../paper-146-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
