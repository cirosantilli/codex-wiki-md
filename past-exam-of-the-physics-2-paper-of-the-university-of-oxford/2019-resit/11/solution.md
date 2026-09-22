<h1 id="11/solution">Solution</h1>

↑ **Parent:** [11](../11.md)

Use [phasors](../../../phasor.md) with time dependence $e^{i\omega t}$ and [electrical impedance](../../../electrical-impedance.md) $Z=\widetilde V/\widetilde I$. The element laws $V=IR$, $I=C\,dV/dt$ and $V=L\,dI/dt$ give

$$
\boxed{Z_R=R,\qquad Z_C=\frac1{i\omega C}=-\frac{i}{\omega C},\qquad Z_L=i\omega L.}
$$

A [complex number](../../../complex-number.md) records both [amplitude](../../../wave-amplitude.md) and [phase](../../../phase-waves.md), turning the linear [differential equations](../../../differential-equation-split.md) of a sinusoidally driven [electrical circuit](../../../electrical-circuit-split.md) into algebraic equations. A [resistor](../../../resistor.md) has in-phase [voltage](../../../voltage.md) and [electric current](../../../electric-current.md) and dissipates average [power](../../../power.md). For an ideal [capacitor](../../../capacitor.md), the [electric current](../../../electric-current.md) leads the [voltage](../../../voltage.md) by $90^\circ$; for an ideal [inductor](../../../inductor.md), it lags by $90^\circ$. Their imaginary [electrical impedances](../../../electrical-impedance.md) express reversible energy storage and return, with zero net average [power](../../../power.md) over a period. Using $e^{-i\omega t}$ would conjugate the displayed reactive signs without changing predictions.

In the illustrated [Maxwell bridge](../../../maxwell-bridge.md), the left and right vertices are the supply terminals and the upper and lower vertices are detector terminals. Insert a sensitive AC null detector between the latter and drive the former with a sinusoidal source. The upper-left arm is $Z_x=R_x+i\omega L_x$, the upper-right arm is $R_3$, the lower-left arm is $R_2$, and the lower-right arm is the parallel combination

$$
Z_p=\left(\frac1{R_1}+i\omega C\right)^{-1}.
$$

At a null no detector [electric current](../../../electric-current.md) flows, so the two voltage dividers give

$$
\frac{R_3}{Z_x+R_3}=\frac{Z_p}{R_2+Z_p},\qquad
Z_xZ_p=R_2R_3.
$$

Multiplying by the parallel-arm [electrical admittance](../../../electrical-admittance.md) yields

$$
R_x+i\omega L_x=R_2R_3\left(\frac1{R_1}+i\omega C\right).
$$

Equating real and imaginary parts therefore gives

$$
\boxed{R_x=\frac{R_2R_3}{R_1},\qquad L_x=CR_2R_3.}
$$

Two independent adjustments are needed to annul the in-phase and quadrature detector signals. For example, change $R_2$ to set $L_x$ and $R_1$ to set $R_x$, iterating until the detector reads zero. Alternatively, with fixed $R_2,R_3$, independently vary $R_1$ and $C$.

The [Maxwell bridge](../../../maxwell-bridge.md) compares an unknown lossy [inductor](../../../inductor.md) with a stable standard [capacitor](../../../capacitor.md), avoiding the need for an accurately known reference [inductor](../../../inductor.md). The ideal balance equations contain no [frequency](../../../frequency.md), and a null measurement need not rely on absolute detector calibration. In practice choose a suitable [frequency](../../../frequency.md) below the coil's self-resonance, where the series $R_x,L_x$ model and the standard [capacitor](../../../capacitor.md) remain accurate.

If the initial setting is far from balance, the bridge as drawn needs adjustable components and a detector, not merely a more precise readout. Fit resistance boxes or switched ranges for $R_1$ and a ratio arm, and a selectable standard $C$. Choose ranges around

$$
R_2R_3=\frac{L_x}{C},\qquad R_1=\frac{L_x}{CR_x}.
$$

Then approach the null with coarse adjustments followed by finer ones. A large required $R_1$ can be brought into range by increasing $C$ and decreasing $R_2R_3$ proportionally. Start with reduced excitation or reduced detector sensitivity to avoid overload, then increase sensitivity near the null. Changing [frequency](../../../frequency.md) alone cannot repair an impossible component range, since the ideal balance conditions are frequency-independent. Stray [capacitance](../../../capacitance.md) and lead [electrical resistance](../../../electrical-resistance.md) set practical accuracy limits and may require shielding and short connections.

## ↑ Ancestors (11)

1. [11](../11.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
