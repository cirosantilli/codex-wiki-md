<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

For distributed [inductance](../../../../../inductance.md) $L$ and [capacitance](../../../../../capacitance.md) $C$, a small segment obeys $V_z=-L I_t$ and $I_z=-C V_t$. Differentiation gives $V_{zz}=LCV_{tt}$ and $I_{zz}=LCI_{tt}$. For a forward wave,

$$
\boxed{v=\frac1{\sqrt{LC}},\qquad Z=\frac{V^+}{I^+}=\sqrt{L/C}.}
$$

A backward [voltage](../../../../../voltage.md) wave has current $I^-=-V^-/Z$. This sign matters at an impedance discontinuity.

The source figure is the stacked-strip [parallel-plate transmission line](../../../../../parallel-plate-transmission-line.md) geometry, despite its use of the word coplanar. [Gauss's law](../../../../../gauss-s-law.md) gives $C=\epsilon_0\epsilon_r a/d$. Opposite surface currents give [magnetic field](../../../../../magnetic-field-split.md) $B=\mu_0I/a$ between the strips by [Ampère's law](../../../../../ampere-s-circuital-law.md); the [magnetic flux](../../../../../magnetic-flux.md) per unit [length](../../../../../length.md) is $Bd$, hence $L=Bd/I=\mu_0d/a$. Therefore

$$
\boxed{v=\frac{c}{\sqrt{2.3}}\simeq1.98\times10^8\,\mathrm{m\,s^{-1}},\quad
Z=\frac da\sqrt{\frac{\mu_0}{2.3\epsilon_0}}
\simeq248.4\frac da\,\Omega.}
$$

No numerical $a/d$ is given; the impedance is appropriately left in terms of that ratio. The line is taken to be nonmagnetic and lossless.

Increasing the gap by $\alpha$ changes $L$ to $\alpha L$ and $C$ to $C/\alpha$, so $Z_2=\alpha Z_1$ while $v$ is unchanged. [voltage](../../../../../voltage.md) and current continuity at the step give

$$
V_i+V_r=V_t,\qquad \frac{V_i-V_r}{Z_1}=\frac{V_t}{Z_2}.
$$

Consequently the [voltage](../../../../../voltage.md) and energy-flux [transmission coefficients](../../../../../transmission-coefficient.md) are

$$
\boxed{t_V=\frac{2\alpha}{1+\alpha},\qquad
\mathcal T=\frac{Z_1}{Z_2}|t_V|^2=\frac{4\alpha}{(1+\alpha)^2},}
\qquad r_V=\frac{\alpha-1}{\alpha+1}.
$$

Here amplitudes are peak [voltage](../../../../../voltage.md) amplitudes, with mean [power](../../../../../power.md) $|V|^2/(2Z)$. The reciprocal gaps have $r_V(1/\alpha)=-r_V(\alpha)$: equal reflected [energy](../../../../../energy-split.md) but opposite [voltage](../../../../../voltage.md) phase. A [voltage](../../../../../voltage.md) [transmission coefficient](../../../../../transmission-coefficient.md) above one does not imply [energy](../../../../../energy-split.md) gain.

For a [finite impedance section of a transmission line](../../../../../finite-impedance-section-of-a-transmission-line.md), put $\ell=l_2-l_1$ and $\delta=\omega\ell/v$. Multiple reflections inside the altered section interfere. Summing their [geometric series](../../../../../geometric-series.md), relative to the first boundary,

$$
t_{\rm whole}=\frac{(1-r_V^2)e^{i\delta}}{1-r_V^2e^{2i\delta}},\qquad
\boxed{\mathcal T_{\rm whole}=\left[1+\frac{(\alpha^2-1)^2}{4\alpha^2}\sin^2\delta\right]^{-1}.}
$$

Transmission is unity at $\delta=n\pi$ and minimal at $\delta=(n+1/2)\pi$, with minima $4\alpha^2/(1+\alpha^2)^2$. Resonances are separated by $\Delta f=v/(2\ell)$; the long-wavelength limit also transmits fully. Matching the far termination removes end echoes, not the two internal reflections.

<a id="section-b/b7/image-original-calculated-power-transmission-through-a-finite-changed-impedance-section-between-matched-lines"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-1-line-resonances.png)

**[Figure 2](#section-b/b7/image-original-calculated-power-transmission-through-a-finite-changed-impedance-section-between-matched-lines). Original calculated power transmission through a finite changed-impedance section between matched lines**.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
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
