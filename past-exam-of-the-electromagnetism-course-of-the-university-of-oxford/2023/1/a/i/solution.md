<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [image charge for a grounded conducting sphere](../../../../../image-charge-for-a-grounded-conducting-sphere.md) is obtained by the [Kelvin transform](../../../../../kelvin-transform.md):

$$
\boxed{q^\star=-\frac{a}{r_0}q,\qquad \mathbf r^\star=\frac{a^2}{r_0^2}\mathbf r_0=\left(0,0,\frac{a^2}{r_0}\right).}
$$

It lies inside the [electrical conductor](../../../../../electrical-conductor.md), outside the region where it represents the physical [electric field](../../../../../electric-field-split.md). The [electric potential](../../../../../electric-potential.md) is

$$
\boxed{\phi(\mathbf r)=\begin{cases}
0,&r\leq a,\\[2pt]
\displaystyle\frac1{4\pi\epsilon_0}\left(\frac q{|\mathbf r-\mathbf r_0|}-\frac{qa/r_0}{|\mathbf r-\mathbf r^\star|}\right),&r>a,\quad\mathbf r\ne\mathbf r_0.
\end{cases}}
$$

At the physical [point charge](../../../../../point-charge.md), the [electric potential](../../../../../electric-potential.md) has its usual [Coulomb's law](../../../../../coulomb-s-law.md) singularity. There is no physical singularity at the [image charge](../../../../../image-charge.md): the interior expression is identically zero.

For $|\mathbf r|=a$, direct expansion of squared distances gives

$$
|\mathbf r-\mathbf r^\star|^2
=a^2+\frac{a^4}{r_0^2}-\frac{2a^2}{r_0^2}\mathbf r\cdot\mathbf r_0
=\frac{a^2}{r_0^2}|\mathbf r-\mathbf r_0|^2.
$$

Consequently the two terms cancel exactly, proving the zero [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) on the sphere. At infinity each term is $O(r^{-1})$, and more explicitly

$$
\phi(\mathbf r)=\frac{q(1-a/r_0)}{4\pi\epsilon_0r}+O(r^{-2})\longrightarrow0.
$$

Thus the [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) at infinity also holds. The candidate solves the [Poisson equation](../../../../../poisson-s-equation.md) with the one physical [point charge](../../../../../point-charge.md); [uniqueness of Poisson equation](../../../../../uniqueness-of-poisson-equation.md), with these [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), identifies it as the required [electric potential](../../../../../electric-potential.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
