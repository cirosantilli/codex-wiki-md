<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

For a [nonrelativistic particle](../../../../../nonrelativistic-particle.md), $E(p)=mc^2+p^2/(2m)$. The [Gaussian integral](../../../../../gaussian-integral.md) yields

$$
\boxed{n=g_s\left(\frac{2\pi m k_BT}{h^2}\right)^{3/2}
\exp\left(\frac{\mu-mc^2}{k_BT}\right).}
$$

Indeed $\int_0^\infty p^2e^{-p^2/(2mk_BT)}dp=\sqrt\pi(2mk_BT)^{3/2}/4$, which combines with $4\pi/h^3$ to give the prefactor. For the two species this gives

$$
\boxed{\frac{n_a}{n_b}=\frac{g_a}{g_b}\left(\frac{m_a}{m_b}\right)^{3/2}
\exp\left(\frac{\mu_a-\mu_b-(m_a-m_b)c^2}{k_BT}\right).}
$$

[Chemical equilibrium](../../../../../chemical-equilibrium.md) imposes $\mu_a+\mu_\alpha=\mu_b+\mu_\beta$. If the two massless bath species have zero [chemical potentials](../../../../../chemical-potential.md), then $\mu_a=\mu_b$; their masses alone do not imply this chemical-potential condition.

Weak reactions such as $n+\nu_e\leftrightarrow p+e^-$, with leptons treated as relativistic, interconvert [neutrons](../../../../../neutron.md) and [protons](../../../../../proton.md). Negligible lepton [chemical potentials](../../../../../chemical-potential.md) give approximately $n_n/n_p=\exp[-(m_n-m_p)c^2/(k_BT)]$, since their degeneracies and masses are nearly equal. Equilibrium favors [protons](../../../../../proton.md) increasingly as [temperature](../../../../../temperature.md) falls. But the weak reaction rate decreases faster than the expansion rate and eventually falls below it: [cosmological weak freeze-out](../../../../../cosmological-weak-freeze-out.md) prevents the ratio from following its equilibrium exponential to zero. Free [neutrons](../../../../../neutron.md) subsequently decay, reducing the frozen ratio further.

In [Big Bang nucleosynthesis](../../../../../big-bang-nucleosynthesis.md), cooling eventually makes deuterium survive photodissociation. Nuclear reactions then build [helium](../../../../../helium.md) through deuterium and the light intermediate nuclei, locking almost all surviving [neutrons](../../../../../neutron.md) into stable helium-four. Neglecting binding-energy corrections and taking $r=n_n/n_p\le1$, each [helium](../../../../../helium.md) nucleus uses two [neutrons](../../../../../neutron.md) and two [protons](../../../../../proton.md), so $n_{\rm He}=n_n/2$ and

$$
\boxed{Y_{\rm He}=\frac{4n_{\rm He}}{n_n+n_p}=\frac{2r}{1+r}.}
$$

For example $r=1/7$ gives a [helium](../../../../../helium.md) mass fraction $1/4$, with the remaining baryons predominantly hydrogen.

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
