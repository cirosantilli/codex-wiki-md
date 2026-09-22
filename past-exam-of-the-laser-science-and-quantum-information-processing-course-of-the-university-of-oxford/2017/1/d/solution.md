<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The upper-state [density](../../../../density.md) is clamped near threshold once the [laser](../../../../laser-split.md) operates, so excess pumping mainly increases [photon](../../../../photon.md) [density](../../../../density.md) and output [power](../../../../power.md). For approximately pump-independent absorption efficiency, $r=P_p/P_{p,\mathrm{th}}$, and both $P_{\mathrm{out}}$ and $f_{\mathrm{ro}}^2$ should rise approximately linearly with $P_p-P_{p,\mathrm{th}}$.

**The left ordinate is the square of the [frequency](../../../../frequency.md)**, in $\mathrm{kHz}^2$, rather than [frequency](../../../../frequency.md) in kHz. Reading the original triangles gives a threshold near $12$–$13\ \mathrm{mW}$ and a slope about $1.0\ \mathrm{kHz}^2/\mathrm{mW}$. A representative straight-line fit to visually read marker centers gives $P_{p,\mathrm{th}}\simeq12.2\ \mathrm{mW}$ and $A=d f_{\mathrm{ro}}^2/dP_p\simeq1.02\times10^6\ \mathrm{Hz}^2/\mathrm{mW}$. Therefore

$$
A\simeq\frac1{4\pi^2\tau_c\tau_2P_{p,\mathrm{th}}},\qquad
\boxed{\tau_c\simeq\frac1{4\pi^2(0.013)(12.2)(1.02\times10^6)}
\simeq1.6\times10^{-7}\ \mathrm s.}
$$

The displayed precision is limited by graph reading and scatter; a lifetime around $0.15\ \mathrm{\mu s}$ is the meaningful result. The output squares have a compatible threshold and an approximately constant slope above it.

The round-trip time is

$$
t_{\mathrm{rt}}=\frac{2n_rL}{c}=\frac{2(1.46)(7)}c\simeq6.82\times10^{-8}\ \mathrm s.
$$

If mirror transmission is the only appreciable passive loss, [energy](../../../../energy-split.md) decays by $R_1R_2=e^{-t_{\mathrm{rt}}/\tau_c}$ per round trip. For $R_1=1$,

$$
\boxed{R_2=e^{-t_{\mathrm{rt}}/\tau_c}\simeq0.65,}
$$

a [power](../../../../power.md) [reflectance](../../../../reflectance.md) of roughly 65%. The exact exponential is preferable to replacing $1-R_2$ by $t_{\mathrm{rt}}/\tau_c$, since the inferred round-trip loss is not tiny. If distributed fibre loss is appreciable, the lifetime instead fixes the total round-trip retention; without a separate loss measurement, the bare mirror [reflectance](../../../../reflectance.md) is not uniquely determined and is at least this retention factor.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
