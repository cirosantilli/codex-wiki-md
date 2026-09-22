<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the three-dimensional [Debye model](../../../../debye-model.md), the [lattice](../../../../lattice.md) has $3N$ [normal modes](../../../../normal-mode.md) for $N$ atoms. Replacing their dispersion by a linear acoustic dispersion up to a cutoff gives the [Debye heat capacity](../../../../debye-heat-capacity.md)

$$
C_m(T)=9Nk_B\left(\frac{T}{\theta_D}\right)^3\int_0^{\theta_D/T}\frac{x^4e^x}{(e^x-1)^2}\,dx.
$$

At low [temperature](../../../../temperature-split.md) the upper limit can be replaced by infinity. Since the integral then equals $4\pi^4/15$,

$$
\boxed{C_m(T)\sim\frac{12\pi^4}{5}Nk_B\left(\frac{T}{\theta_D}\right)^3\quad(T\ll\theta_D).}
$$

At high [temperature](../../../../temperature-split.md) each harmonic mode contributes $k_B$ by the [equipartition theorem](../../../../equipartition-theorem.md), giving the [Dulong-Petit law](../../../../dulong-petit-law.md)

$$
\boxed{C_m(T)\longrightarrow3Nk_B\quad(T\gg\theta_D).}
$$

For one mole replace $Nk_B$ by $R$. The curve starts with zero slope, rises as $T^3$, and levels off toward the classical limit. This is the [lattice](../../../../lattice.md) contribution; a metal's [electronic heat capacity](../../../../electronic-heat-capacity.md) is a separate low-temperature term.

The [Debye wavevector](../../../../debye-wavevector.md) follows by counting three polarizations inside the cutoff sphere:

$$
3\frac{\mathcal V}{(2\pi)^3}\frac{4\pi k_D^3}{3}=3N,\qquad k_D=(6\pi^2n)^{1/3}.
$$

With the supplied [speed of sound](../../../../speed-of-sound.md) treated as the effective Debye speed, $\omega_D=vk_D$ and

$$
\boxed{\theta_D=\frac{\hbar v}{k_B}(6\pi^2n)^{1/3}\simeq\frac{\hbar(3600)}{k_B}(6\pi^2\times5.9\times10^{28})^{1/3}\simeq4.17\times10^2\,\mathrm K.}
$$

Here $k_D\simeq1.52\times10^{10}\,\mathrm{m^{-1}}$. Real crystals have different longitudinal and transverse sound speeds; the one-speed estimate uses the stated value, rather than inferring those unprovided branches.

<a id="1/a/image-debye-lattice-heat-capacity-and-the-squared-magnitude-of-the-drude-conductivity"></a>
![](../../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2016-heat-capacity-and-conductivity.png)

**[Figure 1](#1/a/image-debye-lattice-heat-capacity-and-the-squared-magnitude-of-the-drude-conductivity). Debye lattice heat capacity and the squared magnitude of the Drude conductivity**.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
