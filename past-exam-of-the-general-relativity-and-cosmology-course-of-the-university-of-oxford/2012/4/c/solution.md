<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume an ideal nondegenerate hydrogen gas in [thermal equilibrium](../../../../thermal-equilibrium-split.md) and [chemical equilibrium](../../../../chemical-equilibrium.md), with ground-state atoms and charge neutrality. Let $n_p=n_e=Xn_B$ and $n_H=(1-X)n_B$. The ground-state [Saha equation](../../../../saha-ionization-equation.md), with the usual electron/proton spin factors cancelling the atomic ground-state degeneracy, is

$$
\frac{n_en_p}{n_H}=\left(\frac{m_ek_BT}{2\pi\hbar^2}\right)^{3/2}e^{-B/(k_BT)}.
$$

Invert it and use $n_B=n_\gamma/s=(0.24/s)(k_BT/(\hbar c))^3$. This gives

$$
\frac{1-X}{X^2}=\frac{0.24(2\pi)^{3/2}}s\left(\frac{k_BT}{m_ec^2}\right)^{3/2}e^{B/(k_BT)},
$$

so

$$
\boxed{\frac{1-X}{X^2}\simeq\frac{3.8}s\left(\frac{k_BT}{m_ec^2}\right)^{3/2}\exp\frac{B}{k_BT}.}
$$

Here $m_e$ is the electron mass denoted $M_e$ in the source, and $0.24(2\pi)^{3/2}=3.78$. At $X=1/2$, the left side is two. At $k_BT$ of order $B$, the right side is extremely small because $1/s\sim10^{-9}$ and $B/(m_ec^2)\ll1$. A large exponential is needed to compensate, requiring $B/(k_BT)\gg1$ rather than a temperature of order the binding energy.

Physically, there are enormously many photons per baryon, so even a small high-energy tail of the thermal photon distribution can maintain ionization. Recombination is delayed until that tail is sufficiently depleted. This explains the low recombination temperature without solving the equilibrium equation; actual cosmological recombination also eventually requires rate equations once equilibrium fails.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
