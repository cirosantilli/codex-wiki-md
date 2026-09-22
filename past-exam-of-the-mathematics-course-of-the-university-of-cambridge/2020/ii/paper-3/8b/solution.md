<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

The repulsive force is $\mathbf F=k\mathbf r/r^3=-\nabla(k/r)$, so the [Hamiltonian](../../../../../hamiltonian.md) is

$$
H=\frac{\mathbf p^2}{2m}+\frac kr.
$$

The [Hamilton's equations](../../../../../hamilton-s-equations.md) give $\dot{\mathbf r}=\mathbf p/m$ and $\dot{\mathbf p}=k\mathbf r/r^3$. Consequently

$$
\dot{\mathbf L}
=\dot{\mathbf r}\times\mathbf p+\mathbf r\times\dot{\mathbf p}=\mathbf0,
$$

so the [angular momentum](../../../../../angular-momentum.md) is conserved. Moreover,

$$
\dot{\mathbf p}\times\mathbf L
=k\left(\frac{\mathbf r(\mathbf r\cdot\mathbf p)}{r^3}-\frac{\mathbf p}{r}\right)
=-mk\frac{d\widehat{\mathbf r}}{dt}.
$$

It follows that the [Laplace-Runge-Lenz vector](../../../../../laplace-runge-lenz-vector.md) $\mathbf A=\mathbf p\times\mathbf L+mk\widehat{\mathbf r}$ is conserved. By the [Hamiltonian conservation law](../../../../../hamiltonian-conservation-law.md), these time derivatives are exactly $\{\mathbf L,H\}$ and $\{\mathbf A,H\}$, so both [Poisson brackets](../../../../../poisson-bracket.md) vanish.

The [integrals of motion](../../../../../integral-of-motion.md) are the energy $H$, the components of $\mathbf L$, and the components of $\mathbf A$, subject to

$$
\mathbf A\cdot\mathbf L=0,
\qquad
A^2=m^2k^2+2mHL^2.
$$

Taking the [dot product](../../../../../dot-product.md) of $\mathbf A$ with $\widehat{\mathbf r}$ gives

$$
A\cos\theta=\frac{L^2}{r}+mk.
$$

Therefore the [polar equation of a repulsive inverse-square orbit](../../../../../polar-equation-of-a-repulsive-inverse-square-orbit.md) is

$$
r=\frac{L^2/(mk)}{(A/(mk))\cos\theta-1}
=\frac{\lambda}{e\cos\theta-1},
$$

where $\lambda=L^2/(mk)\geq0$ and $e=A/(mk)\geq0$. For a nonradial physical scattering orbit $H>0$, the identity above gives $e>1$, as expected for a [hyperbolic Kepler orbit](../../../../../hyperbolic-kepler-orbit.md).

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
