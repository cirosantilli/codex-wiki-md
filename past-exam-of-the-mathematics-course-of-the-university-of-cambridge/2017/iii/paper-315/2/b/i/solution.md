<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let the closed atmospheric parcel exchange [heat](../../../../../../../heat.md) and volume work with reservoirs at fixed [temperature](../../../../../../../temperature.md) $T$ and [pressure](../../../../../../../pressure.md) $P$, while reactions rearrange its conserved elemental inventory. For a reversible differential between equilibrium states, the [first law of thermodynamics](../../../../../../../first-law-of-thermodynamics.md), with chemical work included, is

$$
dU=T\,dS-P\,dV+\sum_i\mu_i\,dN_i.
$$

The [Gibbs free energy](../../../../../../../gibbs-free-energy.md) $G=U+PV-TS$ therefore obeys

$$
dG=-S\,dT+V\,dP+\sum_i\mu_i\,dN_i.
$$

The [first law of thermodynamics](../../../../../../../first-law-of-thermodynamics.md) supplies this differential but does not alone choose the direction of a reaction. The [Second law of thermodynamics](../../../../../../../second-law-of-thermodynamics.md) does: for the parcel plus its reservoirs, at fixed $T,P$ and with no non-volume work,

$$
dS_{\rm total}=dS-\frac{dU+P\,dV}{T}=-\frac{dG}{T}\ge0.
$$

Thus spontaneous reactions decrease [Gibbs free energy](../../../../../../../gibbs-free-energy.md), and stable [thermochemical equilibrium](../../../../../../../thermochemical-equilibrium.md) is its constrained minimum. For an allowed reaction of extent $d\xi$, let $dN_i=\nu_i\,d\xi$, with positive [stoichiometric vector](../../../../../../../stoichiometric-vector.md) entries for products and negative entries for reactants. At an interior minimum,

$$
\boxed{\left(\frac{\partial G}{\partial\xi}\right)_{T,P}
=\sum_i\nu_i\mu_i=0,\qquad
\delta^2G\ge0\text{ on allowed variations}.}
$$

The condition must hold for every independent allowed reaction, with fixed total atoms of each element and any relevant charge constraint. At a boundary with absent species, only feasible one-sided variations are permitted. These are the hypotheses of [constrained Gibbs minimization for chemical equilibrium](../../../../../../../constrained-gibbs-minimization-for-chemical-equilibrium.md).

For an [ideal gas](../../../../../../../ideal-gas.md) mixture, $\mu_i=\mu_i^\circ(T)+\mathcal RT\log(x_iP/P^\circ)$, where $x_i$ is the [volume mixing ratio](../../../../../../../volume-mixing-ratio.md) and $\mathcal R$ the molar gas constant. Therefore

$$
\prod_i\left(\frac{x_iP}{P^\circ}\right)^{\nu_i}
=\exp\left(-\frac{\Delta_rG^\circ}{\mathcal RT}\right)\equiv K_p(T).
$$

This is a dimensionless activity-based equilibrium constant, not a bare product of dimensional pressures.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 315](../../../../paper-315-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
