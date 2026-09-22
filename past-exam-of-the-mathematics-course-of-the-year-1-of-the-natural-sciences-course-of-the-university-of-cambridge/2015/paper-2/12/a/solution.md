<h1 id="12/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Orient the common axis of the wedge faces along $z$ and its azimuthal bisector along positive $x$. Reflection symmetries give $\bar y=\bar z=0$. In [spherical coordinates](../../../../../spherical-coordinate-system.md), use $0\leq r\leq a$, $0\leq\theta\leq\pi$, and $-\beta/2\leq\varphi\leq\beta/2$. The [volume](../../../../../volume.md) is

$$
V=\int_0^a r^2\,dr\int_0^\pi\sin\theta\,d\theta\int_{-\beta/2}^{\beta/2}d\varphi
=\frac{2\beta a^3}{3}.
$$

Since $x=r\sin\theta\cos\varphi$, the first moment is

$$
\int_Vx\,dV=\left(\frac{a^4}{4}\right)
\left(\int_0^\pi\sin^2\theta\,d\theta\right)
\left(\int_{-\beta/2}^{\beta/2}\cos\varphi\,d\varphi\right)
=\frac{\pi a^4}{4}\sin\frac\beta2.
$$

Dividing by the [volume](../../../../../volume.md) locates the [centre of mass](../../../../../center-of-mass.md):

$$
\boxed{\bar{\mathbf x}=\frac{3\pi a}{8\beta}\sin\frac\beta2\,\mathbf e_x},\qquad
\boxed{f(\beta)=\frac{3\pi}{8\beta}\sin\frac\beta2}.
$$

This is the centroid formula for a [spherical wedge](../../../../../spherical-wedge.md).

For the sketch, $f$ is positive and decreases from $\lim_{\beta\to0^+}f=3\pi/16$ to $\lim_{\beta\to2\pi^-}f=0$, with $f(\pi)=3/8$. Indeed, on putting $q=\beta/2$, the sign of $f'$ is the sign of $q\cos q-\sin q$. The negative of this expression has [derivative](../../../../../derivative.md) $q\sin q>0$ for $0<q<\pi$ and starts at zero, proving strict decrease.

<a id="12/a/image-distance-of-the-centre-of-mass-of-a-spherical-wedge-from-its-sphere-centre"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2-spherical-wedge-centroid.png)

**[Figure 1](#12/a/image-distance-of-the-centre-of-mass-of-a-spherical-wedge-from-its-sphere-centre). Distance of the centre of mass of a spherical wedge from its sphere centre**.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [12](../../12.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
