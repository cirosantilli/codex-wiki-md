<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [geometrized units](../../../../../geometrized-units.md) with $\hbar=k_B=1$ initially, and write $f(r)=1-2M/r$, $h(r)=1-Q^2/(Mr)$. The given nonextremality assumption makes $h_H=h(2M)=1-Q^2/(2M^2)>0$. Thus the static [Killing vector field](../../../../../killing-vector-field.md) has a simple zero of its norm at

$$
\boxed{r_H=2M.}
$$

The exterior $r>2M$ is static. For [radial null geodesics](../../../../../radial-null-geodesic.md), $dt/dr=\pm1/f$, independently of $h$. With $v=t+\int dr/f$, the metric is

$$
ds^2=-\frac f h\,dv^2+\frac2h\,dv\,dr+r^2d\Omega^2,
$$

which is regular at $r_H$ since $h_H>0$. The outgoing null equation is $dr/dv=f/2$. Inside the future horizon these rays move to smaller radius, while outside they can escape to infinity. Hence the zero is the [event horizon](../../../../../event-horizon.md). The inner zero of $h$ is not another regular [Killing horizon](../../../../../killing-horizon.md): the Killing norm there diverges rather than vanishes. The strict charge bound matters when making the regular extension.

For the [Euclidean black-hole regularity condition](../../../../../euclidean-black-hole-regularity-condition.md), continue $t=it_E$, consistent with the sign of the given quantum time-translation operator. Set $x=r-2M$. To leading order $f=x/(2M)$ and $h=h_H$, so the radial–time part of the Euclidean metric is

$$
ds_E^2=\frac{x}{2Mh_H}dt_E^2+\frac{2M}{h_Hx}dx^2.
$$

Introduce the radial [proper length](../../../../../proper-length.md) coordinate $\rho$ by $x=h_H\rho^2/(8M)$. Then

$$
ds_E^2=d\rho^2+\frac{\rho^2}{16M^2}dt_E^2
+(2M)^2d\Omega^2+O(\rho^2).
$$

The first two terms are a polar plane with angle $t_E/(4M)$. Smoothness at its origin requires

$$
\boxed{\Delta t_E=8\pi M.}
$$

A different period would make a [conical singularity](../../../../../conical-singularity.md). The time coordinate is normalized to [proper time](../../../../../proper-time.md) at infinity, so no further asymptotic redshift factor is needed. The cancellation of $h_H$ proves the charge independence of the [Euclidean horizon period under a regular radial conformal factor](../../../../../euclidean-horizon-period-under-a-regular-radial-conformal-factor.md); this argument would fail at $h_H=0$.

To justify the thermal interpretation, analytic continuation of the [time-evolution operator](../../../../../time-evolution-operator.md) $U(t)=e^{iHt}$ gives $U(it_E)=e^{-Ht_E}$. Its matrix element is an imaginary-time propagation kernel. Identifying the initial and final configurations and integrating over them takes its [trace](../../../../../matrix-trace.md), giving the [Euclidean path integral](../../../../../euclidean-path-integral.md) $Z=\operatorname{Tr}e^{-\beta H}$. In an energy eigenbasis each state has weight $e^{-\beta E}$, exactly the [Boltzmann factor](../../../../../boltzmann-factor.md) of a [canonical ensemble](../../../../../canonical-ensemble.md). Thus the geometrically required period is the inverse [Hawking temperature](../../../../../hawking-temperature.md). With dimensions restored, an imaginary time period $\Delta t_E$ gives $\beta=\Delta t_E/\hbar=1/(k_BT)$. Consequently

$$
\boxed{T_H=\frac1{8\pi M}\quad\text{in natural units},\qquad
T_H=\frac{\hbar c^3}{8\pi Gk_B\mathcal M}\quad(Q=0).}
$$

Here $\mathcal M$ is mass in ordinary units; for a neutral hole $M=G\mathcal M/c^2$ and the physical imaginary-time period is $8\pi G\mathcal M/c^3$. Bosonic thermal fields are periodic and fermionic fields antiperiodic over that same Euclidean period. The relation to the canonical density operator, not just dimensional reasoning, identifies the temperature.

For an evaporation estimate take a neutral, isolated [Schwarzschild black hole](../../../../../schwarzschild-spacetime.md) and approximate its radiated power with the [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md). Its area is $A=16\pi G^2\mathcal M^2/c^4$, and the photon [Stefan-Boltzmann constant](../../../../../stefan-boltzmann-constant.md) is $\sigma_{SB}=\pi^2k_B^4/(60\hbar^3c^2)$. Substituting the temperature gives

$$
P\simeq A\sigma_{SB}T_H^4
=\frac{\hbar c^6}{15360\pi G^2\mathcal M^2},\qquad
\frac{d\mathcal M}{dt}\simeq-\frac{\hbar c^4}{15360\pi G^2\mathcal M^2}.
$$

The [black-hole evaporation](../../../../../black-hole-evaporation.md) speeds up as the mass decreases. Integrating, rather than dividing the initial rest energy by the initial power, gives

$$
\boxed{t_{\rm evap}\simeq\frac{5120\pi G^2\mathcal M_0^3}{\hbar c^4}
\simeq2.1\times10^{67}\ {\mathrm{years}}\quad
(\mathcal M_0=2\times10^{30}\ {\mathrm{kg}}).}
$$

The corresponding initial [Hawking temperature](../../../../../hawking-temperature.md) is about $6\times10^{-8}\,$K. This is the [Stefan-Boltzmann estimate of Schwarzschild evaporation time](../../../../../stefan-boltzmann-estimate-of-schwarzschild-evaporation-time.md) at the level of accuracy requested. [Greybody factors](../../../../../greybody-factor.md) and other emitted species alter the numerical coefficient, but not the leading cubic scaling of a large isolated hole. The estimate assumes negligible accretion or ambient radiation absorption; a stellar-mass hole in the present cosmic radiation bath is not currently losing mass at that isolated-hole rate. Finally the semiclassical formula does not describe the Planck-scale endpoint: extrapolating it to zero mass is an estimate of the macroscopic lifetime, not a proof of what the final quantum object is.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
