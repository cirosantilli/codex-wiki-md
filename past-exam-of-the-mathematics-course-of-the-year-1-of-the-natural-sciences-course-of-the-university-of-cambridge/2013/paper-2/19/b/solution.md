<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First calculate the [curl](../../../../../curl.md):

$$
\nabla\times\mathbf F=(0,-2z,3y-1).
$$

By [Stokes theorem](../../../../../stokes-theorem.md), use the positively oriented equator $\mathbf r(\phi)=(a\cos\phi,a\sin\phi,0)$, $0\leq\phi\leq2\pi$. Its tangent is $a(-\sin\phi,\cos\phi,0)$, while the restricted field is $(0,3a^2\cos\phi\sin\phi-a\cos\phi,0)$. Thus

$$
\iint_S(\nabla\times\mathbf F)\cdot d\mathbf S
=\int_0^{2\pi}\left(3a^3\cos^2\phi\sin\phi-a^2\cos^2\phi\right)d\phi
=\boxed{-\pi a^2}.
$$

The first term integrates to zero over a full period and the second uses $\int_0^{2\pi}\cos^2\phi\,d\phi=\pi$.

One can also calculate directly on the curved [surface](../../../../../topological-surface-split.md). With [spherical coordinates](../../../../../spherical-coordinate-system.md) $0\leq\theta\leq\pi/2$, $0\leq\phi\leq2\pi$,

$$
d\mathbf S=a^2\sin\theta(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta)\,d\theta\,d\phi.
$$

Substitution gives the scalar integrand $a^3\sin^2\theta\cos\theta\sin\phi-a^2\sin\theta\cos\theta$. Its azimuthal [sine](../../../../../sine.md) term vanishes, and the rest gives $-2\pi a^2\int_0^{\pi/2}\sin\theta\cos\theta\,d\theta=-\pi a^2$, confirming the [orientation](../../../../../orientation-of-a-simplex.md) and the same result.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
