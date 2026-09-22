<h1 id="section-b/b6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [transmission line](../../../../../../transmission-line.md) must be treated as a distributed circuit when its propagation time is significant on the [signal](../../../../../../signal.md) timescale. Let $R',L',G',C'$ denote resistance, [inductance](../../../../../../inductance.md), leakage conductance and [capacitance](../../../../../../capacitance.md) per unit length. Applying [Kirchhoff's voltage law](../../../../../../kirchhoff-cycle-law.md) and [Kirchhoff's current law](../../../../../../kirchhoff-node-law.md) to a short length $dx$ gives the [telegrapher's equations](../../../../../../telegrapher-s-equations.md)

$$
\frac{\partial V}{\partial x}=-R'I-L'\frac{\partial I}{\partial t},\qquad
\frac{\partial I}{\partial x}=-G'V-C'\frac{\partial V}{\partial t}.
$$

For a lossless line, $R'=G'=0$. Differentiating again gives [wave equations](../../../../../../wave-equation-split.md) with

$$
\boxed{v=\frac1{\sqrt{L'C'}},\qquad Z_0=\sqrt{\frac{L'}{C'}}.}
$$

The travelling solutions can be written $V=V_+(t-x/v)+V_-(t+x/v)$ and $I=[V_+(t-x/v)-V_-(t+x/v)]/Z_0$. The minus sign for the backward wave is essential to [power](../../../../../../power.md) transport.

At a load $Z_L$, continuity of voltage and current gives the voltage [reflection coefficient](../../../../../../reflection-coefficient.md)

$$
\boxed{\Gamma_L=\frac{Z_L-Z_0}{Z_L+Z_0}.}
$$

A matched termination $Z_L=Z_0$ absorbs the incident [signal](../../../../../../signal.md) without reflection. An open circuit has $\Gamma_L=+1$ and a short circuit has $\Gamma_L=-1$. Superposed incident and reflected waves produce [standing waves](../../../../../../standing-wave.md). A sinusoidal lossless line of length $\ell$ transforms the termination into

$$
Z_{\mathrm{in}}=Z_0\frac{Z_L+iZ_0\tan(k\ell)}{Z_0+iZ_L\tan(k\ell)}
$$

for the $e^{i\omega t}$ convention. At a quarter [wavelength](../../../../../../wavelength.md), $Z_{\mathrm{in}}=Z_0^2/Z_L$, allowing impedance transformation. A coaxial line supports a transverse electromagnetic mode whose ideal $L',C'$ are calculated in A4. Its [energy](../../../../../../energy-split.md) travels in the fields between conductors; the [characteristic impedance](../../../../../../characteristic-impedance.md) is not the wire's DC resistance. Losses introduce attenuation and make the [characteristic impedance](../../../../../../characteristic-impedance.md) and propagation constant complex.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
