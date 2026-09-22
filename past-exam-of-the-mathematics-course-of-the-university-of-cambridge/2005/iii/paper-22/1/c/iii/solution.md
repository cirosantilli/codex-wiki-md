<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Yoneda lemma](../../../../../../../yoneda-lemma.md), applied to the representing [Omega-spectrum](../../../../../../../omega-spectrum.md) spaces in each degree, makes the comparison more explicit. Put

$$
T_j=\Sigma^{-j}\Sigma^\infty D_j.
$$

The structure map of $D$ supplies $T_j\to T_{j+1}$, and $D$ is the [homotopy colimit of spectra](../../../../../../../homotopy-colimit-of-spectra.md) of this sequence. The inverse-tower transition on maps into $E$ is precomposition with $T_j\to T_{j+1}$. Under the [suspension spectrum](../../../../../../../suspension-spectrum.md) adjunction it takes $[D_{j+1},E_{j+1}]_*$ to $[D_j,E_j]_*$ by taking the adjoint through $D_j\to\Omega D_{j+1}$ and the [Omega-spectrum](../../../../../../../omega-spectrum.md) identification $E_j\simeq\Omega E_{j+1}$.

Consequently the maps of [represented cohomology theories](../../../../../../../represented-cohomology-theory.md) are exactly the compatible degreewise operations:

$$
\boxed{\operatorname{Nat}_{\Sigma}(\widetilde D^*,\widetilde E^*)\cong\lim_j[D_j,E_j]_* .}
$$

Only nonnegative degrees need be listed, since the suspension compatibility recovers the negative degrees. The [Milnor exact sequence for maps of spectra](../../../../../../../milnor-exact-sequence-for-maps-of-spectra.md) gives the sharper description

$$
0\longrightarrow\lim\nolimits^1_j[\Sigma D_j,E_j]_*\longrightarrow[D,E]_{\mathrm{st}}\longrightarrow\lim_j[D_j,E_j]_*\longrightarrow0.
$$

Thus $\operatorname{HPh}(D,E)\cong\lim^1_j[\Sigma D_j,E_j]_*$, with bonding maps coming from the same telescope. For an inverse tower $A_j$ with maps $r_j:A_{j+1}\to A_j$, $\lim A_j$ is the kernel and $\lim^1 A_j$ is the cokernel of

$$
\prod_j A_j\longrightarrow\prod_j A_j,\qquad(a_j)\longmapsto(a_j-r_j(a_{j+1})).
$$

**The first comparison quotients by spectrum homotopy; the second quotients by hyperphantom maps.** These are different identifications.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 22](../../../../paper-22-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
