<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

For excitation [energy](../../../../../energy-split.md) $\Delta=\hbar\omega$, the [geometric series](../../../../../geometric-series.md) gives the [thermal partition function of a quantum harmonic oscillator](../../../../../thermal-partition-function-of-a-quantum-harmonic-oscillator.md) with its [zero-point energy](../../../../../zero-point-energy.md) subtracted:

$$
Z=\sum_{n=0}^{\infty}e^{-\beta n\Delta}=\frac1{1-e^{-\beta\Delta}},\qquad
U=-\frac{\partial\ln Z}{\partial\beta}
=\boxed{\frac{\hbar\omega}{e^{\beta\hbar\omega}-1}.}
$$

Thus $U\to0$ at low [temperature](../../../../../temperature-split.md) and approaches $k_BT$ at high [temperature](../../../../../temperature-split.md). Restoring the zero-point term multiplies $Z$ by $e^{-\beta\Delta/2}$ and adds $\Delta/2$ to $U$, without changing the thermal occupation [probabilities](../../../../../probability.md).

To count electromagnetic modes, put a large cavity in a periodic box of [volume](../../../../../volume.md) $V$. One transverse polarization has wavevector-state [density](../../../../../density.md) $V/(2\pi)^3$; there are two independent polarizations. In the shell $k\to k+dk$,

$$
dN=2\frac{V}{(2\pi)^3}4\pi k^2dk
=\frac{V}{\pi^2}k^2dk.
$$

With $\omega=ck$, the [electromagnetic mode density in a box](../../../../../electromagnetic-mode-density-in-a-box.md) becomes

$$
\boxed{g(\omega)=\frac{dN}{d\omega}=\frac{V\omega^2}{\pi^2c^3}.}
$$

The continuum expression is the large-cavity leading term; using standing-wave boundary conditions gives the same bulk count. Both [photon](../../../../../photon.md) polarizations must be included. This is [density](../../../../../density.md) per [angular frequency](../../../../../angular-frequency.md), not per ordinary [frequency](../../../../../frequency.md).

Each mode is an oscillator with zero [photon](../../../../../photon.md) [chemical potential](../../../../../chemical-potential-split.md) in [thermal equilibrium](../../../../../thermal-equilibrium-split.md). Multiplying its mean thermal [energy](../../../../../energy-split.md) by the mode [density](../../../../../density.md) per [volume](../../../../../volume.md) gives the [angular-frequency Planck energy density](../../../../../angular-frequency-planck-energy-density.md)

$$
\boxed{u(\omega,T)=\frac{\hbar\omega^3}{\pi^2c^3}\frac1{e^{\hbar\omega/(k_BT)}-1}.}
$$

At small $\hbar\omega/(k_BT)$ it reduces to the Rayleigh–Jeans result $k_BT\omega^2/(\pi^2c^3)$; exponential suppression at high [frequency](../../../../../frequency.md) prevents a divergent thermal [energy](../../../../../energy-split.md). With $x=\hbar\omega/(k_BT)$,

$$
u(T)=\int_0^{\infty}u(\omega,T)d\omega
=\frac{k_B^4T^4}{\pi^2\hbar^3c^3}\int_0^{\infty}\frac{x^3}{e^x-1}dx
=\boxed{\frac{\pi^2k_B^4}{15\hbar^3c^3}T^4.}
$$

The integral is the stipulated $\pi^4/15$. This is a [volume](../../../../../volume.md) [energy](../../../../../energy-split.md) [density](../../../../../density.md), $aT^4$; for isotropic cavity radiation the outward black-surface flux is $cu/4=\sigma_{\rm SB}T^4$, with $\sigma_{\rm SB}=\pi^2k_B^4/(60\hbar^3c^2)$. Distinguishing flux, spectral [density](../../../../../density.md) and total [volume](../../../../../volume.md) [energy](../../../../../energy-split.md) avoids extra factors of $c$, $4$ or $2\pi$.

<a id="section-c/c12/image-oscillator-and-radiation-energy"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1-thermal-radiation.png)

**[Figure 5](#section-c/c12/image-oscillator-and-radiation-energy). Oscillator and radiation energy**. Thermal excitation and dimensionless Planck spectra.

## ↑ Ancestors (14)

1. [C12](../c12.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
