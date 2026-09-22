<h1 id="30a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The characteristic vector field $b=(\nabla_vH,-\nabla_xH)$ is a [divergence-free vector field](../../../../../../divergence-free-vector-field.md):

$$
\nabla_z\cdot b=\sum_{i=1}^n(H_{x_iv_i}-H_{v_ix_i})=0.
$$

The [Jacobian determinant](../../../../../../jacobian-determinant.md) $J_t=\det D\Phi_t$ obeys $\dot J_t=(\nabla\cdot b)(\Phi_t)J_t=0$, with $J_0=1$. Thus the flow preserves phase-space volume, the [Liouville theorem in Hamiltonian mechanics](../../../../../../liouville-s-theorem-hamiltonian.md). Changing variables $(x,v)=\Phi_t(\xi,\eta)$ and using (i) gives

$$
\boxed{\int_{\mathbb R^{2n}}F(f(x,v,t))\,dx\,dv=\int_{\mathbb R^{2n}}F(f_I(\xi,\eta))\,d\xi\,d\eta.}
$$

This applies on intervals where the flow is a diffeomorphism of the phase space and the integrals are defined; for finite conservation statements require integrability. For instance compactly supported initial data and $F(0)=0$ give the usual setting. An arbitrary smooth $F$ need not make these integrals finite on infinite-volume space, and merely smooth $H$ does not exclude escape of characteristics to infinity. Equivalently $F(f)_t+\nabla_z\cdot[bF(f)]=0$, with no flux through infinity, proves the same [Casimir invariant of a transport equation](../../../../../../casimir-invariant-of-a-transport-equation.md) conservation.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [30A](../../30a.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
