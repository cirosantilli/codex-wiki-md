<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Generalized Stokes theorem](../../../../../../generalized-stokes-theorem.md) applied to the [closed differential one-form](../../../../../../closed-differential-one-form.md) gives

$$
\boxed{\rho_1(k)+\rho_2(\bar ak)+\rho_3(ak)=0.}
$$

Equivalently, the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) is

$$
\sum_{j=1}^3E(-ic_jk)\Phi_j(c_jk)
=-\frac i2\sum_{j=1}^3E(-ic_jk)\Psi_j(c_jk).
$$

The identical outward [Neumann boundary data](../../../../../../neumann-boundary-data.md) make the three known transforms equal:

$$
\Psi_j(k)=\Psi(k)=\int_{-l/2}^{l/2}e^{(k+\lambda/k)s}f(s)ds.
$$

To reduce the unknown traces to a single function, use rotation invariance and uniqueness. For $\lambda>0$ the difference $u$ of two solutions has zero outward derivative and

$$
\int_D|\nabla u|^2dA+4\lambda\int_D|u|^2dA=0,
$$

by [Green's first identity](../../../../../../green-s-first-identity.md). Thus $u=0$. Rotation by $a$ preserves the equation, the domain and the oriented boundary data, so it preserves $q$; hence $q^{(1)}=q^{(2)}=q^{(3)}=q$ and $\Phi_j=\Phi$. The [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) becomes the **single equation with three spectral unknowns**

$$
E(-ik)\Phi(k)+E(-i\bar ak)\Phi(\bar ak)+E(-iak)\Phi(ak)
=-\frac i2[E(-ik)\Psi(k)+E(-i\bar ak)\Psi(\bar ak)+E(-iak)\Psi(ak)].
$$

The three unknowns are evaluations of the same boundary transform, not three freely specified boundary data.

The printed allowance of all real $\lambda$ requires a qualification. At $\lambda=0$, existence requires $3\int_{-l/2}^{l/2}f(s)ds=0$ by the [divergence theorem](../../../../../../divergence-theorem.md), and solutions differ by a constant. Fixing a rotation-invariant normalization gives uniqueness and the same rotational conclusion. In fact the unnormalized solution is already invariant: its rotation difference is constant, and three successive rotations make three times that constant zero. For $\lambda<0$, uniqueness fails precisely when $-4\lambda$ is an [eigenvalue](../../../../../../eigenvalue.md) of the [Neumann Laplacian](../../../../../../neumann-laplacian.md). At these parameters identical data do not force an arbitrary solution to be rotationally invariant. Averaging any solution over the three rotations produces a solution with the common trace used here; the difference is a homogeneous [Neumann eigenfunction](../../../../../../neumann-eigenfunction.md), or a sum of them. Part (e) describes both solvability and this remaining freedom rather than assuming uniqueness for every real parameter.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
