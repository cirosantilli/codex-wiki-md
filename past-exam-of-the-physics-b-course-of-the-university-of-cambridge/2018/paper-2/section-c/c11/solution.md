<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

**Equilibrium radiation and cavity [frequencies](../../../../../frequency.md).** A [blackbody](../../../../../blackbody.md) absorbs all incident radiation at every [frequency](../../../../../frequency.md) and direction. In [thermal equilibrium](../../../../../thermal-equilibrium-split.md) its emission spectrum depends only on its [temperature](../../../../../temperature-split.md). Radiation inside an isothermal absorbing cavity, sampled through a small aperture that hardly disturbs equilibrium, realizes [black-body radiation](../../../../../black-body-radiation.md) to a good approximation. Microscopic absorption and emission establish the equilibrium distribution; a perfectly reflecting wall is the convenient idealization used to count the modes once that distribution is specified.

In a [rectangular electromagnetic cavity](../../../../../rectangular-electromagnetic-cavity.md), the [wave equation](../../../../../wave-equation-split.md) and [perfect conductor](../../../../../perfect-conductor.md) wall [boundary conditions](../../../../../boundary-condition.md) select component wavenumbers $k_x=\pi l/L_x$, $k_y=\pi m/L_y$, $k_z=\pi n/L_z$. Combining the [vacuum](../../../../../vacuum.md) [dispersion relation](../../../../../dispersion-relation-split.md) $\omega=c|\mathbf k|$ and $\nu=\omega/(2\pi)$ gives

$$
\boxed{\nu_{lmn}=\frac{c}{2\pi}\sqrt{\left(\frac{\pi l}{L_x}\right)^2+
\left(\frac{\pi m}{L_y}\right)^2+\left(\frac{\pi n}{L_z}\right)^2}.}
$$

For example, electric-field components can have the spatial dependence

$$
\begin{aligned}
E_x&=A_x\cos(k_xx)\sin(k_yy)\sin(k_zz),\\
E_y&=A_y\sin(k_xx)\cos(k_yy)\sin(k_zz),\\
E_z&=A_z\sin(k_xx)\sin(k_yy)\cos(k_zz).
\end{aligned}
$$

For three positive indices, [Gauss's law](../../../../../gauss-s-law.md) requires $k_xA_x+k_yA_y+k_zA_z=0$, leaving two independent [polarizations of an electromagnetic wave](../../../../../polarization-of-an-electromagnetic-wave.md).

**Index qualification.** The original paper describes the indices as positive integers. That describes the three-nonzero-index family but omits valid electromagnetic modes with exactly one zero index, which have one [polarization of an electromagnetic wave](../../../../../polarization-of-an-electromagnetic-wave.md). For instance, with $n=0$, $l,m\geq1$, only $E_z$ above remains; it is normal to the top and bottom faces and vanishes at the side walls. Two zero indices give no nontrivial cavity field. The omitted one-zero-index family does not affect the leading three-dimensional mode count, but is essential to the thin-cavity limit below. Retaining the paper's strict positivity restriction for every mode would instead give a thickness gap and would not yield its requested two-dimensional [power law](../../../../../power-law.md).

**Three-dimensional mode count.** A lattice cell in positive $\mathbf k$ space has [volume](../../../../../volume-thermodynamics.md) $\pi^3/V$, where $V=L_xL_yL_z$. In a continuum approximation, a shell of radius $k$ and thickness $dk$ contains its positive octant, multiplied by two polarizations:

$$
dN=2\frac{V}{\pi^3}\frac18\,4\pi k^2\,dk
=\frac{V}{\pi^2}k^2\,dk.
$$

Using $k=2\pi\nu/c$ gives

$$
\boxed{dN=V\frac{8\pi\nu^2}{c^3}\,d\nu.}
$$

For a finite cavity the exact [density of states](../../../../../density-of-states.md) is discrete; this formula is its bulk continuum limit, appropriate when many modes contribute and wall corrections are small.

**[Mean](../../../../../expected-value-split.md) [photon number](../../../../../photon-number.md).** A mode is a [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator-split.md) with thermal excitation [energies](../../../../../energy-split.md) $s h\nu$, $s=0,1,2,\ldots$. The [zero-point energy](../../../../../zero-point-energy.md) does not enter its thermal occupation. Put $q=e^{-h\nu/(k_BT)}$. Its [partition function](../../../../../canonical-partition-function.md) and [mean](../../../../../expected-value-split.md) occupation are

$$
Z_\nu=\sum_{s=0}^\infty q^s=\frac1{1-q},\qquad
\langle s\rangle=q\frac{\partial\ln Z_\nu}{\partial q}
=\frac{q}{1-q}
=\boxed{\frac{1}{e^{h\nu/(k_BT)}-1}.}
$$

This is the [Bose-Einstein distribution](../../../../../bose-einstein-distribution.md) with zero [photon](../../../../../photon.md) [chemical potential](../../../../../chemical-potential-split.md): equilibrium absorption and emission do not conserve [photon number](../../../../../photon-number.md).

**Thermal [energy](../../../../../energy-split.md).** Multiply the [density of states](../../../../../density-of-states.md) by the [mean](../../../../../expected-value-split.md) excitation [energy](../../../../../energy-split.md) $h\nu\langle s\rangle$ and integrate:

$$
U=V\int_0^\infty\frac{8\pi\nu^2}{c^3}\frac{h\nu}{e^{h\nu/(k_BT)}-1}\,d\nu.
$$

The substitution $x=h\nu/(k_BT)$ isolates all the dependence on cavity dimensions and [temperature](../../../../../temperature-split.md):

$$
U=\frac{8\pi V(k_BT)^4}{h^3c^3}
\int_0^\infty\frac{x^3}{e^x-1}\,dx.
$$

Expanding $1/(e^x-1)=\sum_{r=1}^\infty e^{-rx}$ gives an [integral](../../../../../integral-split.md) $\sum_r6/r^4=6\zeta(4)=\pi^4/15$. Hence

$$
\boxed{U=\frac{8\pi^5k_B^4}{15h^3c^3}VT^4
=\frac{\pi^2k_B^4}{15\hbar^3c^3}L_xL_yL_zT^4.}
$$

This is the thermal [energy](../../../../../energy-split.md) only, excluding the zero-point contribution. The three-dimensional continuum regime requires $k_BT$ large compared with the geometric level spacings in all three directions.

**Spectral sketch.** The spectral [energy density](../../../../../energy-density.md) per unit ordinary [frequency](../../../../../frequency.md) is [Planck's law](../../../../../planck-s-law.md),

$$
u_\nu(T)=\frac{8\pi h\nu^3}{c^3}\frac{1}{e^{h\nu/(k_BT)}-1}.
$$

At small [frequency](../../../../../frequency.md) it rises as $8\pi k_BT\nu^2/c^3$, while at large [frequency](../../../../../frequency.md) it decays exponentially. Raising [temperature](../../../../../temperature-split.md) increases the spectrum at every fixed positive [frequency](../../../../../frequency.md), moves the peak to larger [frequency](../../../../../frequency.md) in proportion to $T$, and increases the integrated [area](../../../../../surface-area.md) in proportion to $T^4$. A plot per unit [wavelength](../../../../../wavelength.md) has a different peak position because the integration variable changes.

<a id="section-c/c11/image-planck-spectral-energy-density-at-three-temperatures-on-common-frequency-and-energy-density-scales"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2-2018-blackbody-spectra.png)

**[Figure 2](#section-c/c11/image-planck-spectral-energy-density-at-three-temperatures-on-common-frequency-and-energy-density-scales). Planck spectral energy density at three temperatures on common frequency and energy-density scales**. Original plots of the frequency spectrum, with temperatures in the ratios 1:1.5:2. The dimensionless horizontal axis is hν/(kBTref), and the vertical scale is common to all curves. The higher-temperature peak moves right and the area grows as T to the fourth power.

**Thin-cavity radiation.** Let $A=L_xL_y$. The relevant low-temperature window is

$$
\frac{\pi\hbar c}{L_x},\ \frac{\pi\hbar c}{L_y}\ll k_BT\ll\frac{\pi\hbar c}{L_z}.
$$

Nonzero thickness indices are then thermally suppressed, while many in-plane modes are populated. The $n=0$ family has one [polarization of an electromagnetic wave](../../../../../polarization-of-an-electromagnetic-wave.md). Its allowed in-plane wavenumbers form a lattice of cell [area](../../../../../surface-area.md) $\pi^2/A$; a quarter of a circular shell therefore contains

$$
dN=\frac{A}{\pi^2}\frac14(2\pi k\,dk)
=\frac{A}{2\pi}k\,dk
=\frac{2\pi A\nu}{c^2}\,d\nu.
$$

Thus the [dimensional crossover of thermal cavity radiation](../../../../../dimensional-crossover-of-thermal-cavity-radiation.md) gives

$$
U_{2D}=\frac{2\pi A(k_BT)^3}{h^2c^2}\int_0^\infty\frac{x^2}{e^x-1}\,dx
=\boxed{\frac{4\pi\zeta(3)k_B^3}{h^2c^2}L_xL_yT^3\ \propto\ L_xL_yT^3.}
$$

The [integral](../../../../../integral-split.md) is $2\zeta(3)$ by the same geometric-series argument. A model with a different number of independent [polarizations of an electromagnetic wave](../../../../../polarization-of-an-electromagnetic-wave.md) changes the prefactor but not the $T^3$ scaling. For a cavity with fixed finite $L_x,L_y$, cooling still further eventually freezes its lowest in-plane mode as well: the strict $T\to0$ thermal [energy](../../../../../energy-split.md) is exponentially suppressed. The requested [area](../../../../../surface-area.md) law is the intermediate quasi-two-dimensional regime, not an arbitrarily low-temperature continuum limit.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
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
