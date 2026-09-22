<h1 id="h/h2/solution">Solution</h1>

↑ **Parent:** [H2](../h2.md)

By reflection symmetry, $G$ is the midpoint of the [cylinder](../../../../cylinder-geometry.md) axis. With position $r$ measured from $G$, define $J^G_{ij}=\int(|r|^2\delta_{ij}-r_ir_j)\,dm$. Symmetry makes the off-diagonal entries zero. Uniform [density](../../../../probability-density-function.md) gives $\langle x^2\rangle=\langle y^2\rangle=a^2/4$ and $\langle z^2\rangle=b^2/3$, by integrating over a disk and the [interval](../../../../interval-mathematics.md) $[-b,b]$. Hence

$$
\boxed{J^G=M\operatorname{diag}(a^2/4+b^2/3,\ a^2/4+b^2/3,\ a^2/2).}
$$

For parallel axes based at $P$, the tensor form of the parallel-axis theorem is $J^P=J^G+M(|d|^2I-dd^T)$, where $d=\overrightarrow{PG}$. This follows by substituting $r+d$ in the defining integral and using $\int r\,dm=0$. Here $d$ is an axial vector of length $b$, so

$$
\boxed{A=M(a^2/4+4b^2/3),\quad C=Ma^2/2,\qquad J^P=\operatorname{diag}(A,A,C).}
$$

The [Euler angles](../../../../euler-angles.md) $\psi,\phi$ are [cyclic coordinates](../../../../cyclic-coordinate.md). Their conserved conjugate momenta are $p_\psi=C(\dot\psi+\dot\phi\cos\theta)=Cn$ and $p_\phi=A\dot\phi\sin^2\theta+Cn\cos\theta=h$. The [Lagrangian](../../../../lagrangian.md) has no explicit time dependence, so the conserved energy is kinetic plus gravitational potential, namely the expression given with constant $E$.

Eliminate the angular velocities using $\dot\phi=(h-Cn\cos\theta)/(A\sin^2\theta)$ and $\dot\psi+\dot\phi\cos\theta=n$. The energy equation becomes

$$
A\dot\theta^2=2E-Cn^2+2Mgb\cos\theta-\frac{(h-Cn\cos\theta)^2}{A\sin^2\theta}.
$$

Thus

$$
\boxed{F(\theta)=A\sin^2\theta(2E-Cn^2+2Mgb\cos\theta)-(h-Cn\cos\theta)^2.}
$$

The elimination is valid away from the coordinate poles; the multiplied equation extends by [continuity](../../../../continuous-function.md) to any pole reached by a regular motion.

## ↑ Ancestors (12)

1. [H2](../h2.md)
2. [H](../../h.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
