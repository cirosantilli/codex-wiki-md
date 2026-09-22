<h1 id="9b/solution">Solution</h1>

↑ **Parent:** [9B](../9b.md)

In the nonrelativistic regime,

$$
E(p)=mc^2+\frac{p^2}{2m}+O\!\left(\frac{p^4}{m^3c^2}\right).
$$

The assumption $E-\mu\gg k_BT$ puts the [Fermi-Dirac distribution](../../../../../fermi-dirac-distribution.md) in its [Maxwell-Boltzmann limit](../../../../../maxwell-boltzmann-distribution.md), so

$$
\begin{aligned}
n&\simeq\frac{4\pi g_s}{h^3}
e^{(\mu-mc^2)/(k_BT)}
\int_0^\infty p^2e^{-p^2/(2mk_BT)}\,dp\\
&=\frac{4\pi g_s}{h^3}
e^{(\mu-mc^2)/(k_BT)}
\frac{\sqrt\pi}{4}(2mk_BT)^{3/2}.
\end{aligned}
$$

Therefore the [nonrelativistic Maxwell--Boltzmann number density](../../../../../nonrelativistic-maxwell-boltzmann-number-density.md) is

$$
\boxed{
n=g_s\left(\frac{2\pi mk_BT}{h^2}\right)^{3/2}
\exp\left(\frac{\mu-mc^2}{k_BT}\right).}
$$

For $p+e^-\leftrightarrow H+\gamma$, [chemical equilibrium](../../../../../chemical-equilibrium.md) and the vanishing [photon chemical potential](../../../../../photon-chemical-potential.md) imply

$$
\mu_p+\mu_e=\mu_H.
$$

Applying the number-density formula to each massive species and eliminating the chemical potentials gives

$$
\frac{n_en_p}{n_H}
=\frac{g_eg_p}{g_H}
\left(\frac{2\pi k_BT}{h^2}\right)^{3/2}
\left(\frac{m_em_p}{m_H}\right)^{3/2}
\exp\left(-\frac{(m_p+m_e-m_H)c^2}{k_BT}\right).
$$

Use charge neutrality, $n_p\simeq n_e$, the mass approximation $m_H\simeq m_p$, and the convention in the question that suppresses the order-one internal-degeneracy ratio $g_eg_p/g_H$. With the [Hydrogen binding energy](../../../../../hydrogen-binding-energy.md)

$$
E_{\rm bind}=(m_p+m_e-m_H)c^2,
$$

we obtain the [Saha ionization equation](../../../../../saha-ionization-equation.md)

$$
\boxed{
\frac{n_e^2}{n_H}\simeq
\left(\frac{2\pi m_ek_BT}{h^2}\right)^{3/2}
\exp\left(-\frac{E_{\rm bind}}{k_BT}\right).}
$$

The assumptions are [thermal equilibrium](../../../../../thermal-equilibrium.md) and [chemical equilibrium](../../../../../chemical-equilibrium.md) before [cosmological recombination](../../../../../recombination-cosmology.md), a [nonrelativistic nondegenerate gas](../../../../../nondegenerate-gas.md), zero [photon chemical potential](../../../../../photon-chemical-potential.md), [charge neutrality](../../../../../charge-neutrality.md), negligible proton-electron mass correction in the translational prefactor, and the stated [degeneracy-factor approximation](../../../../../degeneracy-factor.md).

## ↑ Ancestors (10)

1. [9B](../9b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
