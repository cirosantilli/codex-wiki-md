<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For any interior point $\mathbf p$, choose a sufficiently small circle centred on $\mathbf p$ and wholly inside the disk. Translating the origin does not change the [Laplace equation](../../../../../laplace-equation.md), so part (b) gives

$$
\Psi(\mathbf p)=\frac1{2\pi}\int_0^{2\pi}\Psi(\mathbf p+\rho(\cos\theta,\sin\theta))\,d\theta.
$$

Suppose a real [harmonic function](../../../../../harmonic-function.md), continuous on the closed disk, attains its global maximum $M$ at an interior point. Every value on each such circle is at most $M$, and their average is $M$. By continuity, every value on the circle must therefore equal $M$. Varying its radius shows that a neighbourhood of the point also has value $M$.

Thus the set of points attaining $M$ is open in the disk, and it is closed by continuity. The disk is connected, so this set must be the whole disk. The function is constant and has the same maximum on the boundary. Otherwise the maximum cannot be interior. Compactness of the closed disk guarantees existence of a maximum, proving the [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md):

$$
\boxed{\max_{r\leq R}\Psi=\max_{r=R}\Psi}.
$$

Continuity up to the boundary is the standard hypothesis for this attained-maximum formulation.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
