<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Consider a species in [thermal equilibrium](../../../../../../thermal-equilibrium.md), with [energy density](../../../../../../energy-density.md) and pressure depending on [temperature](../../../../../../temperature.md) and with vanishing [chemical potential](../../../../../../chemical-potential.md), as in the supplied thermodynamic relation. Put $U=\rho(T)V$. The [first law of thermodynamics](../../../../../../first-law-of-thermodynamics.md) gives

$$
dS=\frac VT\frac{d\rho}{dT}\,dT+\frac{\rho+P}{T}\,dV.
$$

Since $dP/dT=(\rho+P)/T$,

$$
\frac{d}{dT}\left(\frac{\rho+P}{T}\right)
=\frac1T\frac{d\rho}{dT}.
$$

The differential is therefore exact:

$$
dS=d\left[V\frac{\rho+P}{T}\right].
$$

After fixing the irrelevant additive entropy zero, the [entropy density at zero chemical potential](../../../../../../entropy-density-at-zero-chemical-potential.md) is

$$
\boxed{s=\frac{S}{V}=\frac{\rho+P}{T}.}
$$

More precisely the first law leaves an additive constant in $S$; extensivity fixes that constant for the usual entropy-density normalization. A nonzero chemical potential would instead require $Ts=\rho+P-\mu n$, so the stated formula is not a universal identity for a decoupled massive species with conserved particle number.

For a [reversible thermodynamic process](../../../../../../reversible-thermodynamic-process.md) that is an [adiabatic process](../../../../../../adiabatic-process.md) in a [comoving volume](../../../../../../comoving-volume.md), $\dot V=3HV$ and the [cosmological perfect-fluid continuity equation](../../../../../../cosmological-perfect-fluid-continuity-equation.md) gives $\dot\rho=-3H(\rho+P)$. Differentiating the extensive expression explicitly, or using the exact differential above, gives

$$
\dot S=\frac1T\left[V\dot\rho+(\rho+P)\dot V\right]=0,
\qquad \boxed{a^3s=\text{constant}.}
$$

This is [cosmological entropy conservation](../../../../../../cosmological-entropy-conservation.md) for the closed equilibrium gas with no entropy-producing energy injection.

For [radiation in cosmology](../../../../../../radiation-in-cosmology.md), $P=\rho/3$, so $s=4\rho/(3T)$. Comparing $s=c_1g_\star T^3$ and $\rho=c_2g_\star T^4$ yields the **coefficient ratio**

$$
\boxed{c_1=\frac43c_2,\qquad \frac{c_2}{c_1}=\frac34.}
$$

When all relativistic species share the same temperature and count, the familiar normalizations are $c_1=2\pi^2/45$ and $c_2=\pi^2/30$. More generally the energy and entropy effective counts can differ; the common $g_\star$ here uses the assumptions stated in the question.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
