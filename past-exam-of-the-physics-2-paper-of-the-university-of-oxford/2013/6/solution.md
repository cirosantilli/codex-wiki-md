<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The ideal voltage source drives a series $L$–$R$–$C$ branch and a separate resistor $R$ in parallel. At $\omega_0=1/\sqrt{LC}$, the series branch is purely resistive, so its peak current is $I_p=V_0/R$. Its stored energies are

$$
U_L=\frac12LI_p^2\sin^2\omega_0t,\qquad U_C=\frac12LI_p^2\cos^2\omega_0t.
$$

Their sum is constant in sinusoidal steady state, with value $U_{\max}=LV_0^2/(2R^2)$. Each resistor dissipates average power $V_0^2/(2R)$, including the resistor directly across the source. Over one cycle,

$$
W_{\rm diss}=\frac{2\pi}{\omega_0}\frac{V_0^2}{R},\qquad
\boxed{\frac{U_{\max}}{W_{\rm diss}}=\frac{\omega_0L}{4\pi R}=\frac1{4\pi R}\sqrt{\frac LC}.}
$$

Omitting the parallel resistor would double this ratio. The expression concerns the driven steady state, not a switch-on transient.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2013](../../2013-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
