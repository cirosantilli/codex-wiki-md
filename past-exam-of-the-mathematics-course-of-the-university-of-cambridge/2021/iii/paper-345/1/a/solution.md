<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With buoyancy perturbation $b=-g\rho'/\rho_0$, the inviscid [Boussinesq equations](../../../../../../boussinesq-equations.md) are

$$
\frac{D\mathbf u}{Dt}=-\frac1{\rho_0}\nabla p+b\widehat{\mathbf z},
\qquad
\nabla\mathbin{\cdot}\mathbf u=0,
\qquad
\frac{Db}{Dt}+N^2w=0.
$$

For

$$
\mathbf u=\nabla\times(\psi\widehat{\mathbf y})
=(-\psi_z,0,\psi_x),
$$

incompressibility is automatic. Define the [Jacobian determinant](../../../../../../jacobian-determinant.md)

$$
J(A,B)=A_xB_z-A_zB_x.
$$

The material derivative is $D/Dt=\partial_t+J(\psi,\mathord\cdot)$. Taking the $y$ component of the curl of momentum gives the exact finite-amplitude system

$$
\boxed{
\partial_t\nabla^2\psi+J(\psi,\nabla^2\psi)=b_x,
}
$$



$$
\boxed{
\partial_tb+J(\psi,b)+N^2\psi_x=0.
}
$$

If the disturbance amplitude is small enough that each Jacobian is asymptotically smaller than its corresponding time derivative, the system can be linearized. Eliminating $b$ then gives

$$
\boxed{
\partial_t^2\nabla^2\psi+N^2\partial_x^2\psi=0
}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
