<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the **number-density [virial expansion](../../../../../virial-expansion.md)**, following the [density versus molar second virial convention](../../../../../density-versus-molar-second-virial-convention.md), with $n=N/V$:

$$
\frac{p}{nk_BT}=1+B_2(T)n+O(n^2).
$$

Thus $B_2$ is the coefficient of the first [density](../../../../../density.md) correction and has units of [volume](../../../../../volume.md). With molar [density](../../../../../density.md) instead, the molar coefficient is $N_AB_2$. For a classical pair potential $u(r)$,

$$
\boxed{B_2(T)=-\frac12\int\left(e^{-u(r)/(k_BT)}-1\right)d^3r=2\pi\int_0^\infty\left[1-e^{-u(r)/(k_BT)}\right]r^2dr.}
$$

Attractive separations contribute negatively and short-range repulsion contributes positively. For inert-gas interactions the attractive contribution dominates at sufficiently low [temperature](../../../../../temperature-split.md), $B_2$ crosses zero at the [Boyle temperature](../../../../../boyle-temperature.md), and repulsion dominates above it.

<a id="1/a/image-an-illustrative-lennard-jones-second-virial-coefficient-is-negative-at-low-temperature-crosses-zero-and-has-a-broad-positive-maximum"></a>
![](../../../../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2016/paper-1-second-virial.png)

**[Figure 1](#1/a/image-an-illustrative-lennard-jones-second-virial-coefficient-is-negative-at-low-temperature-crosses-zero-and-has-a-broad-positive-maximum). An illustrative Lennard-Jones second virial coefficient is negative at low temperature, crosses zero and has a broad positive maximum**. [Source](paper-1-second-virial.py).

The [soft-core high-temperature second virial coefficient](../../../../../soft-core-high-temperature-second-virial-coefficient.md) illustrates why the far-high-temperature tail depends on the model. A hard-core estimate $B_2\simeq b-a/(k_BT)$ tends to positive excluded [volume](../../../../../volume.md) $b$. A soft repulsive potential, such as the [Lennard-Jones potential](../../../../../lennard-jones-potential.md) in the original diagram, allows a positive maximum followed by decay toward zero. The sign change is the main attraction-versus-repulsion feature; neither sketch should be interpreted as measured data for a specified gas. This classical, dilute-gas sketch omits low-temperature quantum-exchange corrections.[Section 2.5: interacting gas, virial expansion and Mayer pair function](../../../../../classical-gases-by-david-tong.md)

## ↑ Ancestors (14)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
