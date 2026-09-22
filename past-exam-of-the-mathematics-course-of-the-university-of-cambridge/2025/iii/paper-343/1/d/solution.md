<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In a [quantum-trajectory unravelling](../../../../../../quantum-trajectory-theory.md), a pure state evolves between jumps under

$$
H_{\rm eff}=H-\frac i2\sum_\alpha L_\alpha^\dagger L_\alpha,
$$

and a jump of type $\alpha$ sends $|\phi\rangle$ to $L_\alpha|\phi\rangle/\|L_\alpha|\phi\rangle\|$. Averaging $|\phi_t\rangle\langle\phi_t|$ over the stochastic jump records recovers $\rho(t)$.

Equivalently, over a short interval $dt$ use the operators in a [Kraus representation](../../../../../../kraus-representation.md)

$$
K_0=I-iH_{\rm eff}dt,
\qquad
K_\alpha=\sqrt{dt}\,L_\alpha,
$$

and the [Stinespring dilation](../../../../../../stinespring-dilation.md) $V=\sum_\mu K_\mu\otimes|\mu\rangle_E$. Iterating with fresh environment systems produces a pure system-environment history whose [partial trace](../../../../../../partial-trace.md) is the Lindblad evolution.

If the fixed point is pure, stationarity requires $L_\alpha|\psi_*\rangle=\ell_\alpha|\psi_*\rangle$ for every $\alpha$, together with preservation of its ray by the adjusted effective Hamiltonian. After shifting the jumps one may take it to be a [dark state of a Lindblad equation](../../../../../../dark-state-of-a-lindblad-equation.md). Once a trajectory reaches that ray, neither no-jump evolution nor a jump takes it away; in the example of part (c), a jump transfers any excited component directly into the singlet.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
