<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

In series the same current passes through both [resistors](../../../../../resistor.md), while their [voltage](../../../../../voltage.md) drops add: $V=I(R_1+R_2)$. In parallel the same [voltage](../../../../../voltage.md) drives currents $V/R_1$ and $V/R_2$, which add. Thus $R_s=R_1+R_2$ and $R_p^{-1}=R_1^{-1}+R_2^{-1}$.

Use [phasors](../../../../../phasor.md) proportional to $e^{i\omega t}$. Then $Z_L=i\omega L$ and $Z_C=1/(i\omega C)$. The printed diagram places C in parallel with the series RL branch, so the input admittance is

$$
Y=\frac1Z=i\omega C+\frac1{R+i\omega L},\qquad
\operatorname{Re}Y=\frac{R}{R^2+\omega^2L^2},\quad
\operatorname{Im}Y=\omega\left(C-\frac{L}{R^2+\omega^2L^2}\right).
$$

Its nonzero zero-phase [frequency](../../../../../frequency.md) exists for $R^2<L/C$:

$$
\boxed{\omega_1=\sqrt{\frac1{LC}-\frac{R^2}{L^2}}.}
$$

At zero [frequency](../../../../../frequency.md), $|Y|=1/R$ and $I_0=V_0/R$. At $\omega_1$, $R^2+\omega_1^2L^2=L/C$, giving

$$
\boxed{|Y(\omega_1)|=\frac{RC}{L},\qquad I_0(\omega_1)=\frac{V_0RC}{L}.}
$$

For $0<\omega<\omega_1$, $\operatorname{Im}Y<0$, so current lags [voltage](../../../../../voltage.md). At very high [frequency](../../../../../frequency.md), $Y\sim i\omega C$, so current leads by $\pi/2$. Zero [phase](../../../../../phase-waves.md) need not coincide exactly with the minimum current magnitude in this lossy network.

The three measured limits determine the components in order:

$$
R=\frac{V_0}{I_{\rm DC}}=100\,\Omega,\qquad
C=\frac{\alpha}{V_0}=2.50\times10^{-7}\,\mathrm F,\qquad
L=\frac{V_0RC}{I_0(\omega_1)}=0.100\,\mathrm H,
$$



$$
\boxed{\omega_1=6.245\times10^3\,\mathrm{rad\,s^{-1}}.}
$$

For the changed resistance, the quoted $0.6\,\mathrm{kHz}$ is an ordinary [frequency](../../../../../frequency.md), so $\omega'=2\pi(600\,\mathrm{s^{-1}})$. Keeping L and C fixed gives

$$
\boxed{R'=\sqrt{\frac LC-\omega'^2L^2}=5.08\times10^2\,\Omega.}
$$

## ↑ Ancestors (13)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
