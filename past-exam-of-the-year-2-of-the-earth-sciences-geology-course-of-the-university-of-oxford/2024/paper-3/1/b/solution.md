<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The normal-incidence [acoustic impedance](../../../../../acoustic-impedance.md) is $Z=\rho V_p$, with units $\mathrm{kg\,m^{-2}\,s^{-1}}$. Thus

$$
\boxed{Z_1=1.50\times10^6,\qquad Z_2=2.25\times10^6,\qquad Z_3=5.00\times10^6.}
$$

Define the [pressure-amplitude reflection coefficient](../../../../../pressure-amplitude-reflection-coefficient.md) and [pressure-amplitude transmission coefficient](../../../../../pressure-amplitude-transmission-coefficient.md) for incidence downwards from layer $i$ into layer $j$ by

$$
r_p=\frac{p_r}{p_i}=\frac{Z_j-Z_i}{Z_j+Z_i},\qquad t_p=\frac{p_t}{p_i}=\frac{2Z_j}{Z_j+Z_i}=1+r_p.
$$

Here $p$ denotes compressional normal-stress amplitude; in the [water](../../../../../water.md) it is the acoustic [pressure](../../../../../pressure-split.md). Continuity of normal [traction](../../../../../traction.md) and normal particle [velocity](../../../../../velocity.md) gives these expressions. They describe each interface separately, before any layer [layer reverberation](../../../../../layer-reverberation.md).

| Interface, downward incidence | $r_p$ | $t_p$ | Reflected [energy](../../../../../energy-split.md) fraction $R_E$ | Transmitted [energy](../../../../../energy-split.md) fraction $T_E$ |
| --- | --- | --- | --- | --- |
| Water to sediment | $1/5=0.2000$ | $6/5=1.2000$ | $1/25=0.0400$ | $24/25=0.9600$ |
| Sediment to basement | $11/29=0.37931$ | $40/29=1.37931$ | $121/841=0.14388$ | $720/841=0.85612$ |

For a lossless normal-incidence [plane wave](../../../../../plane-wave.md), intensity is proportional to $p^2/Z$, so

$$
R_E=r_p^2,\qquad T_E=\frac{Z_i}{Z_j}t_p^2=\frac{4Z_iZ_j}{(Z_i+Z_j)^2},\qquad R_E+T_E=1.
$$

A transmitted pressure amplitude exceeding unity is therefore compatible with [conservation of energy](../../../../../conservation-of-energy.md). If instead the coefficient is defined for particle [velocity](../../../../../velocity.md) measured along the same downward coordinate, $r_v=-r_p$ and $t_v=2Z_i/(Z_i+Z_j)=1-r_p$: the two transmitted velocity coefficients are $0.8000$ and $18/29=0.62069$. Upward incidence reverses the sign of $r_p$, interchanges the transmitted pressure and velocity coefficients, and leaves $R_E,T_E$ unchanged. At normal incidence between these ideal [isotropic](../../../../../isotropy.md) layers there is no P-to-S [seismic mode conversion](../../../../../seismic-mode-conversion.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
