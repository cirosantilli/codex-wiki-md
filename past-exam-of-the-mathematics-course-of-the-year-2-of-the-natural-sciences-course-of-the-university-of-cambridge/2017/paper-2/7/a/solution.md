<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use displacements $x_i$ from an [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md), so the two spring extensions are $x_2-x_1$ and $x_3-x_2$. The [kinetic energy](../../../../../kinetic-energy.md) and [elastic potential energy](../../../../../elastic-energy.md) are

$$
\boxed{T=\frac m2(\dot x_1^2+\mu\dot x_2^2+\dot x_3^2),\qquad V=\frac k2\big[(x_2-x_1)^2+(x_3-x_2)^2\big].}
$$

Thus $T=\dot x^TM\dot x/2$ and $V=x^TKx/2$, with the [small-oscillation mass and stiffness matrices](../../../../../small-oscillation-mass-and-stiffness-matrices.md)

$$
\boxed{M=m\begin{pmatrix}1&0&0\\0&\mu&0\\0&0&1\end{pmatrix},\qquad K=k\begin{pmatrix}1&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix}.}
$$

If $x_i$ instead denote absolute positions, the appropriate natural spring lengths must first be subtracted from the differences in $V$. They do not affect the equations for displacements.

[Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) give $M\ddot x+Kx=0$, so a [normal mode](../../../../../normal-mode.md) $x=ve^{i\omega t}$ obeys the [generalized eigenvalue problem for small oscillations](../../../../../generalized-eigenvalue-problem-for-small-oscillations.md) $Kv=\omega^2Mv$. Reflection symmetry separates antisymmetric shapes $(A,0,-A)^T$ from symmetric shapes $(A,B,A)^T$. In the antisymmetric sector the end equation is $kA=m\omega^2A$, giving $\omega^2=k/m$. In the symmetric sector the two independent equations are

$$
k(A-B)=m\omega^2A,\qquad2k(B-A)=\mu m\omega^2B.
$$

Twice the first plus the second gives $m\omega^2(2A+\mu B)=0$. If $\omega=0$, then $B=A$. Otherwise $B=-2A/\mu$, and substitution into the first equation gives $\omega^2=(k/m)(1+2/\mu)$. Thus the three independent shapes are:

$$
\begin{array}{c|c|c}
&v&\omega^2\\\hline
0&(1,1,1)^T&0\\
1&(1,0,-1)^T&k/m\\
2&(1,-2/\mu,1)^T&(k/m)(1+2/\mu)
\end{array}.
$$

For $v_0$ both springs retain their lengths, so this is uniform translation. For $v_1$ the end masses move oppositely and their forces on the middle mass cancel. For $v_2$ the end masses move together, while the middle mass moves oppositely so the [centre of mass](../../../../../center-of-mass.md) remains fixed. Direct substitution verifies all three eigenpairs; for positive $m,k,\mu$ the three [eigenvalues](../../../../../eigenvalue.md) are distinct and exhaust the three degrees of freedom. These are the [normal modes of three masses connected by two equal springs](../../../../../normal-modes-of-three-masses-connected-by-two-equal-springs.md).

A useful normalization is the [weighted inner product](../../../../../weighted-inner-product.md) induced by $M$. Since the squared mass norms are $m(\mu+2)$, $2m$ and $m(2+4/\mu)$, respectively, take

$$
\boxed{q_0=\frac{v_0}{\sqrt{m(\mu+2)}},\quad q_1=\frac{v_1}{\sqrt{2m}},\quad q_2=\frac{v_2}{\sqrt{m(2+4/\mu)}},\qquad q_i^TMq_j=\delta_{ij}.}
$$

If ordinary Euclidean unit [eigenvectors](../../../../../eigenvector.md) are intended instead, divide $v_0,v_1,v_2$ by $\sqrt3,\sqrt2,\sqrt{2+4/\mu^2}$, respectively. The frequencies and physical motions are independent of this normalization choice. The zero-frequency coordinate has general motion $A+Bt$ rather than an oscillation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
