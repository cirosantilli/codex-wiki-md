<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Interpret the stated [free energy](../../../../thermodynamic-free-energy.md) as per lattice site of volume $v_0$. [Flory–Huggins solution theory](../../../../flory-huggins-solution-theory.md) counts [polymer](../../../../polymer-split.md) chains, giving the [entropy](../../../../entropy-split.md) term $(\varphi/N)\ln\varphi$, and [solvent](../../../../solvent.md) molecules, giving $(1-\varphi)\ln(1-\varphi)$. The interaction term penalizes unlike contacts when $\chi>0$; a simple contact model has $\chi=z[\epsilon_{ps}-(\epsilon_{pp}+\epsilon_{ss})/2]/(k_BT)$. Connectivity reduces [polymer](../../../../polymer-split.md) [translational entropy](../../../../translational-entropy.md) relative to independent [monomers](../../../../monomer.md). This is an incompressible mean-field model with composition-independent $\chi$ for the calculations below.[1942, connected-chain combinatorial entropy and mixing free energy](../../../../thermodynamics-of-high-polymer-solutions-by-paul-j-flory.md)

Expanding the dilute [osmotic pressure](../../../../osmotic-pressure.md) identifies the effective second virial coefficient. A [good solvent](../../../../good-solvent.md) has $\chi<1/2$ and positive [excluded volume](../../../../excluded-volume.md), promoting swollen chains. A [poor solvent](../../../../poor-solvent.md) has $\chi>1/2$, favouring contraction and potentially phase separation. The theta-solvent condition is $\chi=1/2$ in this long-chain mean-field description: the second virial term vanishes, but higher terms remain. For finite $N$, this condition is not the exact critical point, which instead has $\chi_c=(1+N^{-1/2})^2/2$.

Let $g=f_{\rm mix}/(k_BT)$. The [osmotic pressure in Flory-Huggins solution theory](../../../../osmotic-pressure-in-flory-huggins-solution-theory.md) is

$$
\boxed{\Pi=\frac{k_BT}{v_0}(\varphi g'-g)
=-\frac{k_BT}{v_0}\left[\ln(1-\varphi)+(1-1/N)\varphi+\chi\varphi^2\right].}
$$

Thus $\Pi=(k_BT/v_0)[\varphi/N+(1/2-\chi)\varphi^2+\varphi^3/3+\cdots]$. For [mass](../../../../mass.md) [concentration](../../../../concentration.md) $c=\rho_p\varphi$ and chain molar [mass](../../../../mass.md) $M_n=N\rho_pv_0N_A$,

$$
\frac\Pi c=\frac{RT}{M_n}+B c+O(c^2).
$$

[osmometry](../../../../osmometry.md) uses a membrane permeable to [solvent](../../../../solvent.md) but retaining every [polymer](../../../../polymer-split.md) chain, at known uniform [temperature](../../../../temperature-split.md). Extrapolate $\Pi/c$ to zero [concentration](../../../../concentration.md) to remove interactions; the intercept gives the [number-average molar mass](../../../../number-average-molar-mass.md). Aggregation, leakage of small chains, [ions](../../../../ion.md) with a Donnan contribution, or a poor-solvent two-phase sample invalidate the simple molecular-weight interpretation.

The measured ratios give an exactly linear reduced-pressure fit:

$$
\boxed{\Pi/c=185+750c\quad\text{in the stated SI concentration units},\qquad
M_n=\frac{RT}{185}.}
$$

The [reduced osmotic-pressure intercept](../../../../reduced-osmotic-pressure-intercept.md) is $185\,\mathrm{Pa\,m^3\,kg^{-1}}$. The data determine **$M_n/T=0.04494\,\mathrm{kg\,mol^{-1}\,K^{-1}}$**; the measurement [temperature](../../../../temperature-split.md) is needed to convert this into an absolute [molar mass](../../../../molar-mass.md). For an explicitly assumed room [temperature](../../../../temperature-split.md) $T=300\,\mathrm K$, **$M_n\simeq13.5\,\mathrm{kg\,mol^{-1}}=1.35\times10^4\,\mathrm{g\,mol^{-1}}$**. The boxed expression is the general answer for an arbitrary experimental [temperature](../../../../temperature-split.md).

<a id="3/image-original-reduced-osmotic-pressure-regression-and-its-zero-concentration-intercept"></a>
![](../../../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2014/paper-1-osmometry.png)

**[Figure 3](#3/image-original-reduced-osmotic-pressure-regression-and-its-zero-concentration-intercept). Original reduced-osmotic-pressure regression and its zero-concentration intercept**.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
