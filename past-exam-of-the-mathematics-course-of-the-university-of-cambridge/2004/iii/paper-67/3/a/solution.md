<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the [Maxwell-Boltzmann velocity distribution](../../../../../../maxwell-boltzmann-velocity-distribution.md), each Cartesian component has mean-square velocity $k_BT_e/m_e$. Thus $\langle v^2\rangle=3k_BT_e/m_e$. The original PDF calls this quantity an rms velocity, but the rms speed is its square root. Also, its $n_\gamma$ must mean the dimensionless mean [occupation number](../../../../../../occupation-number.md) $n$, since its equilibrium value is a [Planck photon distribution](../../../../../../planck-photon-distribution.md); it is not the frequency-integrated [photon number density](../../../../../../photon-number-density.md).

Take $x=h\nu/(k_BT_\gamma)$ at a fixed local radiation temperature. Because $x$ is proportional to [frequency](../../../../../../frequency.md),

$$
\nu^2\partial_\nu^2n+4\nu\partial_\nu n
=x^2\partial_x^2n+4x\partial_xn
=x^{-2}\partial_x(x^4\partial_xn).
$$

The hot-electron [Kompaneets equation](../../../../../../kompaneets-equation.md) therefore becomes

$$
\boxed{\frac{\partial n}{\partial y}=x^{-2}\frac{\partial}{\partial x}\left(x^4\frac{\partial n}{\partial x}\right),\qquad
dy=\frac{k_BT_e}{m_ec^2}n_e\sigma_Tc\,dt.}
$$

For traversal length $d\ell=c\,dt$, the [Compton y parameter](../../../../../../compton-y-parameter.md) is

$$
\boxed{y=\frac{\sigma_T}{m_ec^2}\int n_ek_BT_e\,d\ell
=\frac{\sigma_T}{m_ec^2}\int P_e\,d\ell.}
$$

It measures electron [pressure](../../../../../../pressure.md) integrated along the [line of sight](../../../../../../line-of-sight.md), or the [Thomson scattering](../../../../../../thomson-scattering.md) [optical depth](../../../../../../optical-depth.md) weighted by $k_BT_e/(m_ec^2)$. In this hot-electron limit the mean fractional [energy](../../../../../../energy.md) gain is approximately $4y$. The derivation assumes nonrelativistic electrons, Thomson-limit photon [energies](../../../../../../energy.md) and $T_e\gg T_\gamma$. The original PDF uses $h\nu$, as required for ordinary [frequency](../../../../../../frequency.md); the converted TeX incorrectly substitutes $\hbar\nu$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
