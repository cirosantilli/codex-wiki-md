<h1 id="section-b/10/i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a monolithic series-connected [multi-junction solar cell](../../../../../../../multi-junction-solar-cell.md), **all junctions carry the same terminal current**, so a weakly illuminated junction limits the useful series current. Adjust absorber thicknesses, compositions and optical coupling to balance collected photocurrent. Tunnel interconnects provide electrical continuity; low-loss contacts and interfaces also matter. Equal incident energy in each spectral band would not guarantee equal current, because photon counts and collection efficiencies differ.

Put the largest bandgap at the illuminated top and the smallest at the bottom:

$$
\boxed{\text{light}\ \longrightarrow\
\mathrm{InGaAlP}\ (1.88\,eV)\ \longrightarrow\
\mathrm{InGaAs}\ (1.40\,eV)\ \longrightarrow\
\mathrm{Ge}\ (0.67\,eV).}
$$

The top absorber captures high-energy photons while transmitting lower-energy photons to the subsequent layers. Placing germanium first would absorb photons that the higher-gap cells could use at higher [voltage](../../../../../../../voltage.md).

The absorption edges are approximately

$$
\lambda_1=660\,\mathrm{nm},\qquad
\lambda_2=886\,\mathrm{nm},\qquad
\lambda_3=1850\,\mathrm{nm}.
$$

For ideal sharp, complete absorption without reflection, the available plotted spectral bands are therefore the visible region below $660\,\mathrm{nm}$ for the top cell, $660$–$886\,\mathrm{nm}$ for the middle cell, and $886$–$1850\,\mathrm{nm}$ for germanium. Photons beyond $1850\,\mathrm{nm}$ pass all three ideal absorbers. The source plot begins around $350\,\mathrm{nm}$, so it does not supply an ultraviolet integral below that point.

Using coarse readings of the provided curve, the band integrals are of order $1.2\times10^4$, $0.7\times10^4$ and $1.2\times10^4$ in plotted-ordinate-units times nanometers, respectively. These are only approximate areas under a low-resolution graph, not calibrated radiances in SI units: the ordinate gives no physical unit or spectral normalization. The robust result is the band allocation; precise photocurrent matching needs a calibrated spectrum and each junction's external quantum efficiency,

$$
J_{{\rm ph},j}=e\int\mathrm{EQE}_j(\lambda)\frac{\lambda I_\lambda}{hc}\,d\lambda.
$$

Thus the diagram and band boundaries establish the intended stack, while the plot cannot justify precise watt-per-area or current values.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [I](../../i.md)
3. [10](../../../10.md)
4. [Section B](../../../../section-b.md)
5. [Paper 1](../../../../../paper-1-split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../split.md)
8. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
