<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

For sinusoidal steady state with the $e^{i\omega t}$ convention, [complex impedance](../../../../../electrical-impedance.md) is the phasor ratio $Z=\widetilde V/\widetilde I$, encoding both amplitude ratio and phase. From $V=L\,dI/dt$, an ideal inductor has $Z_L=i\omega L$; from $I=C\,dV/dt$, a capacitor has $Z_C=(i\omega C)^{-1}$.

The original diagram has $R_1,L_1$ in series, and $R_4,C_4$ in parallel. Thus

$$
Z_1=R_1+i\omega L_1,\qquad Z_4=\frac{R_4}{1+i\omega R_4C_4}.
$$

With the right supply node as the reference, the two unloaded [voltage divider](../../../../../voltage-divider.md) outputs are $\widetilde V_A=V_0R_2/(Z_1+R_2)$ and $\widetilde V_B=V_0Z_4/(R_3+Z_4)$. Subtracting gives

$$
\boxed{V_{AB}=V_0\left[\frac{R_2}{Z_1+R_2}-\frac{Z_4}{R_3+Z_4}\right].}
$$

The [series-RL parallel-RC bridge balance](../../../../../series-rl-parallel-rc-bridge-balance.md) is $Z_1Z_4=R_2R_3$. Equating its real and imaginary coefficients gives

$$
\boxed{R_1=\frac{R_2R_3}{R_4}=25\,\Omega,\qquad
L_1=R_2R_3C_4=0.250\,\mathrm H.}
$$

These ideal components balance the bridge at any frequency, not just the test frequency.

At $\omega=200\,\mathrm{rad\,s^{-1}}$, the current amplitude through $R_2$ is $5/|50+50i|=0.0707\,\mathrm A$. Using peak rather than RMS supply amplitude,

$$
\boxed{\overline P_{R_2}=\frac12|\widetilde I|^2R_2=0.0625\,\mathrm W.}
$$

In the DC steady state the inductor is a short and the capacitor is open. Both dividers have equal resistors, so each midpoint is at2.5V and the bridge stays balanced. The upper-branch current is0.100A, giving $\boxed{P_{R_2,\rm DC}=0.250\,\mathrm W}$.

For the high-input-resistance voltmeter, hold the other components fixed. At the DC balance,

$$
\frac{dV_{AB}}{dR_1}=-\frac{V_0R_2}{(R_1+R_2)^2}=-0.0500\,\mathrm{V\,\Omega^{-1}},\qquad
\boxed{\delta R_1\simeq\frac{0.001}{0.0500}=0.020\,\Omega.}
$$

The [DC bridge resistance resolution](../../../../../dc-bridge-resistance-resolution.md) is a local readout resolution, or0.08% of $R_1$, not a total uncertainty allowing for supply, component calibration or voltmeter loading. [§15.2, resistor/inductor/capacitor phasors and peak/RMS distinction](../../../../../university-physics-volume-2-by-samuel-j-ling-and-others.md)

## ↑ Ancestors (13)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
