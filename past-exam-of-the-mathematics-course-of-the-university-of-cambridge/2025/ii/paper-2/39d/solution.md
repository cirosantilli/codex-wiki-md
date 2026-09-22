<h1 id="39d/solution">Solution</h1>

↑ **Parent:** [39D](../39d.md)

At zero Reynolds number, an incompressible Newtonian fluid obeys the Stokes equations

$$
-\nabla p+\mu\nabla^2\mathbf u=0,
\qquad
\nabla\cdot\mathbf u=0.
$$

Taking the divergence gives $\nabla^2p=0$. Taking the curl and writing $\boldsymbol\omega=\nabla\times\mathbf u$ gives

$$
\mu\nabla^2\boldsymbol\omega=0.
$$

Thus both pressure and vorticity are harmonic in the fluid.

In the laboratory frame, the boundary conditions are

$$
\mathbf u\to0\quad(r\to\infty),
$$

and, on $r=a$,

$$
\mathbf u\cdot\mathbf n=\mathbf U\cdot\mathbf n,
\qquad
(\mathbf I-\mathbf n\mathbf n^T)\mathbf u
=(\mathbf I-\mathbf n\mathbf n^T)\mathbf U.
$$

The first is impermeability of the solid surface and the second is viscous no slip. Together they say $\mathbf u=\mathbf U$ on the sphere.

For the stated solution, put

$$
A(r)=\frac{3a}{4r}+\frac{a^3}{4r^3},
\qquad
B(r)=\frac{3a}{4r^3}-\frac{3a^3}{4r^5},
\qquad
s=\mathbf U\cdot\mathbf x.
$$

Then $u_j=AU_j+Bs x_j$, and

$$
\boxed{
\frac{\partial u_j}{\partial x_i}
=\frac{A'}r x_iU_j
+\frac{B'}r s x_ix_j
+B U_ix_j+B s\delta_{ij},}
$$

where

$$
A'=-\frac{3a}{4r^2}-\frac{3a^3}{4r^4},
\qquad
B'=-\frac{9a}{4r^4}+\frac{15a^3}{4r^6}.
$$

## ↑ Ancestors (10)

1. [39D](../39d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
