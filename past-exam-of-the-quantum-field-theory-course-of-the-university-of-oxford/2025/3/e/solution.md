<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The corrected expression in [d](../d.md) is a [vacuum two-point function](../../../../vacuum-two-point-function.md), or [Wick contraction](../../../../wick-contraction.md), of the free [Dirac field](../../../../dirac-field.md). It equals the negative spinor transpose of the usual [Dirac propagator](../../../../dirac-propagator.md) with reversed spacetime arguments. It supplies the internal fermion lines in [Feynman diagrams](../../../../feynman-diagram.md), rather than a position-space detection probability.

For $x^0>y^0$, $\psi(y)$ creates an [antiparticle](../../../../antiparticle.md) and $\bar\psi(x)$ annihilates it. The $v\bar v$ term describes positive-energy [antiparticle](../../../../antiparticle.md) propagation from $y$ to $x$. For $y^0>x^0$, $\bar\psi(x)$ creates a [particle](../../../../particle-physics.md) and $\psi(y)$ annihilates it. The $u\bar u$ term describes positive-energy [particle](../../../../particle-physics.md) propagation from $x$ to $y$, with the minus sign required by exchanging the odd operators in [fermionic time ordering](../../../../fermionic-time-ordering.md). Neither term describes a physical negative-energy excitation.

The [Heaviside step functions](../../../../heaviside-step-function.md) select these chronological alternatives. The factors $e^{\mp ip\cdot z}$ are on-shell plane waves with $p^0=E_{\mathbf p}>0$, and $d\Pi_p$ is the positive-energy [Lorentz-invariant phase-space measure](../../../../lorentz-invariant-phase-space-measure.md). The sum over $s$ includes the two [spin](../../../../spin.md) states. With standard relativistic spinor normalization, the [fermion spin sums](../../../../fermion-spin-sum.md) are

$$
\sum_s u^s(\mathbf p)\bar u^s(\mathbf p)=\not{p}+\mu,\qquad
\sum_s v^s(\mathbf p)\bar v^s(\mathbf p)=\not{p}-\mu.
$$

They encode the [spinor](../../../../spinor.md) structure and solve the corresponding on-shell [Dirac equations](../../../../dirac-equation.md). In particular, the corrected answer can also be written

$$
C_{ab}(x,y)=\int\frac{d^4p}{(2\pi)^4}\frac{i(\not{p}-\mu)_{ba}}{p^2-\mu^2+i0}\,e^{-ip\cdot(x-y)}.
$$

The [Feynman i-epsilon prescription](../../../../feynman-i-epsilon-prescription.md) specifies the temporal boundary conditions of the [Green function](../../../../green-s-function-split.md); its positive- and negative-frequency residues reproduce the two terms and their relative minus sign. With $S_F$ defined in [d](../d.md),

$$
(i\not{\partial}-\mu)S_F(w)=i\delta^{(4)}(w)I.
$$

The contact term is fixed by the equal-time [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md). Choosing a value for $\theta(0)$ does not change the unequal-time sign demonstrated above.

Finally, [microcausality](../../../../microcausality.md) requires field [anticommutators](../../../../anticommutator.md) to vanish at spacelike separation; the time-ordered [vacuum two-point function](../../../../vacuum-two-point-function.md) itself need not vanish there. These facts are compatible with relativistic causality. The plus-plus expression printed in the paper lacks the [fermionic sign](../../../../fermionic-sign.md) needed for this standard [Dirac propagator](../../../../dirac-propagator.md) interpretation.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
