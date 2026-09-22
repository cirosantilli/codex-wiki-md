<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

Expand the relativistic energy as $\epsilon(p)=mc^2+p^2/(2m)+O(p^4/(m^3c^2))$. In the dilute nonrelativistic regime the occupation denominator is dominated by its exponential, so the [Fermi-Dirac distribution](../../../../../fermi-dirac-distribution.md) reduces to the [Maxwell-Boltzmann distribution](../../../../../maxwell-boltzmann-distribution.md). The number density is then

$$
n\simeq\frac{4\pi g_s}{h^3}e^{(\mu-mc^2)/(kT)}\int_0^\infty p^2e^{-p^2/(2mkT)}\,dp
=\boxed{g_s\left(\frac{2\pi mkT}{h^2}\right)^{3/2}e^{(\mu-mc^2)/(kT)}}.
$$

The assumed low temperature makes the contributing momenta nonrelativistic; the large positive $(mc^2-\mu)/(kT)$ makes occupation numbers small.

For [chemical equilibrium](../../../../../chemical-equilibrium.md) of hydrogen ionization, $\mu_p+\mu_e=\mu_H+\mu_\gamma$, and thermal photons have $\mu_\gamma=0$. Apply the same dilute-gas expression to protons, electrons and ground-state hydrogen. Their density ratio is

$$
\frac{n_pn_e}{n_H}=\frac{g_pg_e}{g_H}\left(\frac{2\pi kT}{h^2}\frac{m_pm_e}{m_H}\right)^{3/2}e^{-(m_p+m_e-m_H)c^2/(kT)}.
$$

Assume charge neutrality with no other important ionic species, so $n_p=n_e$; neglect the binding-energy mass correction in $m_p/m_H$, so this ratio is approximately one. Including proton and electron spin gives $g_p=g_e=2$ and ground-state $g_H=4$, hence $g_pg_e/g_H=1$. Equivalently one may consistently omit nuclear spin from both proton and hydrogen degeneracies. Thus the [Saha equation](../../../../../saha-ionization-equation.md) is

$$
\boxed{\frac{n_e^2}{n_H}\simeq\left(\frac{2\pi m_ekT}{h^2}\right)^{3/2}e^{-I/(kT)}.}
$$

The assumptions are thermal and [chemical equilibrium](../../../../../chemical-equilibrium.md) at a common temperature, dilute nonrelativistic species, neutral total charge, predominantly ground-state hydrogen, and negligible interaction/partition-function corrections. The Maxwell-Boltzmann density formula applies to dilute hydrogen whether its composite spin makes it a boson or a fermion.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
