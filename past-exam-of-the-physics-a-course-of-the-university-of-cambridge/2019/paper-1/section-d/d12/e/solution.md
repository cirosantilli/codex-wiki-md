<h1 id="section-d/d12/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A non-ideal amplifier is not specified by infinite [input impedance](../../../../../../input-impedance.md) alone: its [open-loop gain](../../../../../../open-loop-gain.md) and [output impedance](../../../../../../output-impedance.md) must also be modeled. Take its internal controlled output to be $u=-A(s)v$, where $v$ is the inverting-input potential, and place a resistance $r_o$ between $u$ and the actual output $y=V_{\mathrm{out}}$. The non-inverting input remains grounded; assume no external load. This gives an explicit [finite-gain operational-amplifier integrator](../../../../../../finite-gain-operational-amplifier-integrator.md) model.

<a id="section-d/d12/e/image-non-ideal-integrator-model-and-its-gain-and-phase-for-a-specified-dominant-pole-amplifier"></a>
![](../../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1-nonideal-integrator.png)

**[Figure 4](#section-d/d12/e/image-non-ideal-integrator-model-and-its-gain-and-phase-for-a-specified-dominant-pole-amplifier). Non-ideal integrator model and its gain and phase for a specified dominant-pole amplifier**.

Writing [Kirchhoff's current law](../../../../../../kirchhoff-node-law.md) at the input and output nodes gives

$$
\frac{V_{\mathrm{in}}-v}{R}=sC(v-y),\qquad \frac{u-y}{r_o}=sC(y-v),\qquad u=-A(s)v.
$$

The second equation gives $y=(sCr_o-A)v/(1+sCr_o)$. Substitution in the first gives the general [transfer function](../../../../../../transfer-function.md)

$$
\boxed{H(s)=\frac{V_{\mathrm{out}}}{V_{\mathrm{in}}}=\frac{sCr_o-A(s)}{1+sC\{r_o+R[1+A(s)]\}}.}
$$

For sinusoidal [phasors](../../../../../../phasor.md), set $s=i\omega$. The numerator and denominator are complex, so the magnitude gives the [amplitude](../../../../../../wave-amplitude.md) ratio and their arguments give the relative phase.

The simplest model takes $r_o=0$ and a constant finite gain $A_0>0$. It gives

$$
H(i\omega)=-\frac{A_0}{1+i\omega RC(1+A_0)},\qquad |H|=\frac{A_0}{\sqrt{1+\omega^2R^2C^2(1+A_0)^2}},\qquad \arg H=\pi-\tan^{-1}[\omega RC(1+A_0)].
$$

Thus below $\omega_l=[(1+A_0)RC]^{-1}$ the amplifier has gain magnitude $A_0$ and inversion. Above that [frequency](../../../../../../frequency.md) it approaches an integrator with magnitude $A_0/[(1+A_0)\omega RC]\simeq1/(\omega RC)$ and phase $+90^\circ$. Constant finite gain by itself predicts no further high-frequency turnover.

For a more realistic sketch, use the standard dominant-pole [open-loop gain](../../../../../../open-loop-gain.md) $A(s)=A_0/(1+s/\omega_a)$, still with $r_o=0$. Then

$$
\boxed{H(s)=\frac{-A_0}{1+bs+cs^2},\quad b=\omega_a^{-1}+(1+A_0)RC,\quad c=RC/\omega_a.}
$$

The exact [frequency](../../../../../../frequency.md) response is

$$
|H(i\omega)|=\frac{A_0}{\sqrt{(1-c\omega^2)^2+b^2\omega^2}},\qquad \phi(\omega)=\pi-\operatorname{atan2}(b\omega,1-c\omega^2).
$$

Assuming $A_0\gg1$ and $A_0\omega_aRC\gg1$, the turnover frequencies are well separated: $\omega_l\simeq1/(A_0RC)$ and $\omega_h\simeq A_0\omega_a$, the approximate unity-gain angular [frequency](../../../../../../frequency.md) of the amplifier. The regimes are

$$
\boxed{\begin{array}{c|c|c}
\text{frequency}&|H|&\text{phase}\\ \hline
\omega\ll\omega_l&A_0&180^\circ\\
\omega_l\ll\omega\ll\omega_h&(\omega RC)^{-1}&90^\circ\\
\omega\gg\omega_h&A_0\omega_a/(\omega^2RC)&0^\circ
\end{array}}
$$

with magnitude slopes $0,-20,-40\,\mathrm{dB}$ per decade and smooth phase transitions. This is the solid curve in the figure; $180^\circ$ and $-180^\circ$ denote the same phase.

If finite $r_o$ is retained and $A(i\omega)\to0$, the general expression instead approaches $r_o/(R+r_o)$ at very high [frequency](../../../../../../frequency.md): the [capacitor](../../../../../../capacitor.md) couples the input to the output through a passive [voltage](../../../../../../voltage.md) divider. The dashed curve illustrates that eventual feedthrough. Other amplifier poles or an external load would alter the response again. No particular values of $A_0,\omega_a,r_o$ are given in the paper, so the numerical sketch is illustrative and the general expression states the model dependence explicitly.

## ↑ Ancestors (15)

1. [E](../e.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
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
