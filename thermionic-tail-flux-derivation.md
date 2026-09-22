# Thermionic tail-flux derivation

↑ **Parent:** [Richardson-Dushman law](richardson-dushman-law.md)

Consider a planar surface with outward normal along $z$. For an auxiliary equilibrium [electron gas](electron-gas.md) just outside it, let $n_v$ be the total [number density](number-density.md), counting both signs of $v_z$. Its [Maxwell-Boltzmann velocity distribution](maxwell-boltzmann-velocity-distribution.md) has normal-component density

$$
f_z(v_z)=\sqrt{\frac{m_e}{2\pi k_BT}}
e^{-m_ev_z^2/(2k_BT)}.
$$

An [electron](electron.md) with $v_z>0$ crosses more area per unit time when it moves faster. The outgoing number flux therefore uses $v_z f_z$, rather than just the probability of $v_z>0$:

$$
\Gamma=n_v\int_0^\infty v_zf_z(v_z)\,dv_z
=n_v\sqrt{\frac{k_BT}{2\pi m_e}}.
$$

This integral contributes only $T^{1/2}$. Holding a classical bulk [number density](number-density.md) fixed and imposing a normal [kinetic energy](kinetic-energy.md) threshold $W$ would instead give $\Gamma=n\sqrt{k_BT/(2\pi m_e)}e^{-W/(k_BT)}$; that argument alone does not produce $T^2$.

For the ideal surface model, measure external [electron](electron.md) energies from the metal's [chemical potential](chemical-potential-split.md) $\mu$. A freely propagating external state has $E-\mu=W+p^2/(2m_e)$. When $W\gg k_BT$, its [Fermi-Dirac distribution](fermi-dirac-distribution.md) reduces to the [Maxwell–Boltzmann statistics](maxwell-boltzmann-statistics.md) tail. Counting two [spin](spin.md) states per [phase space](phase-space.md) cell of volume $h^3$ gives

$$
n_v=\frac{2}{h^3}\int_{\mathbb R^3}
e^{-[W+p^2/(2m_e)]/(k_BT)}\,d^3p
=2\left(\frac{2\pi m_e k_BT}{h^2}\right)^{3/2}
e^{-W/(k_BT)}.
$$

Each of the three [Gaussian integrals](gaussian-integral.md) supplies $T^{1/2}$. Combining this $T^{3/2}$ state count with the $T^{1/2}$ crossing factor gives

$$
J=e\Gamma
=\frac{4\pi m_e e k_B^2}{h^3}\,T^2e^{-W/(k_BT)}.
$$

The auxiliary atmosphere supplies an equilibrium state-counting argument; an operating collector removes the outgoing [electrons](electron.md). It need not maintain a real equilibrium gas throughout the gap. Unit transmission and the ideal free [electron](electron.md) state count are substantive assumptions, so this calculation does not determine an arbitrary real surface's measured $A$.

In particular, [electrons](electron.md) inside a [metal](metal.md) generally form a degenerate [Fermi gas](fermi-gas.md). A classical distribution for the escaping tail does not imply a classical distribution for the whole interior. Richardson himself emphasized this distinction in his lecture.[Nobel Lectures, Physics 1922–1941; pp. 230–231, internal versus external electron statistics](nobel-lectures-physics-1922-1941/thermionic-phenomena-and-the-laws-which-govern-them-by-owen-willans-richardson.md)

## ↑ Ancestors (6)

1. [Richardson-Dushman law](richardson-dushman-law.md)
2. [Thermionic emission](thermionic-emission-split.md)
3. [Electron](electron.md)
4. [Subatomic particle](subatomic-particle.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Thermionic Richardson constant](thermionic-richardson-constant.md)
