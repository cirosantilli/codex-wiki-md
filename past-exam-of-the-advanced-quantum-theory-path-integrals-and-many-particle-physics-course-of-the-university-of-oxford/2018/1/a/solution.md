<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With no pairing, the [Hamiltonian](../../../../hamiltonian.md) is diagonal in the [fermionic occupation numbers](../../../../fermionic-occupation-number.md). The [Pauli exclusion principle](../../../../pauli-exclusion-principle.md) allows each momentum mode to be either empty or occupied once. Without a fixed [fermion number](../../../../fermion-number.md) constraint, occupying a mode lowers the [energy](../../../../energy-split.md) precisely when its single-particle [energy](../../../../energy-split.md) is negative. Therefore, with $|0\rangle$ the [Fock vacuum](../../../../fock-vacuum.md), a [ground state](../../../../ground-state.md) is

$$
\boxed{|\mathrm{GS}\rangle=\prod_{p:\,\epsilon(p)<0}c_p^\dagger|0\rangle,\qquad E_{\mathrm{GS}}=\sum_{p:\,\epsilon(p)<0}\epsilon(p).}
$$

Choose a fixed ordering of the [fermionic creation operators](../../../../fermionic-creation-operator.md); changing it alters only the overall [phase](../../../../phase-waves.md). Any zero-energy modes may be occupied or empty without changing the [ground-state energy](../../../../ground-state-energy.md).

To identify the occupied modes, complete the square:

$$
\frac{\epsilon(p)}\alpha=\left(p^2-\frac\beta2\right)^2+\mu-\frac{\beta^2}{4}.
$$

Here $\beta$ is the dispersion parameter, not [inverse temperature](../../../../inverse-temperature.md). If $\beta^2<4\mu$, every mode has positive [energy](../../../../energy-split.md) and the unique [ground state](../../../../ground-state.md) is the [Fock vacuum](../../../../fock-vacuum.md), with $E_{\mathrm{GS}}=0$. If $\beta^2=4\mu$, there are still no negative-energy modes, but $p=\pm\sqrt{\beta/2}$ have zero [energy](../../../../energy-split.md) if they lie on the allowed momentum grid. Each such mode doubles the [ground-state degeneracy](../../../../ground-state-degeneracy.md).

For $\beta^2>4\mu$, define

$$
p_-^2=\frac{\beta-\sqrt{\beta^2-4\mu}}2,\qquad
p_+^2=\frac{\beta+\sqrt{\beta^2-4\mu}}2.
$$

Both are positive, and the occupied [Fermi sea](../../../../fermi-sea.md) consists of the two intervals $p_-<|p|<p_+$. With $p=2\pi n/L$, the requested finite-size [ground-state energy](../../../../ground-state-energy.md) is explicitly

$$
\boxed{E_{\mathrm{GS}}=2\alpha\!\sum_{\substack{n\in\mathbb Z_{>0}\\ Lp_-/(2\pi)<n<Lp_+/(2\pi)}}\left[\left(\frac{2\pi n}L\right)^4-\beta\left(\frac{2\pi n}L\right)^2+\mu\right].}
$$

The factor two counts opposite momenta. Endpoints are excluded from this [sum](../../../../sum.md) because they have zero [energy](../../../../energy-split.md); when an endpoint is allowed, its optional occupation adds [ground-state degeneracy](../../../../ground-state-degeneracy.md). A narrow negative-energy interval can contain no allowed finite-size momenta, in which case the [sum](../../../../sum.md) is empty. The zero-momentum mode is always empty since $\epsilon(0)=\alpha\mu>0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
