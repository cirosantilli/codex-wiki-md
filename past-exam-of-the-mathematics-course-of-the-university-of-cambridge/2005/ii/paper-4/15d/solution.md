<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

In a large volume, one one-particle state occupies momentum-space volume $h^3/V$. A spherical shell of radius $p$ has volume $4\pi p^2dp$, so for spin degeneracy $g$ the [density of states](../../../../../density-of-states.md) is $4\pi gVp^2dp/h^3$. With ultra-relativistic dispersion $E=cp$ and zero [chemical potential](../../../../../chemical-potential.md), the [Bose-Einstein distribution](../../../../../bose-einstein-distribution.md) gives

$$
\epsilon=\frac{4\pi gc}{h^3}\int_0^\infty\frac{p^3\,dp}{e^{cp/(kT)}-1}
=\frac{4\pi g(kT)^4}{h^3c^3}\int_0^\infty\frac{x^3\,dx}{e^x-1}.
$$

The convergent dimensionless integral is $\pi^4/15$, obtained by expansion into exponentials and summing $\sum n^{-4}$. Therefore **$\epsilon\propto T^4$ and $\alpha=4$**. Photons are massless bosons with two polarizations; equilibrium emission and absorption do not conserve photon number and force $\mu_\gamma=0$.

For recombination, [chemical equilibrium](../../../../../chemical-equilibrium.md) imposes $\mu_p+\mu_e=\mu_H+\mu_\gamma=\mu_H$, including rest [energies](../../../../../energy.md) in the [chemical potentials](../../../../../chemical-potential.md). Divide the three nonrelativistic number-density expressions to obtain

$$
\frac{n_pn_e}{n_H}
=\frac{g_pg_e}{g_H}\left(\frac{2\pi kT}{h^2}\right)^{3/2}
\left(\frac{m_pm_e}{m_H}\right)^{3/2}e^{-I/(kT)}.
$$

Here $m_pc^2+m_ec^2-m_Hc^2=I$. Neglect the relative proton/hydrogen mass difference and take the ground-state degeneracy ratio $g_pg_e/g_H=1$ ([Electron](../../../../../electron.md) and proton spins give $2\cdot2$ and hydrogen gives $4$). [Charge neutrality](../../../../../charge-neutrality.md) gives $n_p=n_e$. This yields the stated [Saha equation](../../../../../saha-ionization-equation.md)

$$
\boxed{\frac{n_e^2}{n_H}
=\left(\frac{2\pi m_ekT}{h^2}\right)^{3/2}e^{-I/(kT)}}.
$$

With $n_e=X_en_B$ and $n_H=(1-X_e)n_B$, the ratio asked for is

$$
\boxed{\frac{1-X_e}{X_e^2}
=\eta\,16\pi\zeta(3)\left(\frac{kT}{hc}\right)^3
\left(\frac{h^2}{2\pi m_ekT}\right)^{3/2}e^{I/(kT)}}.
$$

Equivalently the prefactor is $16\pi\zeta(3)\eta(2\pi)^{-3/2}[kT/(m_ec^2)]^{3/2}$. Because photons vastly outnumber baryons, even a small high-energy tail can keep hydrogen ionized. Neutralization therefore requires exponential suppression of that tail far below $kT=I$, explaining the much lower recombination temperature. The equilibrium formula is an estimate; the actual expanding-universe recombination kinetics eventually depart from Saha equilibrium.

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
