<h1 id="section-e/e14/solution">Solution</h1>

↑ **Parent:** [E14](../e14.md)

For a steady thin-wire [electric current](../../../../../electric-current.md), the [Biot-Savart law](../../../../../biot-savart-law.md) is

$$
d\mathbf B=\frac{\mu_0I}{4\pi}\frac{d\boldsymbol\ell\times\mathbf R}{R^3},
$$

where $\mathbf R$ points from the source element to the field point and $d\boldsymbol\ell$ follows positive [electric current](../../../../../electric-current.md). On a circular loop's axis the transverse contributions cancel by [symmetry](../../../../../symmetry-physics.md). The axial numerator is $a^2d\varphi$ and the distance is $\sqrt{a^2+z^2}$, giving

$$
B_z(z)=\frac{\mu_0I}{4\pi}\int_0^{2\pi}\frac{a^2\,d\varphi}{(a^2+z^2)^{3/2}},\qquad \boxed{B_z(z)=\frac{\mu_0I a^2}{2(a^2+z^2)^{3/2}}.}
$$

Its graph is positive and even, with maximum $\mu_0I/(2a)$ at the centre and a $|z|^{-3}$ far-field decay. Reversing the [electric current](../../../../../electric-current.md) reverses its sign.

For two equally oriented $N$-turn coils centred at $\pm D$, superposition gives

$$
B_{\rm ax}(z)=\frac{\mu_0NIa^2}{2}\left[\frac1{(a^2+(z-D)^2)^{3/2}}+\frac1{(a^2+(z+D)^2)^{3/2}}\right].
$$

Consequently

$$
\boxed{B_{\rm ax}(0)=\frac{\mu_0NIa^2}{(a^2+D^2)^{3/2}}.}
$$

This is an even differentiable function, so every odd derivative at zero vanishes, including the first and third. To check the second derivative explicitly, let $f(s)=(a^2+s^2)^{-3/2}$. Then

$$
f''(s)=\frac{3(4s^2-a^2)}{(a^2+s^2)^{7/2}},\qquad B_{\rm ax}''(0)=\frac{3\mu_0NIa^2(4D^2-a^2)}{(a^2+D^2)^{7/2}}.
$$

Thus **$2D=a$ makes the quadratic variation vanish**, which is the [Helmholtz coil](../../../../../helmholtz-coil.md) condition. The central value and leading axial variation are

$$
\boxed{B_0=\left(\frac45\right)^{3/2}\frac{\mu_0NI}{a},\qquad \frac{B_{\rm ax}(z)}{B_0}=1-\frac{144}{125}\left(\frac za\right)^4+O((z/a)^6).}
$$

<a id="section-e/e14/image-an-original-comparison-of-axial-field-uniformity-for-several-coil-separations"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1-helmholtz-profile.png)

**[Figure 7](#section-e/e14/image-an-original-comparison-of-axial-field-uniformity-for-several-coil-separations). An original comparison of axial field uniformity for several coil separations**.

Near the centre, the coils' [magnetic field lines](../../../../../magnetic-field-line.md) are nearly straight and parallel to the axis. On the axis rotational [symmetry](../../../../../symmetry-physics.md) makes $B_x=B_y=0$ exactly; in the central plane the radial components from the two coils cancel. More quantitatively, in the current-free central volume, axisymmetry and $\nabla\cdot\mathbf B=0$ imply

$$
B_r(r,z)=-\frac r2B_{\rm ax}'(z)+O(r^3),\qquad B_z(r,z)=B_{\rm ax}(z)-\frac{r^2}{4}B_{\rm ax}''(z)+O(r^4).
$$

The suppressed axial derivatives therefore also suppress transverse [magnetic fields](../../../../../magnetic-field-split.md) near the centre. The smallness applies locally compared with the coil radius; it is not a claim of an exactly uniform field throughout the apparatus.

## ↑ Ancestors (13)

1. [E14](../e14.md)
2. [Section E](../../section-e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
