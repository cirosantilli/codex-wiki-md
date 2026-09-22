<h1 id="section-a/a1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [fluctuation-dissipation theorem](../../../../../fluctuation-dissipation-theorem.md) relates spontaneous fluctuations in [thermal equilibrium](../../../../../thermal-equilibrium-split.md) to the dissipative part of the [linear response](../../../../../linear-response-theory.md) to a weak conjugate force. For an overdamped trapped coordinate, the [Langevin equation](../../../../../langevin-dynamics.md) is

$$
\gamma\dot x+Kx=f(t)+\xi(t),\qquad \langle\xi(t)\xi(t')\rangle=2\gamma k_BT\delta(t-t').
$$

The [fluctuation-dissipation relation for a Langevin particle](../../../../../fluctuation-dissipation-relation-for-a-langevin-particle.md) fixes the noise strength from the same drag coefficient $\gamma$ that dissipates motion. With a drive proportional to $e^{-i\omega t}$, the [linear response](../../../../../linear-response-theory.md) function is $\chi(\omega)=1/(K-i\gamma\omega)$. The two-sided angular-frequency [power spectral density](../../../../../power-spectral-density.md) then obeys

$$
\boxed{S_{xx}(\omega)=\frac{2\gamma k_BT}{K^2+\gamma^2\omega^2}=\frac{2k_BT}{\omega}\operatorname{Im}\chi(\omega).}
$$

Its integral $\int S_{xx}\,d\omega/(2\pi)=k_BT/K$ agrees with the [equipartition theorem](../../../../../equipartition-theorem.md). Without a restoring force, the same noise-drag relation gives the diffusion-mobility relation $D=k_BT/\gamma$.

In [thermal calibration of an optical trap](../../../../../thermal-calibration-of-an-optical-trap.md), record a bead's spontaneous displacement fluctuations and compare their spectrum with its response to a weak calibrated oscillatory force. The [overdamped harmonic-trap power spectrum](../../../../../overdamped-harmonic-trap-power-spectrum.md) and the dissipative response must be consistent with the same temperature and drag. The equilibrium and weak-drive conditions are essential: an actively driven bath need not obey this equilibrium relation.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [A1](../../a1.md)
3. [Section A](../../../section-a.md)
4. [2006](../../../../2006-split.md)
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
