<h1 id="s12/3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use number concentrations and write the [electrochemical potential](../../../../../electrochemical-potential.md) of a sodium ion as $\widetilde\mu=\mu^\circ+k_{\rm B}T\ln c+e\psi$. Define the inward [sodium-motive force](../../../../../sodium-motive-force.md) as available work per positive charge for transport from outside to inside. With $V_m=\psi_i-\psi_o$,

$$
\boxed{\mathcal E_{\rm Na}=\frac{\widetilde\mu_o-\widetilde\mu_i}{e}=\frac{k_{\rm B}T}{e}\ln\frac{c_o}{c_i}-V_m.}
$$

Its negative is the signed inward free-energy cost per charge; stating this direction removes a common sign ambiguity.

Long-open sodium channels establish electrochemical equilibrium, $k_{\rm B}T\ln(c_{i0}/c_o)+eV_{m0}=0$. This does not generally require equal concentrations: impermeant counterions can support a nonzero equilibrium [membrane potential](../../../../../membrane-potential-split.md). Let $n_0=c_{i0}V$. For a large fixed-concentration external reservoir, after pumping $n$ ions out, $c_i(n)=(n_0-n)/V$ and $V_m(n)=V_{m0}-ne/C$. The [sodium export cost from a capacitive vesicle](../../../../../sodium-export-cost-from-a-capacitive-vesicle.md) for exporting another ion is

$$
\Delta G_{\rm Na}(n)=k_{\rm B}T\ln\frac{c_oV}{n_0-n}-eV_{m0}+\frac{ne^2}{C}=\boxed{\frac{ne^2}{C}+k_{\rm B}T\ln\frac{n_0}{n_0-n}}.
$$

The initial-equilibrium relation was used in the last step. The first term is the incremental electrical cost and the second is the change in chemical cost from their initial balanced values.

If the intended initial reference is uncharged with $V_{m0}=0$ and $c_{i0}=c_o$, then $n_0=c_oV$ and the requested form in the listed variables is

$$
\boxed{\Delta G_{\rm Na}(n)=\frac{ne^2}{C}+k_{\rm B}T\ln\frac{c_o}{c_o-n/V},\qquad 0<n<c_oV.}
$$

That equal-concentration reference is an additional assumption. For example, $c_{i0}=2c_o$ and $V_{m0}=-(k_{\rm B}T/e)\ln2$ also give zero initial sodium flux, but a different ion inventory. Thus the open-channel condition alone cannot determine $n_0$ from $c_oV$. If concentrations are molar rather than number densities, use the corresponding [Avogadro constant](../../../../../avogadro-constant.md) conversion and $RT$ for molar free energies. Treating the capacitor charge discretely gives a charging-energy increment $(n+1/2)e^2/C$ rather than the differential $ne^2/C$; the distinction is negligible for the thousands of ions used next.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [3](../../3.md)
3. [S12](../../../s12.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
