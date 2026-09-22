<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

**[Temperature](../../../../../temperature-split.md) as an equilibrium relation.** Classical thermodynamics begins with the [zeroth law of thermodynamics](../../../../../zeroth-law-of-thermodynamics.md): [thermal equilibrium](../../../../../thermal-equilibrium-split.md) is transitive. A [thermometer](../../../../../thermometer.md) can therefore assign a common empirical [temperature](../../../../../temperature-split.md) to systems in mutual [thermal equilibrium](../../../../../thermal-equilibrium-split.md). Different [thermometer](../../../../../thermometer.md) properties initially give different monotone empirical scales; a resistance reading by itself does not define the absolute scale.

The [Second law of thermodynamics](../../../../../second-law-of-thermodynamics-split.md) provides a substance-independent thermodynamic scale. A reversible engine operating between reservoirs has a [heat](../../../../../heat-split.md) ratio depending only on their [temperatures](../../../../../temperature-split.md). One chooses absolute [temperature](../../../../../temperature-split.md) so that $Q_h/Q_c=T_h/T_c$, with $Q_h,Q_c$ the positive [heat](../../../../../heat-split.md) magnitudes. Its reversible efficiency is $1-T_c/T_h$. Equivalently, reversible [heat](../../../../../heat-split.md) defines [entropy](../../../../../entropy-split.md) through $dS=\delta Q_{\mathrm{rev}}/T$. For an equilibrium simple compressible system,

$$
dU=T\,dS-p\,dV+\mu\,dN,
\qquad
\boxed{\frac1T=\left(\frac{\partial S}{\partial U}\right)_{V,N}.}
$$

Classical thermodynamics uses this relation without needing a microscopic account of [entropy](../../../../../entropy-split.md). A dilute-gas [thermometer](../../../../../thermometer.md) realizes an empirical scale approaching the thermodynamic scale after corrections for nonideal behavior.

**Statistical meaning of the same [derivative](../../../../../derivative.md).** In the microcanonical description, an equilibrium [energy](../../../../../energy-split.md) shell containing $\Omega(U,V,N)$ accessible states has $S=k_B\ln\Omega$. Its statistical [temperature](../../../../../temperature-split.md) is consequently

$$
\boxed{\frac1T=k_B\left(\frac{\partial\ln\Omega}{\partial U}\right)_{V,N}.}
$$

To see why this is an equilibrium [temperature](../../../../../temperature-split.md), let two weakly coupled systems exchange a small [energy](../../../../../energy-split.md) while their total [energy](../../../../../energy-split.md) stays fixed. The combined multiplicity is $\Omega_A(U_A)\Omega_B(U_{\mathrm{tot}}-U_A)$. Maximizing its [logarithm](../../../../../logarithm.md) gives

$$
\frac{\partial\ln\Omega_A}{\partial U_A}
=\frac{\partial\ln\Omega_B}{\partial U_B},
$$

which is equality of the two inverse [temperatures](../../../../../temperature-split.md). Stability requires the total [entropy](../../../../../entropy-split.md) maximum, not only stationarity. The overwhelmingly dominant [macrostate](../../../../../macrostate.md) in a large system therefore realizes the [thermodynamic equilibrium](../../../../../thermodynamic-equilibrium.md) condition.

A large reservoir gives a small subsystem the canonical [probabilities](../../../../../probability.md) $p_i\propto e^{-\beta E_i}$, with $\beta=1/(k_BT)$. In that ensemble, $F=-k_BT\ln Z$ and $S=-k_B\sum_i p_i\ln p_i$ agree with macroscopic thermodynamic relations in their usual equilibrium regime. The equipartition identity for a classical dilute monatomic gas, $\langle p^2/(2m)\rangle=3k_BT/2$, is a useful operational connection between microscopic motion and [temperature](../../../../../temperature-split.md), but is not a universal definition: quantum modes need not obey equipartition, and a system away from equilibrium need not have one [temperature](../../../../../temperature-split.md) at all.

For finite systems one must specify the [entropy](../../../../../entropy-split.md) convention and [energy](../../../../../energy-split.md) resolution; surface and fluctuation corrections can distinguish definitions that agree in the ordinary [thermodynamic limit](../../../../../thermodynamic-limit.md). Bounded-energy population-inverted systems can also have a negative [entropy](../../../../../entropy-split.md) [derivative](../../../../../derivative.md) and hence a negative statistical [temperature](../../../../../temperature-split.md). That possibility lies outside an ordinary positive-temperature ideal-gas [thermometer](../../../../../thermometer.md); it does not [mean](../../../../../expected-value-split.md) [temperature](../../../../../temperature-split.md) is merely an arbitrary average [kinetic energy](../../../../../kinetic-energy.md).

**Obtaining the [energy](../../../../../energy-split.md)–[temperature](../../../../../temperature-split.md) conversion.** The [Boltzmann constant](../../../../../boltzmann-constant.md) connects [entropy](../../../../../entropy-split.md) measured in $\mathrm{J\,K^{-1}}$ with the dimensionless [logarithm](../../../../../logarithm.md) of a state count. Historically it could be determined from the [ideal gas law](../../../../../ideal-gas-law.md) $pV=Nk_BT$: measure the [molar gas constant](../../../../../molar-gas-constant.md) $R$ and independently determine the [Avogadro constant](../../../../../avogadro-constant.md) $N_A$, then obtain $k_B=R/N_A$. The independent particle-number determination matters; using $R$ alone would not fix [energy](../../../../../energy-split.md) per particle.

An electrical method uses [Johnson-Nyquist noise](../../../../../thermal-electrical-noise.md). A resistor of resistance $R_e$ at known [temperature](../../../../../temperature-split.md) has, in the classical range $hf\ll k_BT$, a one-sided open-circuit voltage-noise spectrum $S_V(f)=4k_BTR_e$. Over a calibrated flat bandwidth $\Delta f$,

$$
\boxed{k_B=\frac{\langle v^2\rangle}{4TR_e\Delta f}.}
$$

A practical measurement uses an equilibrium resistor, a calibrated low-noise amplifier and a known [transfer function](../../../../../transfer-function.md), subtracts or independently characterizes amplifier [noise](../../../../../noise-signal-processing.md), and replaces a nominal bandwidth by the actual [effective noise bandwidth](../../../../../effective-noise-bandwidth.md). Varying [temperature](../../../../../temperature-split.md) and fitting the mean-square voltage is more informative than treating one amplified voltage sample as the thermal [variance](../../../../../variance-split.md). Other primary methods relate [temperature](../../../../../temperature-split.md) to sound speed in a dilute gas or to calibrated particle [diffusion](../../../../../diffusion.md) and [mobility](../../../../../order-parameter-mobility.md).

There is a historically relevant unit-definition qualification: by the date of this exam, the revised SI had already taken effect on 20 May 2019. The [kelvin](../../../../../kelvin.md) is now defined by fixing

$$
\boxed{k_B=1.380649\times10^{-23}\,\mathrm{J\,K^{-1}}\quad\text{exactly}.}
$$

The same experiments now realize or compare thermodynamic [temperatures](../../../../../temperature-split.md) using this fixed constant, whereas historically they measured the conversion constant on an independently defined [temperature](../../../../../temperature-split.md) scale. The physical distinction between equilibrium [temperature](../../../../../temperature-split.md) and microscopic state counting is unchanged.[BIPM, SI definitions effective from 20 May 2019 and fixed [Boltzmann constant](../../../../../boltzmann-constant.md)](https://www.bipm.org/en/measurement-units/)

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
