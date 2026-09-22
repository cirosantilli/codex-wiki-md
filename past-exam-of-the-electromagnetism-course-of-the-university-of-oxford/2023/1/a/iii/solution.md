<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Integrate the [surface charge density](../../../../../surface-charge-density.md) using the [surface integral](../../../../../surface-integral.md) in [spherical coordinates](../../../../../spherical-coordinate-system.md):

$$
Q=2\pi a^2\frac{q(a-r_0^2/a)}{4\pi}
\int_{-1}^1\frac{du}{(a^2+r_0^2-2ar_0u)^{3/2}}.
$$

Since $r_0>a$, the elementary integral is

$$
\frac1{ar_0}\left[\frac1{\sqrt{a^2+r_0^2-2ar_0u}}\right]_{-1}^1
=\frac1{ar_0}\left(\frac1{r_0-a}-\frac1{r_0+a}\right)
=\frac2{r_0(r_0^2-a^2)}.
$$

Substitution yields the total induced [electric charge](../../../../../electric-charge-split.md)

$$
\boxed{Q=-\frac{qa}{r_0}=q^\star.}
$$

The equality with the [image charge](../../../../../image-charge.md) also follows by applying [Gauss's law](../../../../../gauss-s-law.md) to the exterior [electric field](../../../../../electric-field-split.md): the physical and fictitious descriptions give the same [electric flux](../../../../../electric-flux.md) through a sphere enclosing the conductor but excluding the physical [point charge](../../../../../point-charge.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
