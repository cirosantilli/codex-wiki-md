<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Johnson-Nyquist noise](../../../../../../thermal-electrical-noise.md) is equilibrium electrical fluctuation caused by thermal agitation of charge carriers. A [resistor](../../../../../../resistor.md) can generate a fluctuating terminal [voltage](../../../../../../voltage.md) even when its mean current is zero. In the classical [frequency](../../../../../../frequency.md) range $hf\ll k_BT$, the [fluctuation-dissipation theorem](../../../../../../fluctuation-dissipation-theorem.md) relates this [noise](../../../../../../noise-signal-processing.md) to dissipative resistance. The one-sided [voltage](../../../../../../voltage.md) [power spectral density](../../../../../../power-spectral-density.md) of an unloaded [resistor](../../../../../../resistor.md) is

$$
\boxed{S_V^{(1)}(f)=4k_BTR\quad\mathrm{V^2/Hz}.}
$$

Equivalently its short-circuit current spectrum is $4k_BT/R$. Over a flat bandwidth $B$ the rms [voltage](../../../../../../voltage.md) is $\sqrt{4k_BTRB}$. A real measurement instead integrates $S_V(f)|H(f)|^2$ over positive [frequency](../../../../../../frequency.md), with loading and the filter's [effective noise bandwidth](../../../../../../effective-noise-bandwidth.md) included. A flat spectrum does not imply an infinite physically measurable [variance](../../../../../../variance-split.md); the circuit and the quantum high-frequency regime limit the ideal white-noise model.

Cooling or narrowing the accepted bandwidth reduces [thermal noise](../../../../../../thermal-noise.md). Reducing resistance lowers its open-circuit [voltage](../../../../../../voltage.md) [noise](../../../../../../noise-signal-processing.md) but raises its short-circuit current [noise](../../../../../../noise-signal-processing.md), so the appropriate choice depends on source impedance and amplifier loading. Thermal agitation is not a fluctuating externally applied [voltage](../../../../../../voltage.md) that can be removed by perfect shielding alone.

[Shot noise](../../../../../../shot-noise.md) arises from discrete transfer events. In the simplest [shot noise counting model](../../../../../../shot-noise-counting-model.md), equal charges $q$ arrive independently at constant rate $r$. A gate of duration $t$ contains a Poisson number $K$, with mean and [variance](../../../../../../variance-split.md) $rt$. Therefore mean current is $I=qr$, and the averaged-current [variance](../../../../../../variance-split.md) is $qI/t$. The corresponding one-sided low-frequency spectrum is

$$
\boxed{S_I^{(1)}(f)=2qI,\qquad I_{\mathrm{rms,noise}}=\sqrt{2qIB}}
$$

for a flat accepted bandwidth. [Electron](../../../../../../electron.md) current has $q=e$. Vacuum emission or photodetection can approximate independent arrivals; correlations in a conductor can suppress or enhance the fluctuations. Discreteness by itself does not guarantee Poisson statistics.

For a fixed mean current the ideal shot-noise formula is not proportional to [temperature](../../../../../../temperature-split.md), whereas Johnson [noise](../../../../../../noise-signal-processing.md) is. Increasing current raises absolute [shot noise](../../../../../../shot-noise.md) but lowers its fractional size, since $\sqrt{2qIB}/I\propto I^{-1/2}$. Both can appear approximately white within a useful [frequency](../../../../../../frequency.md) band, and independent [noise](../../../../../../noise-signal-processing.md) powers add after referring them to a common measurement point. Their spectra must use the same convention: two-sided densities are half these one-sided values. A real low-current experiment can also contain amplifier [noise](../../../../../../noise-signal-processing.md), low-frequency drift and correlated transfer [noise](../../../../../../noise-signal-processing.md), so a mean current or resistance alone does not specify its complete [noise](../../../../../../noise-signal-processing.md) budget.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
