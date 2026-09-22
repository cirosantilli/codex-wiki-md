<h1 id="10/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret the supplied [free energies](../../../../../thermodynamic-free-energy.md) as standard reaction [free energies](../../../../../thermodynamic-free-energy.md) and use $c^\circ=1\,\mathrm{mol\,L^{-1}}$. The dimensionless [equilibrium constants](../../../../../equilibrium-constant.md) are

$$
K_C=\exp\!\left(-\frac{15000}{RT}\right)=2.3477\times10^{-3},
\qquad K_D=\exp\!\left(\frac{35000}{RT}\right)=1.3651\times10^6.
$$

Under the ideal-solution approximation, $[C]=K_C[L]$ and $[D]=(K_D/c^\circ)[L]^2$. Set $k_D=K_D/c^\circ$, with units $\mathrm{M^{-1}}$. Conservation counts two original [molecules](../../../../../molecule-split.md) in each [dimer](../../../../../dimer.md):

$$
c_0=[L]+[C]+2[D]=(1+K_C)[L]+2k_D[L]^2.
$$

The physical, positive root can be written without subtractive cancellation as

$$
\boxed{[L]=\frac{2c_0}{1+K_C+\sqrt{(1+K_C)^2+8k_Dc_0}}}.
$$

The resulting [concentrations](../../../../../concentration.md) are:

| Initial analytical [concentration](../../../../../concentration.md) | $[L]$/M | $[C]$/M | $[D]$/M |
| --- | --- | --- | --- |
| $0.100\,\mathrm M$ | **$1.9120\times10^{-4}$** | **$4.4888\times10^{-7}$** | **$0.0499042$** |
| $1.000\,\mathrm M$ | **$6.0502\times10^{-4}$** | **$1.4204\times10^{-6}$** | **$0.499697$** |

For example, the first row satisfies $[L]+[C]+2[D]=0.100\,\mathrm M$; using $[L]+[C]+[D]$ would incorrectly count [dimers](../../../../../dimer.md). At both [concentrations](../../../../../concentration.md) almost all molecular units belong to [dimers](../../../../../dimer.md).

[dimer](../../../../../dimer.md) formation is favored by sufficiently high [concentration](../../../../../concentration.md) because it joins two [molecules](../../../../../molecule-split.md). Dilution favors the separated species, whereas $[C]/[L]=K_C$ is concentration-independent in this ideal model. More than half the molecular units are dimerized when $2[D]>[L]+[C]$, equivalently $c_0>(1+K_C)^2/k_D\simeq7.36\times10^{-7}\,\mathrm M$. The supplied [free energies](../../../../../thermodynamic-free-energy.md) at one [temperature](../../../../../temperature-split.md) do not determine a [temperature](../../../../../temperature-split.md) trend without additional [enthalpy](../../../../../enthalpy-split.md) information. At $1\,\mathrm M$, neglected nonideal activities could be significant; the table is the requested concentration-based model.

## ↑ Ancestors (10)

1. [I](../i.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../split.md)
6. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
