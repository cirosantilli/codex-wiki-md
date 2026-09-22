<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\psi(t)$ be the [star formation rate](../../../../../../star-formation-rate.md), $M$ the remaining gas mass, and $S$ the mass put into stars. With zero returned bulk gas, pristine [galactic gas inflow](../../../../../../galactic-gas-inflow.md), and no [galactic outflow](../../../../../../galactic-outflow.md), [mass conservation](../../../../../../mass-conservation.md) gives

$$
\dot S=\psi,\qquad \dot M=-(1-\nu)\psi.
$$

A well-mixed gas reservoir loses existing metals at rate $Z\psi$ and gains newly synthesized metals at rate $y\psi$; the incoming gas brings none. Thus

$$
\frac{d(MZ)}{dt}=y\psi-Z\psi,\qquad
M\dot Z=(y-\nu Z)\psi.
$$

For $0<\nu<1$, eliminate time and integrate:

$$
\frac{dZ}{y-\nu Z}=-\frac{dM}{(1-\nu)M},\qquad
\frac{y-\nu Z}{y-\nu Z_0}=\left(\frac M{M_0}\right)^{\nu/(1-\nu)}.
$$

The [proportional-infall model of galactic chemical evolution](../../../../../../proportional-infall-model-of-galactic-chemical-evolution.md) therefore gives, for initially pristine gas,

$$
\boxed{Z=\frac y\nu\left[1-\left(\frac M{M_0}\right)^{\nu/(1-\nu)}\right]}.
$$

**The displayed form requires $Z_0=0$**; more generally $Z=y/\nu+(Z_0-y/\nu)(M/M_0)^{\nu/(1-\nu)}$. Also $S=(M_0-M)/(1-\nu)$ for an initially star-free reservoir, so $M/M_0$ is not the [gas fraction of a galaxy](../../../../../../gas-fraction-of-a-galaxy.md) $M/(M+S)$. As a check, the $\nu\to0$ limit is the [closed-box model of galactic chemical evolution](../../../../../../closed-box-model-of-galactic-chemical-evolution.md) relation $Z=y\log(M_0/M)$; at $\nu=1$ the gas mass is constant and one must instead solve $\dot Z=(y-Z)\psi/M_0$. Retaining a nonzero [stellar yield](../../../../../../stellar-yield.md) while setting bulk mass return to zero is the prescribed trace-metal approximation, not a literal claim that stellar ejecta have no mass.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
