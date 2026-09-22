<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

Assume dilute nondegenerate nonrelativistic particles, a common temperature, chemical equilibrium, charge neutrality $n_p=n_e$, and photons with zero chemical potential. The reaction balance gives $\mu_p+\mu_e=\mu_H$. Dividing the two charged-species equilibrium densities by the neutral density cancels their chemical-potential factors and leaves

$$
\frac{n_pn_e}{n_H}=\frac{g_pg_e}{g_H}\left(\frac{2\pi kT}{h^2}\frac{m_pm_e}{m_H}\right)^{3/2}\exp\left[-\frac{(m_p+m_e-m_H)c^2}{kT}\right].
$$

For ground-state hydrogen, $g_p=g_e=2$ and $g_H=4$, and $m_H\simeq m_p$ in the thermal prefactor. The rest-mass difference is $I/c^2$. These approximations give the [Saha ionization equation](../../../../../saha-ionization-equation.md)

$$
\boxed{\frac{n_e^2}{n_H}=\left(\frac{2\pi m_ekT}{h^2}\right)^{3/2}e^{-I/(kT)}.}
$$

Excited levels or different degeneracy conventions would change the prefactor; the stated assumptions give the printed normalization.

Write the right side as $S(T)$. Since $n_e=X_en_B$ and $n_H=(1-X_e)n_B$, the [hydrogen ionization fraction](../../../../../hydrogen-ionization-fraction.md) obeys $X_e^2/(1-X_e)=S(T)/n_B$. With $n_B=\eta n_\gamma$, the given blackbody photon density then yields

$$
\boxed{\frac{1-X_e}{X_e^2}=\frac{4\sqrt2\,\zeta(3)}{\sqrt\pi}\,\eta\left(\frac{kT}{m_ec^2}\right)^{3/2}e^{I/(kT)}.}
$$

There are vastly more photons than baryons. Even when the typical photon energy is below the ionization energy, the high-energy tail can contain enough ionizing photons to keep nearly every baryon ionized. Neutral hydrogen forms only when that tail becomes sufficiently depleted relative to the very small baryon-to-photon ratio. This entropy/number-density effect explains why [cosmological recombination](../../../../../recombination-cosmology.md) occurs at a temperature far below $I$, rather than simply when $kT$ first falls below the binding energy. The [Saha ionization equation](../../../../../saha-ionization-equation.md) describes the equilibrium estimate; late kinetic freeze-out is a separate limitation of that approximation.

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
