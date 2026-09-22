<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

In [chemical equilibrium](../../../../../chemical-equilibrium.md), the reaction $p+e\leftrightarrow H+\gamma$ obeys [chemical-potential balance for ionization](../../../../../chemical-potential-balance-for-ionization.md)

$$
\mu_p+\mu_e=\mu_H+\mu_\gamma=\mu_H,
$$

because a photon gas in equilibrium has [photon chemical potential](../../../../../photon-chemical-potential.md) $\mu_\gamma=0$. Applying the given nonrelativistic [Maxwell-Boltzmann distribution](../../../../../maxwell-boltzmann-distribution.md) to each massive species gives

$$
\frac{n_en_p}{n_H}
=\frac{g_eg_p}{g_H}
\left(\frac{2\pi k_BT}{h^2}\right)^{3/2}
\left(\frac{m_em_p}{m_H}\right)^{3/2}
\exp\left(-\frac{m_e+m_p-m_H}{k_BT}\right).
$$

The [Hydrogen binding energy](../../../../../hydrogen-binding-energy.md) is $I=m_e+m_p-m_H$ in units with $c=1$. Thus [Saha's equation](../../../../../saha-ionization-equation.md) is

$$
\boxed{
\frac{n_en_p}{n_H}
=\frac{g_eg_p}{g_H}
\left(\frac{2\pi k_BT}{h^2}\right)^{3/2}
\left(\frac{m_em_p}{m_H}\right)^{3/2}e^{-I/(k_BT)}.}
$$

For ground-state hydrogen, $g_e=g_p=2$ and $g_H=4$, so the degeneracy factor is one. Since $m_p\simeq m_H$, the translational factor is commonly written $(2\pi m_ek_BT/h^2)^{3/2}$.

Charge neutrality gives $n_e=n_p$. Write $n_B=n_e+n_H\simeq\eta n_\gamma$. Then

$$
n_e=X_en_B,
\qquad n_H=(1-X_e)n_B,
$$

and hence

$$
\frac{n_en_p}{n_H}=\frac{X_e^2}{1-X_e}n_B.
$$

Combining this with the stated photon density produces

$$
\boxed{
\frac{1-X_e}{X_e^2}
=\eta\,\frac{g_H}{g_eg_p}
\frac{16\pi\zeta(3)}{(2\pi)^{3/2}}
(k_BT)^{3/2}
\left(\frac{m_H}{m_em_p}\right)^{3/2}
e^{I/(k_BT)}.}
$$

In our universe the [baryon-to-photon ratio](../../../../../baryon-to-photon-ratio.md) is tiny, so there are roughly $10^9$ photons per baryon. Even when the mean photon energy is far below $I$, the high-energy [blackbody radiation](../../../../../black-body-radiation.md) tail contains enough ionizing photons to suppress neutral hydrogen. The [recombination temperature](../../../../../recombination-temperature.md) is reached only after the [Boltzmann factor](../../../../../boltzmann-factor.md) overwhelms this large photon-to-baryon ratio, at $k_BT\simeq0.3\,\mathrm{eV}$.

For a universe with $\eta=1$, take the degeneracy factor as one, $m_H\simeq m_p$, and define $x=I/(k_BT)$. Neutral formation occurs when the boxed ratio is of order one, giving approximately

$$
1\simeq\frac{4\sqrt2\,\zeta(3)}{\sqrt\pi}
\left(\frac{I}{m_ex}\right)^{3/2}e^x.
$$

With $I=13.6\,\mathrm{eV}$ and $m_e=5.11\times10^5\,\mathrm{eV}$, this gives $x\simeq19$ and therefore

$$
\boxed{k_BT\simeq0.7\,\mathrm{eV},}
$$

to order unity. This is much hotter than recombination in our universe because there is no enormous excess of photons, but it remains below $I$ because the electron's large translational phase space still favours the ionized state.

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
