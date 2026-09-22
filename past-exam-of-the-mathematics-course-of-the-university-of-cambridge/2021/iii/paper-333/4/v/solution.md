<h1 id="4/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Define the perturbation vorticity component

$$
\zeta'=u'_z-w'_x.
$$

Taking the curl of the linear momentum equation and using the buoyancy equation gives

$$
(\partial_t+U\partial_x)\zeta'=-b'_x,
\qquad
(\partial_t+U\partial_x)b'=-N^2w'.
$$

Multiply the first equation by $b'$, the second by $\zeta'$, and horizontally average. Periodicity makes the averaged $x$ derivatives vanish, while

$$
\overline{w'\zeta'}
=\overline{w'u'_z-w'w'_x}
=\partial_z\overline{u'w'}
$$

by incompressibility and [integration by parts](../../../../../../integration-by-parts.md). It follows that

$$
\partial_t\overline{b'\zeta'}
=-N^2\partial_z\overline{u'w'}.
$$

Therefore the [wave activity](../../../../../../wave-activity.md) conservation law is

$$
\boxed{
\partial_t\mathcal A+\partial_z\mathcal F_{\mathcal A}=0,
\qquad
\mathcal A=-\frac{\overline{b'\zeta'}}{N^2},
\qquad
\mathcal F_{\mathcal A}=-\overline{u'w'}
}.
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [4](../../4.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
