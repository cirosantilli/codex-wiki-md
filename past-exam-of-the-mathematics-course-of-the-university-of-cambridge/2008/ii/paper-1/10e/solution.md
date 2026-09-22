<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

In the nonrelativistic dilute regime, $E(p)=mc^2+p^2/(2m)+\cdots$ and $(mc^2-\mu)/kT\gg1$, so the Bose or Fermi correction in the denominator is negligible. The common [Maxwell-Boltzmann distribution](../../../../../maxwell-boltzmann-distribution.md) approximation gives

$$
n\simeq\frac{4\pi g_s}{h^3}e^{(\mu-mc^2)/kT}\int_0^\infty p^2e^{-p^2/(2mkT)}dp.
$$

Differentiating the quoted [Gaussian integral](../../../../../gaussian-integral.md) with respect to its squared scale gives $\int_0^\infty p^2e^{-ap^2}dp=\sqrt\pi/(4a^{3/2})$. Therefore

$$
\boxed{n=g_s\left(\frac{2\pi mkT}{h^2}\right)^{3/2}e^{(\mu-mc^2)/kT}.}
$$

[chemical equilibrium](../../../../../chemical-equilibrium.md) of $p+n\leftrightarrow D$ requires $\mu_D=\mu_p+\mu_n$. Apply the density formula to each species to obtain

$$
\frac{n_D}{n_nn_p}=\frac{g_D}{g_ng_p}\left(\frac{2\pi kT}{h^2}\right)^{-3/2}
\left(\frac{m_D}{m_nm_p}\right)^{3/2}e^{B_D/kT}.
$$

Using $g_n=g_p=2$, the specified $g_D=4$, and $m_n\simeq m_p$, $m_D\simeq2m_p$, gives

$$
\boxed{\frac{n_D}{n_nn_p}\simeq\left(\frac{\pi m_pkT}{h^2}\right)^{-3/2}e^{B_D/kT}.}
$$

For $X_a=n_a/n_B$ and $n_B=\eta n_\gamma$, the corresponding [deuterium equilibrium abundance](../../../../../deuterium-equilibrium-abundance.md) is

$$
\boxed{\frac{X_D}{X_nX_p}\simeq\frac{16\zeta(3)}{\sqrt\pi}\,\eta\left(\frac{kT}{m_pc^2}\right)^{3/2}e^{B_D/kT}.}
$$

The very small [baryon-to-photon ratio](../../../../../baryon-to-photon-ratio.md) means that even the high-energy tail contains many photons per baryon capable of destroying deuterium when $kT$ is of order $B_D$. Substantial deuterium survives only after that tail has been exponentially suppressed, so $B_D/kT$ must be large enough to offset the small prefactor. This is the [deuterium bottleneck](../../../../../deuterium-bottleneck.md), not a threshold set just by equality of thermal [energy](../../../../../energy.md) and binding [energy](../../../../../energy.md). The degeneracy $g_D=4$ is used as stipulated for this calculation.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
