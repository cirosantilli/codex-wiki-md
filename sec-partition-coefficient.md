# SEC partition coefficient

↑ **Parent:** [Size-exclusion chromatography](size-exclusion-chromatography.md)

For ideal [SEC](size-exclusion-chromatography.md), define the [SEC partition coefficient](sec-partition-coefficient.md) by

$$
K_d=\frac{\overline c_{\rm pore}}{c_{\rm interparticle}},\qquad
V_e=V_0+K_dV_i,\qquad
K_d=\frac{V_e-V_0}{V_t-V_0}.
$$

Here $\overline c_{\rm pore}$ averages [solute](solute.md) [concentration](concentration.md) over all pore liquid, including inaccessible regions. $V_e$ is column elution [volume](volume-thermodynamics.md). Pure steric exclusion gives $0\le K_d\le1$; the endpoints mean exclusion and full access.[GE Healthcare, Size Exclusion Chromatography: Principles and Methods, printed pp. 15–16: concentration-ratio definition and Kd limits](size-exclusion-chromatography-principles-and-methods-by-ge-healthcare.md)

A storage argument explains the relation. Assume a dilute stable [solute](solute.md), unchanged packing and [solvent](solvent.md), constant [volumetric flow rate](volumetric-flow-rate.md) $Q$, rapid local [chemical equilibrium](chemical-equilibrium.md) between pore liquid and interparticle liquid, negligible binding, and negligible transport through the pores by bulk flow. At interparticle [concentration](concentration.md) $c$, the column holds an [amount of substance](amount-of-substance.md) $n=cV_0+K_dcV_i$. Its exit transports $Qc$ per unit time. The ratio $n/(Qc)$ is the mean residence time in this equilibrium transport model; multiplying by $Q$ gives $V_e=V_0+K_dV_i$. For a narrow symmetric [SEC chromatogram](sec-chromatogram.md) peak, the peak maximum approximates that mean; a strongly asymmetric peak needs an explicitly stated location convention.

The handbook also uses an operational normalization

$$
K_{av}=\frac{V_e-V_0}{V_c-V_0}
=K_d\frac{V_i}{V_i+V_{\rm matrix}}.
$$

This denominator includes solid matrix, so full access gives $K_{av}<1$ when $V_{\rm matrix}>0$. It differs from the pore-liquid [SEC partition coefficient](sec-partition-coefficient.md). Read each source's volume convention before comparing coefficients.[GE Healthcare, Size Exclusion Chromatography: Principles and Methods, printed p. 16, Figure 1.8: Kav uses Vc, not Vt](size-exclusion-chromatography-principles-and-methods-by-ge-healthcare.md)

For an original numerical example, take $V_0=5\,\mathrm{mL}$, $V_i=8\,\mathrm{mL}$, and $V_{\rm matrix}=3\,\mathrm{mL}$. Then $V_t=13\,\mathrm{mL}$ and $V_c=16\,\mathrm{mL}$. Elution at $9\,\mathrm{mL}$ gives $K_d=1/2$ but $K_{av}=4/11$. Even a fully included tracer gives $K_{av}=8/11$, not $1$. These are stipulated volumes, not experimental measurements.

## ↑ Ancestors (5)

1. [Size-exclusion chromatography](size-exclusion-chromatography.md)
2. [Liquid chromatography](liquid-chromatography.md)
3. [Chromatography](chromatography-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [SEC partition coefficient](sec-partition-coefficient.md)
