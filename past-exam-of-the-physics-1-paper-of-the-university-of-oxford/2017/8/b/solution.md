<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the rotation axis as $z$. A slice of the uniform sphere at coordinate $z$ is a disc of radius $R(z)=\sqrt{a^2-z^2}$ and [mass](../../../../mass.md) $dm=\rho\pi(a^2-z^2)\,dz$, where $\rho=3M/(4\pi a^3)$ is its [mass density](../../../../density.md). Applying [a](../a.md) to the slice gives

$$
dI=\frac12R(z)^2\,dm
=\frac{\rho\pi}{2}(a^2-z^2)^2\,dz.
$$

The slices' axes coincide, so no displaced-axis correction is needed. Integrating,

$$
\begin{aligned}
I&=\frac{\rho\pi}{2}\int_{-a}^a(a^4-2a^2z^2+z^4)\,dz\\
&=\frac{\rho\pi}{2}\left(2a^5-\frac43a^5+\frac25a^5\right)
=\frac{8\pi\rho a^5}{15}.
\end{aligned}
$$

Thus the [moment of inertia of a uniform solid sphere](../../../../moment-of-inertia-of-a-uniform-solid-sphere.md) is

$$
\boxed{I=\frac25Ma^2.}
$$

The sphere's [rotational symmetry](../../../../rotational-symmetry.md) makes this valid about every central axis. A thin spherical shell would have a different [mass distribution](../../../../mass-distribution.md) and a different [moment of inertia](../../../../moment-of-inertia.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
