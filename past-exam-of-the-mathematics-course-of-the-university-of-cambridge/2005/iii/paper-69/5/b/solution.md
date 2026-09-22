<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The sine vectors $v_j^{(m)}=\sin(j\theta_m)$, $\theta_m=m\pi/J$, simultaneously diagonalize these two symmetric [tridiagonal matrices](../../../../../../tridiagonal-matrix.md). Their [eigenvalues](../../../../../../eigenvalue.md) are

$$
M:\quad\frac h3(2+\cos\theta_m),\qquad
K:\quad\frac2h(1-\cos\theta_m).
$$

Thus the semidiscrete decay rates are $\lambda_m=6(1-\cos\theta_m)/[h^2(2+\cos\theta_m)]$. The [Forward Euler method](../../../../../../euler-method.md) multiplies each mode by $1-k\lambda_m$. [Stability](../../../../../../stability-of-a-numerical-method.md) requires $0\leq k\lambda_m\leq2$ for every mode.

For a fixed finite Dirichlet grid the largest mode is $\theta_{J-1}=\pi-\pi/J$. Consequently the exact finite-grid bound is

$$
\boxed{0\leq\mu\leq\frac{2-\cos(\pi/J)}{3(1+\cos(\pi/J))},\qquad \mu=k/h^2.}
$$

As the mesh is refined, the upper bound decreases to $1/6$. Hence the mesh-independent answer is **$\boxed{0\leq\mu\leq1/6}$**. This is the [forward Euler limit for a consistent hat mass matrix](../../../../../../forward-euler-limit-for-a-consistent-hat-mass-matrix.md). The frequently seen $1/2$ diffusion bound belongs to the standard second-difference scheme or a lumped [mass matrix](../../../../../../mass-matrix.md), and is not the bound for the consistent Galerkin equations derived here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
