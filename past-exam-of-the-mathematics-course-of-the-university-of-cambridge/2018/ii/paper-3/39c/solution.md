<h1 id="39c/solution">Solution</h1>

↑ **Parent:** [39C](../39c.md)

For each incompressible [Stokes flow](../../../../../stokes-flow-split.md) without body force, $\partial_j\sigma_{ij}=0$ and

$$
\sigma_{ij}=-p\delta_{ij}+2\mu e_{ij},
\qquad
e_{ij}=\frac12(\partial_i u_j+\partial_j u_i).
$$

The [divergence theorem](../../../../../divergence-theorem.md) gives

$$
\int_Su_i^{(1)}\sigma_{ij}^{(2)}n_j\,dS
=\int_V\partial_j u_i^{(1)}\sigma_{ij}^{(2)}\,dV.
$$

Incompressibility removes the pressure term, antisymmetric velocity-gradient parts do not contract with the symmetric stress, and the remaining integrand is $2\mu e_{ij}^{(1)}e_{ij}^{(2)}$, symmetric under $1\leftrightarrow2$. This proves the [Lorentz reciprocal theorem for Stokes flow](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md):

$$
\boxed{\int_Su_i^{(1)}\sigma_{ij}^{(2)}n_j\,dS
=\int_Su_i^{(2)}\sigma_{ij}^{(1)}n_j\,dS.}
$$

By [Linearity of Stokes flow](../../../../../linearity-of-stokes-flow.md), the drag on a translating body is linear in its velocity, so $F_i=A_{ij}U_j$. Apply the reciprocal theorem to two translation solutions with velocities $\mathbf U^{(1)}$ and $\mathbf U^{(2)}$. Their surface velocities are constant and the far-field contribution vanishes, yielding

$$
U_i^{(1)}A_{ij}U_j^{(2)}=U_i^{(2)}A_{ij}U_j^{(1)}.
$$

Since the two vectors are arbitrary,

$$
\boxed{A_{ij}=A_{ji}.}
$$

Thus the [hydrodynamic resistance matrix](../../../../../hydrodynamic-resistance-matrix.md) is symmetric and, for fixed fluid viscosity, depends only on body geometry.

A straight rod has fore-aft symmetry about its centre. Gravity acts through that centre, so the translational-rotational coupling and applied torque vanish. [Kinematic reversibility of Stokes flow](../../../../../kinematic-reversibility-of-stokes-flow.md) and [Uniqueness of Stokes flow](../../../../../uniqueness-of-stokes-flow.md) then rule out spontaneous rotation: the inclination $\theta$ remains constant.

Let the speed for perpendicular translation be $U_0$. The given factor of two makes the parallel speed $2U_0$ for the same force component. Resolving gravity parallel and perpendicular to the rod gives

$$
U_\parallel=2U_0\cos\theta,
\qquad
U_\perp=U_0\sin\theta.
$$

Resolving these velocities horizontally and vertically gives

$$
U_H=U_0\sin\theta\cos\theta,
\qquad
U_V=U_0(1+\cos^2\theta).
$$

Therefore

$$
\boxed{\tan\phi=\frac{U_H}{U_V}
=\frac{\sin\theta\cos\theta}{1+\cos^2\theta}.}
$$

## ↑ Ancestors (10)

1. [39C](../39c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
