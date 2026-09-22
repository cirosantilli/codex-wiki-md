<h1 id="section-a/a1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here the [complex viscoelastic modulus](../../../../../dynamic-modulus.md) is a stress-to-strain response coefficient, rather than a complex number's absolute value. Use strain $\gamma(t)=\operatorname{Re}(\gamma_0e^{i\omega t})$ and stress $\tau(t)=\operatorname{Re}[G^*(\omega)\gamma_0e^{i\omega t}]$, with

$$
\boxed{G^*=G'+iG'',\qquad\tau=\gamma_0(G'\cos\omega t-G''\sin\omega t).}
$$

The [storage modulus](../../../../../storage-modulus.md) $G'$ measures the elastic component; the [loss modulus](../../../../../loss-modulus.md) $G''$ measures dissipation. The mean power per volume is $\omega\gamma_0^2G''/2$, and the energy dissipated per cycle is $\pi\gamma_0^2G''$, fixing the sign convention.

A Hookean solid has $G^*=G_0$, while a Newtonian fluid has $G^*=i\omega\eta$. The [Maxwell model](../../../../../linear-maxwell-fluid.md) interpolates with $G^*=G_0i\omega\tau_R/(1+i\omega\tau_R)$, giving $G'=G_0(\omega\tau_R)^2/[1+(\omega\tau_R)^2]$ and $G''=G_0\omega\tau_R/[1+(\omega\tau_R)^2]$. It is fluid-like at low frequency and elastic on times short compared with relaxation time $\tau_R$.

A [rheometer](../../../../../rheometer.md) imposes [small-amplitude oscillatory shear](../../../../../small-amplitude-oscillatory-shear.md) and resolves the torque amplitude and phase relative to the imposed motion. The [torsional measurement of a complex shear modulus](../../../../../torsional-measurement-of-a-complex-shear-modulus.md) makes the conversion from torque and twist to $G^*$ explicit. A frequency sweep locates relaxation scales; keeping the strain small tests the linear-response assumption.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [A1](../../a1.md)
3. [Section A](../../../section-a.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter course of the University of Cambridge](../../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
