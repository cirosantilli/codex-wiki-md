<h1 id="section-b/12/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Absorption generates electrons and holes in the perovskite. After relaxation toward the band edges, their nonequilibrium populations are described by separate electron and hole [quasi-Fermi levels](../../../../../../quasi-fermi-level.md). Selective contacts collect electrons through an electron-transport layer and holes through a hole-transport layer, while suppressing the opposite carriers.

For ideal contacts at open circuit,

$$
\boxed{qV_{\rm OC}\simeq E_{Fn}-E_{Fp}}.
$$

This [quasi-Fermi-level splitting](../../../../../../quasi-fermi-level-splitting.md) is not the band gap itself or simply the equilibrium built-in voltage. At equilibrium there is one common Fermi level and no extractable photovoltage. Under illumination at open circuit, generation is balanced by recombination while a nonzero population splitting persists.

<a id="section-b/12/i/image-selective-extraction-quasi-fermi-splitting-and-recombination-limited-solar-cell-voltage"></a>
![](../../../../../../past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2023/paper-1-additional-solar-cell.png)

**[Figure 8](#section-b/12/i/image-selective-extraction-quasi-fermi-splitting-and-recombination-limited-solar-cell-voltage). Selective extraction, quasi-Fermi splitting and recombination-limited solar-cell voltage**. Original qualitative energy diagram and stipulated illuminated diode curves. Trap-assisted and interface recombination reduce carrier splitting and open-circuit voltage. Band offsets, energy spacings and current scales are illustrative rather than fitted perovskite data.

Important parasitic paths include trap-assisted [Shockley-Read-Hall recombination](../../../../../../shockley-read-hall-recombination.md) in the bulk, at grain boundaries and at interfaces, and recombination at poorly selective contacts. They lower the steady carrier populations and their quasi-Fermi splitting. [Auger recombination](../../../../../../auger-recombination.md) can matter at high carrier densities but need not dominate an ordinary one-sun device. Radiative recombination is an unavoidable detailed-balance contribution, rather than an avoidable defect loss of the same kind.

An approximate illuminated diode relation is

$$
J(V)=J_{\rm SC}-J_0\left[e^{qV/(n_{\rm id}k_BT)}-1\right],
\qquad
V_{\rm OC}=\frac{n_{\rm id}k_BT}{q}\ln\left(1+\frac{J_{\rm SC}}{J_0}\right).
$$

Increased nonradiative recombination generally increases the dark recombination current and reduces $V_{\rm OC}$; it can also change ideality and fill factor. Shunts add a leakage path. Series resistance mainly reduces voltage under load and fill factor: its simple $IR_s$ drop vanishes at zero terminal current, so it should not be invoked as an automatic direct subtraction from open-circuit voltage.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12](../../12.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
