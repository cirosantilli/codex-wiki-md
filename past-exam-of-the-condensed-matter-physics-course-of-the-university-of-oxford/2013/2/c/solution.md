<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a one-dimensional free-electron gas of length $L$, allowed [wave vectors](../../../../wavevector.md) have spacing $2\pi/L$. Including two [spin](../../../../spin.md) states and occupied [wave vectors](../../../../wavevector.md) from $-k_F$ to $+k_F$,

$$
N_e=2\frac{L}{2\pi}(2k_F),\qquad
\boxed{k_F=\frac{\pi n_e}{2},\qquad
E_F=\frac{\hbar^2k_F^2}{2m_e}=\frac{\pi^2\hbar^2n_e^2}{8m_e}.}
$$

The ground-state [kinetic energy](../../../../kinetic-energy.md) is found by integrating rather than assigning every [electron](../../../../electron.md) the [Fermi energy](../../../../fermi-energy.md):

$$
K_e=2\frac{L}{2\pi}\int_{-k_F}^{k_F}\frac{\hbar^2k^2}{2m_e}\,dk
=\frac{L\hbar^2k_F^3}{3\pi m_e}
=\boxed{\frac13N_eE_F.}
$$

[Charge neutrality](../../../../charge-neutrality.md) gives $N_e=ZN$ because each positive ion has charge $+Ze$. Thus $K_e=ZNE_F/3$. Since the ion separation is $2R$, $L\simeq2RN$ and $n_e=Z/(2R)$. These are one-dimensional number densities and state counts; using a three-dimensional $k_F\propto n^{1/3}$ relation here would change the model. The results concern the ground-state Fermi-gas contribution, neglecting [electron](../../../../electron.md) interactions beyond the supplied electrostatic [energy](../../../../energy-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
