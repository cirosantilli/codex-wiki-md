<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the disk, the hemisphere reaches

$$
z_{\max,D}=R.
$$

For half of the strip surface, invert the first-order equation and integrate from the midpoint to the boundary:

$$
R=\int_0^{z_{\max,T}}
\frac{z^2\,dz}{\sqrt{z_{\max,T}^4-z^4}}
=z_{\max,T}\int_0^1
\frac{u^2\,du}{\sqrt{1-u^4}}.
$$

The [beta function](../../../../../../beta-function.md) integral is

$$
\int_0^1\frac{u^2\,du}{\sqrt{1-u^4}}
=\frac{\sqrt\pi\,\Gamma(3/4)}{\Gamma(1/4)}
\simeq0.59907.
$$

Therefore

$$
\boxed{z_{\max,T}
=\frac{\Gamma(1/4)}{\sqrt\pi\,\Gamma(3/4)}R
\simeq1.669R>R=z_{\max,D}}.
$$

The strip's holographic entropy surface lies deeper in the bulk than that of a disk with the same half-width or radius.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 354](../../../paper-354-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
