<h1 id="36d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the [radiation zone](../../../../../../radiation-zone.md), both fields are transverse to $\widehat{\mathbf x}$ and obey

$$
\mathbf E_0=-c\widehat{\mathbf x}\times\mathbf B_0,
\qquad
|\mathbf E_0|=c|\mathbf B_0|.
$$

The outward [Poynting vector](../../../../../../poynting-vector.md) is

$$
\mathbf S
=\frac1{\mu_0}\mathbf E\times\mathbf B
=\frac c{\mu_0}|\mathbf B_0|^2
\sin^2(\omega t-\mathbf k\mathbin\cdot\mathbf x)
\widehat{\mathbf x},
$$

so its [time average](../../../../../../eulerian-time-average.md) is

$$
\langle S_r\rangle=\frac c{2\mu_0}|\mathbf B_0|^2.
$$

An absorbing shell receives the incident momentum rather than reversing it. Hence [radiation pressure on a perfectly absorbing surface](../../../../../../radiation-pressure-on-a-perfectly-absorbing-surface.md) gives

$$
p(\widehat{\mathbf x})
=\frac{\langle S_r\rangle}{c}
=\frac{|\mathbf B_0|^2}{2\mu_0}.
$$

At $r=R$,

$$
|\mathbf B_0|^2
=\frac{\mu_0^2\omega^4}{16\pi^2R^2c^2}
|\widehat{\mathbf x}\times\mathbf p_0|^2,
$$

and therefore

$$
\boxed{
p(\widehat{\mathbf x})
=\frac{\mu_0\omega^4}{32\pi^2R^2c^2}
|\widehat{\mathbf x}\times\mathbf p_0|^2}.
$$

If $\vartheta$ is the angle between $\widehat{\mathbf x}$ and $\mathbf p_0$, this is

$$
p(\vartheta)=
\frac{\mu_0\omega^4|\mathbf p_0|^2}
{32\pi^2R^2c^2}\sin^2\vartheta.
$$

Its spherical average is $\mu_0\omega^4|\mathbf p_0|^2/(48\pi^2R^2c^2)$; the vector force integrates to zero by the inversion symmetry of the [electric dipole radiation](../../../../../../electric-dipole-radiation.md) pattern.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [36D](../../36d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
