<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take incidence from A into B and first specify **[pressure](../../../../pressure-split.md) amplitude**. For a plane [acoustic wave](../../../../acoustic-wave.md) traveling normally to the interface, the [acoustic impedance](../../../../acoustic-impedance.md) is $Z=\rho c_s$. A right-moving wave has [pressure](../../../../pressure-split.md) amplitude $P=ZU$, where $U$ is its fluid-velocity amplitude; a left-moving reflected wave has $P=-ZU$.

Let $P_i,P_r,P_t$ denote incident, reflected, and transmitted [pressure](../../../../pressure-split.md) amplitudes. Continuity of [pressure](../../../../pressure-split.md) and normal [velocity](../../../../velocity.md) at the interface gives

$$
P_i+P_r=P_t,\qquad \frac{P_i-P_r}{Z_A}=\frac{P_t}{Z_B}.
$$

Solving the two linear equations gives the [acoustic reflection and transmission at an interface](../../../../acoustic-reflection-and-transmission-at-an-interface.md) coefficients

$$
\frac{P_t}{P_i}=\frac{2Z_B}{Z_A+Z_B},\qquad
\frac{P_r}{P_i}=\frac{Z_B-Z_A}{Z_A+Z_B}.
$$

For the same perfect gas, take a common [adiabatic index](../../../../heat-capacity-ratio.md) $\gamma$. The [adiabatic sound speed](../../../../adiabatic-sound-speed.md) satisfies $c_s^2=\gamma p/\rho$. The equal equilibrium [pressure](../../../../pressure-split.md) therefore implies $Z_B/Z_A=\sqrt{\rho_B/\rho_A}=\sqrt\delta$, giving

$$
\boxed{\frac{P_t}{P_i}=\frac{2\sqrt\delta}{1+\sqrt\delta}.}
$$

The word amplitude is otherwise ambiguous. For fluid [velocity](../../../../velocity.md), or [displacement](../../../../displacement.md) at the same frequency, the corresponding answer is

$$
\boxed{\frac{U_t}{U_i}=\frac{\xi_t}{\xi_i}=\frac{2}{1+\sqrt\delta}.}
$$

These are consistent because [pressure](../../../../pressure-split.md) and [velocity](../../../../velocity.md) amplitudes differ by the impedance. As an energy check, the time-averaged [acoustic intensity](../../../../acoustic-energy-flux.md) is $|P|^2/(2Z)$, so its transmission coefficient is $\mathcal T=4\sqrt\delta/(1+\sqrt\delta)^2\leq1$, even when the transmitted [pressure](../../../../pressure-split.md) amplitude exceeds the incident one.

Equal [mean molecular weight](../../../../mean-molecular-weight.md) alone does not logically guarantee equal $\gamma$. If the gases have different values of the [adiabatic index](../../../../heat-capacity-ratio.md), replace $\sqrt\delta$ in these formulas by $\sqrt{\gamma_B\delta/\gamma_A}$; a density-only answer requires the common-$\gamma$ assumption.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
