<h1 id="b5/solution">Solution</h1>

↑ **Parent:** [B5](../b5.md)

The [method of images](../../../../method-of-images.md) replaces conductors by fictitious charges outside the physical solution domain. Choose images so the real-plus-image potential obeys the specified conductor boundary values. The electrostatic uniqueness theorem then identifies that potential in the physical domain; fields inside the replaced conductor are not physical predictions.

Put the cylinder axis at the origin, real line at $(2a,0)$ and image at $(a/2,0)$. Let $r_1,r_2$ be distances from these lines. The exterior potential can be written

$$
\boxed{\phi=\frac{\lambda}{2\pi\epsilon_0}\ln\frac{2r_2}{r_1}.}
$$

On the surface, $r_1^2=a^2(5-4\cos\theta)$ and $r_2^2=r_1^2/4$, so $\phi=0$ everywhere as required. The additive constant is essential for a grounded cylinder; the two-dimensional potential need not also be zero at infinity.

The physical line feels the image field at separation $3a/2$. Its [force](../../../../force-split.md) per unit length is attractive:

$$
\boxed{\frac{\mathbf F}{\mathcal L}=-\frac{\lambda^2}{3\pi\epsilon_0a}\,\hat{\mathbf x}.}
$$

Measure $\theta$ from the radius toward the real line, as in the original diagram. The radial field just outside the surface is

$$
E_r=\frac\lambda{2\pi\epsilon_0}
\left[\frac{a-2a\cos\theta}{a^2(5-4\cos\theta)}
-\frac{a-(a/2)\cos\theta}{(a^2/4)(5-4\cos\theta)}\right].
$$

Since the interior field is zero,

$$
\boxed{\sigma(\theta)=\epsilon_0E_r=-\frac{3\lambda}{2\pi a(5-4\cos\theta)}.}
$$

Integrating $a\sigma(\theta)$ around the circumference gives total induced charge $-\lambda$ per unit length.

<a id="b5/image-original-calculated-exterior-equipotentials-and-induced-surface-charge-distribution-for-the-grounded-cylinder-conductor-interior-excluded-from-the-field-solution"></a>
![](../../../../past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1-gpp2014-cylinder-image.png)

**[Figure 1](#b5/image-original-calculated-exterior-equipotentials-and-induced-surface-charge-distribution-for-the-grounded-cylinder-conductor-interior-excluded-from-the-field-solution). Original calculated exterior equipotentials and induced surface-charge distribution for the grounded cylinder; conductor interior excluded from the field solution**.

## ↑ Ancestors (12)

1. [B5](../b5.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
