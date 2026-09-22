<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $G$ be the remaining gas [mass](../../../../../../mass.md), $S$ the formed stellar [mass](../../../../../../mass.md), and $G_0$ the initial gas [mass](../../../../../../mass.md); initially $S=0$ and the [gas-phase metallicity](../../../../../../gas-phase-metallicity.md) is zero. Take the [stellar yield](../../../../../../stellar-yield.md) $y$ and the [mass-loading factor](../../../../../../mass-loading-factor.md) $\nu$ to be constant, with homogeneous mixing and no [galactic gas inflow](../../../../../../galactic-gas-inflow.md). With the specified zero bulk return, [mass conservation](../../../../../../mass-conservation.md) gives

$$
dG=-(1+\nu)\,dS,\qquad G=G_0-(1+\nu)S.
$$

New metals add $y\,dS$, while [star formation](../../../../../../star-formation.md) and the [galactic outflow](../../../../../../galactic-outflow.md) remove metals at the existing [gas-phase metallicity](../../../../../../gas-phase-metallicity.md) $Z$. Thus

$$
d(GZ)=y\,dS-Z(1+\nu)\,dS,
\qquad G\,dZ=y\,dS=-\frac{y}{1+\nu}\,dG.
$$

The [leaky-box model of galactic chemical evolution](../../../../../../leaky-box-model-of-galactic-chemical-evolution.md) therefore gives

$$
Z=\frac{y}{1+\nu}\ln\frac{G_0}{G}.
$$

For the usual [gas fraction of a galaxy](../../../../../../gas-fraction-of-a-galaxy.md), $\mu=G/(G+S)$, the denominator is the baryonic [mass](../../../../../../mass.md) still in the system, which decreases under the [galactic outflow](../../../../../../galactic-outflow.md). Since $G_0=G+(1+\nu)S$, we have $G_0/G=1+(1+\nu)(1-\mu)/\mu$. **In the remaining-mass convention,**

$$
\boxed{Z(\mu)=\frac{y}{1+\nu}\ln\left[\frac{1+\nu(1-\mu)}{\mu}\right].}
$$

If instead $\mu$ denotes $G/G_0$ relative to the fixed initial reservoir, the same calculation gives $\boxed{Z=y\ln(1/\mu)/(1+\nu)}$. Stating the denominator matters: these two [gas fraction of a galaxy](../../../../../../gas-fraction-of-a-galaxy.md) conventions coincide for the [closed-box model of galactic chemical evolution](../../../../../../closed-box-model-of-galactic-chemical-evolution.md), recovered at $\nu=0$, but differ when gas escapes. Neglecting bulk return while retaining a nonzero [stellar yield](../../../../../../stellar-yield.md) is the intended trace-metal approximation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
