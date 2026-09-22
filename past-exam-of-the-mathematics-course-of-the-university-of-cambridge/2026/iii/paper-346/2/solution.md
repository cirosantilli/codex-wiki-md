<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\bar\rho(t)$ be the homogeneous density. A [Lagrangian coordinate](../../../../../lagrangian-coordinate.md) volume $d^3q$ contains the same mass as its image $d^3x$ under the [Zeldovich approximation](../../../../../zeldovich-approximation.md), so [mass conservation](../../../../../mass-conservation.md) gives

$$
\rho(\mathbf x,t)d^3x=\bar\rho(t)d^3q,
\qquad
d^3x=|J|d^3q,
\qquad
J=\det\!\left(\frac{\partial\mathbf x}{\partial\mathbf q}\right).
$$

Since $1+\delta=\rho/\bar\rho$, the [density contrast](../../../../../density-contrast.md) is

$$
\boxed{1+\delta(\mathbf x,t)=|J|^{-1}}.
$$

For $\mathbf s=-\nabla_q\Phi$, the deformation tensor is

$$
d_{ij}=\frac{\partial s_i}{\partial q_j}
=-\frac{\partial^2\Phi}{\partial q_i\partial q_j}.
$$

Equality of mixed partial derivatives makes it a real [symmetric matrix](../../../../../symmetric-matrix.md). The [real spectral theorem](../../../../../real-spectral-theorem.md) therefore supplies an orthonormal eigenbasis and real eigenvalues, which we denote by $-\lambda_1,-\lambda_2,-\lambda_3$. In that basis,

$$
\frac{\partial x_i}{\partial q_j}
=\delta_{ij}+Dd_{ij}
=\operatorname{diag}(1-D\lambda_1,1-D\lambda_2,1-D\lambda_3),
$$

and hence

$$
\boxed{1+\delta=\prod_{i=1}^3|1-D(t)\lambda_i|^{-1}}.
$$

Before the first crossing all factors are positive, allowing the absolute values to be omitted.

When $1-D\lambda_i=0$, the map loses rank in the corresponding principal direction. Its [Jacobian determinant](../../../../../jacobian-determinant.md) vanishes, trajectories meet, and [shell crossing](../../../../../shell-crossing.md) creates a [cosmological caustic](../../../../../cosmological-caustic.md). The single-stream pressureless density formally diverges and the approximation no longer describes the subsequent multistream dynamics. If only one $\lambda_i$ is positive, one axis first collapses while the other two remain extended, producing a sheet or pancake. Collapse along a second and then a third principal axis produces filaments and nodes. Spatial variation of the eigenvalues joins these objects into the [cosmic web](../../../../../cosmic-web.md) around underdense voids.

The approximation succeeds because it reproduces linear growing-mode evolution exactly, preserves the initial tidal displacement and anisotropic collapse, and follows matter along nearly inertial comoving trajectories instead of expanding only the density at a fixed point. Large scales remain weakly nonlinear and are insensitive to the detailed dynamics after crossing. Its limitations begin at [shell crossing](../../../../../shell-crossing.md): it permits streams to pass through one another, cannot produce virialized halos, and omits velocity dispersion, vorticity, gas pressure, shocks, feedback, and strongly nonlinear self-gravity.

For the one-dimensional displacement,

$$
\boxed{x(q,t)=q-D(t)A\sin(kq)},
\qquad
\frac{\partial x}{\partial q}=1-D(t)Ak\cos(kq),
$$

so mass conservation gives

$$
\boxed{1+\delta(x,t)=|1-D(t)Ak\cos(kq)|^{-1}}.
$$

The earliest crossing occurs where the cosine is maximal:

$$
\boxed{D(t_c)Ak=1},
\qquad
q_n=\frac{2\pi n}{k},
\qquad
x_n=q_n,
$$

for integers $n$. The denominator vanishes at these isolated points.

Write $u=q-q_n$ at $t=t_c$. The [Taylor series](../../../../../taylor-series.md) gives

$$
x-x_n=u-\frac1k\sin(ku)
=\frac{k^2u^3}{6}+O(u^5),
\qquad
\frac{\partial x}{\partial q}
=\frac{k^2u^2}{2}+O(u^4).
$$

Thus $|u|\sim(6|x-x_n|/k^2)^{1/3}$ and

$$
1+\delta
\sim\frac{2}{k^2u^2}
=\frac{2}{6^{2/3}}\frac1{|k(x-x_n)|^{2/3}}.
$$

The first caustic is therefore a cubic cusp with

$$
\boxed{\rho\propto|x-x_n|^{-2/3}}.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
