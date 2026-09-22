<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume a single-phase [ideal gas](../../../../../../../ideal-gas.md) mixture in a closed parcel, with common [temperature](../../../../../../../temperature.md) $T$, total [pressure](../../../../../../../pressure.md) $P$, and molar species amounts $N_i$. Define $N=\sum_iN_i$ and [volume mixing ratios](../../../../../../../volume-mixing-ratio.md) $x_i=N_i/N$, so $\sum_i x_i=1$. Ideal mixing makes partial [pressure](../../../../../../../pressure.md) $P_i=x_iP$.

For a pure ideal species, $d\mu_i=-\bar S_i\,dT+\bar V_i\,dP_i$, with molar volume $\bar V_i=\mathcal RT/P_i$. At fixed [temperature](../../../../../../../temperature.md), integration from standard [pressure](../../../../../../../pressure.md) $P^\circ$ gives

$$
\mu_i(T,P_i)=\mu_i^\circ(T)+\mathcal RT\log(P_i/P^\circ).
$$

The same logarithmic composition term follows from the ideal mixing [entropy](../../../../../../../entropy.md) $\Delta S_{\rm mix}=-\mathcal R\sum_iN_i\log x_i$. Extensivity gives $G=\sum_iN_i\mu_i$. Hence the [Gibbs free energy of an ideal-gas mixture](../../../../../../../gibbs-free-energy-of-an-ideal-gas-mixture.md) is

$$
\boxed{G(T,P,\{N_i\})=N\sum_i x_i\mu_i^\circ(T)
+N\mathcal RT\left[\log(P/P^\circ)+\sum_i x_i\log x_i\right].}
$$

Equivalently, write each standard chemical term as $\mu_i^\circ=h_i^\circ-Ts_i^\circ$, using molar [enthalpy](../../../../../../../enthalpy.md) and [entropy](../../../../../../../entropy.md). For zero abundance the limit $x\log x\to0$ defines the extensive expression continuously.

The fractions alone do not specify the extensive [Gibbs free energy](../../../../../../../gibbs-free-energy.md): the total amount $N$ or an equivalent elemental inventory must also be fixed. Moreover, in a chemically closed reacting system $N$ need not remain constant; for example, hydrogenation of [carbon monoxide](../../../../../../../carbon-monoxide.md) changes the total molecular count while conserving atoms. Minimization is therefore over species amounts subject to elemental constraints, rather than over fractions with an artificially fixed molecular count. Nonideal gases require activities or fugacities; condensates contribute separate phase terms.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
