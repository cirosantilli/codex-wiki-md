<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work in [natural units](../../../../../natural-units.md) $k_B=\hbar=c=1$, initially neglecting helium and excited hydrogen states. The reaction $p+e^-\leftrightarrow H+\gamma$ is in [chemical equilibrium](../../../../../chemical-equilibrium.md) when $\mu_p+\mu_e=\mu_H$, since equilibrium photons have zero chemical potential. Substitution of the nonrelativistic [Maxwell-Boltzmann distribution](../../../../../maxwell-boltzmann-distribution.md) for the three densities gives

$$
\frac{n_pn_e}{n_H}=\frac{g_pg_e}{g_H}\left(\frac{m_pm_eT}{2\pi m_H}\right)^{3/2}\exp\left[-\frac{m_p+m_e-m_H}{T}\right].
$$

For ground-state hydrogen use $g_e=g_p=2$, $g_H=4$, and $m_H\simeq m_p$ in the translational prefactor. Writing its [Hydrogen binding energy](../../../../../hydrogen-binding-energy.md) as $I$, this becomes $(m_eT/(2\pi))^{3/2}e^{-I/T}$. Charge neutrality gives $n_p=n_e=X_en_B$, while baryon conservation gives $n_H=(1-X_e)n_B$. Hence the [hydrogen-only Saha equation](../../../../../hydrogen-only-saha-equation.md) is

$$
\boxed{\frac{1-X_e}{X_e^2}=n_B\left(\frac{2\pi}{m_eT}\right)^{3/2}e^{I/T}.}
$$

The photon [Bose-Einstein distribution](../../../../../bose-einstein-distribution.md) supplies $n_\gamma=2\zeta(3)T^3/\pi^2$, where $\zeta(3)$ is the usual [Riemann zeta function](../../../../../riemann-zeta-function.md) value in the thermal number integral. With [baryon-to-photon ratio](../../../../../baryon-to-photon-ratio.md) $\eta_\gamma=n_B/n_\gamma$, substitution yields

$$
\boxed{\frac{1-X_e}{X_e^2}=\frac{2\zeta(3)}{\pi^2}\eta_\gamma\left(\frac{2\pi T}{m_e}\right)^{3/2}e^{I/T}.}
$$

This reproduces the requested numerical coefficient, with the printed $\xi(3)$ interpreted as the thermal $\zeta(3)$ value. There is a normalization ambiguity in the PDF: it writes $\eta=n_B/s$ without defining $s$. To reproduce this coefficient, $s$ must mean photon number density. If $s$ has its usual [entropy density](../../../../../entropy-density.md) meaning, the [Saha baryon-abundance normalization](../../../../../saha-baryon-abundance-normalization.md) instead gives

$$
s=\frac{2\pi^2}{45}g_{*s}T^3,\qquad \eta_s=\frac{n_B}{s},\qquad
\boxed{\frac{1-X_e}{X_e^2}=\frac{2\pi^2}{45}g_{*s}\eta_s\left(\frac{2\pi T}{m_e}\right)^{3/2}e^{I/T}.}
$$

The two forms agree through $\eta_\gamma=[\pi^4g_{*s}/(45\zeta(3))]\eta_s$, with the entropy sector specified. A baryon-to-entropy ratio cannot simply be inserted into the photon-normalized expression.

As the universe cools, the Boltzmann factor favors neutral atoms and [cosmological recombination](../../../../../recombination-cosmology.md) sharply lowers $X_e$. For an order-one ionized fraction the photon-normalized equation gives the balance

$$
\frac IT\simeq\log\left[\frac{\pi^2}{2\zeta(3)\eta_\gamma}\left(\frac{m_e}{2\pi T}\right)^{3/2}\right]
$$

up to an order-one ionization-fraction factor. The small baryon abundance means that there are very many photons per baryon: even a small high-energy photon tail can ionize most atoms. Thus the [recombination temperature](../../../../../recombination-temperature.md) is far below the microscopic binding scale $I\simeq13.6\,\mathrm{eV}$, typically a few tenths of an eV for the standard abundance, rather than of order $I$.

[Photon decoupling](../../../../../photon-decoupling.md) is a related but distinct kinetic event. The [Thomson scattering](../../../../../thomson-scattering.md) rate $n_e\sigma_T$ falls relative to $H$ as free electrons disappear, and photons begin free streaming. The precise last-scattering epoch depends on integrated optical depth, not only the local equality of rates. At still lower density the effective recombination rate per electron also drops below the expansion rate. [Residual electron freeze-out](../../../../../residual-electron-freeze-out.md) leaves a small nonzero ionized fraction, larger than the vanishingly small equilibrium Saha prediction; radiative atomic bottlenecks mean the entire history cannot be obtained from equilibrium alone.

The temperature comparison in the last request needs an interpretation. If “reionisation temperature” means the microscopic thermal ionization scale, the large photon-to-baryon ratio explains why cosmological recombination requires $T\ll I$. If it means later cosmic [reionization](../../../../../reionization.md), there is no universal thermal threshold: stars or other sources supply ionizing photons and can reheat gas. The cosmological photon background is actually colder at that later epoch, because $T_\gamma\propto a^{-1}$. Its temperature therefore cannot literally be higher than the background temperature at recombination merely because hydrogen is reionized.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
