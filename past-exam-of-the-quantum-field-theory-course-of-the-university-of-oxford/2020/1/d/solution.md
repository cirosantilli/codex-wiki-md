<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a connected amputated [Feynman diagram](../../../../feynman-diagram.md), write $L$ for the number of independent [loop momenta](../../../../loop-momentum.md). Each [loop momentum](../../../../loop-momentum.md) integration scales as $\lambda^4$, each internal [scalar propagator](../../../../scalar-propagator.md) as $\lambda^{-2}$, and each internal [Dirac propagator](../../../../dirac-propagator.md) as $\lambda^{-1}$ when both [four-momenta](../../../../four-momentum.md) and [mass](../../../../mass.md) are scaled. The [Yukawa coupling](../../../../yukawa-interaction.md) has [mass dimension](../../../../mass-dimension.md) zero. Thus

$$
d_S=4L-n_f-2n_s.
$$

Counting the two [fermion](../../../../fermion.md) ends and one scalar end at each [interaction vertex](../../../../interaction-vertex.md), and using connectedness, gives

$$
2n_f=2n_v,\qquad 2n_s+n=n_v,\qquad
L=n_f+n_s-n_v+1.
$$

Consequently $n_f=n_v$, $L=n_s+1$, and

$$
\boxed{d_S=4+2n_s-n_v=4-n.}
$$

**The requested exponent requires amputation and removal of the overall momentum delta function.** An ordinary unamputated connected [Green function](../../../../green-s-function-split.md) has an additional $n$ external [scalar propagators](../../../../scalar-propagator.md), giving [mass dimension](../../../../mass-dimension.md) $4-3n$ after stripping that delta function, or $-3n$ if it is retained. For a concrete check, the free two-point [scalar propagator](../../../../scalar-propagator.md) scales as $\lambda^{-2}$, not $\lambda^2$. The exponent $4-n$ is the engineering result for the amputated object. A fixed [renormalization scale](../../../../renormalization-scale.md) introduces logarithms; the displayed homogeneity is a naive [power counting](../../../../power-counting-in-quantum-field-theory.md) statement rather than an exact quantum scaling law at fixed subtraction scale.

More generally, with $E_s$ external scalar ends and $E_f$ external [fermion](../../../../fermion.md) ends, the same counting gives the [superficial degree of divergence](../../../../superficial-degree-of-divergence.md)

$$
\boxed{D=4-E_s-\frac32E_f.}
$$

This is an upper bound on the overall [ultraviolet divergence](../../../../ultraviolet-divergence.md). Numerator cancellations and [Lorentz invariance](../../../../lorentz-invariance.md) may lower it; an apparently convergent whole [Feynman diagram](../../../../feynman-diagram.md) can still have [ultraviolet subdivergences](../../../../ultraviolet-subdivergence.md). Local subtraction of those [ultraviolet subdivergences](../../../../ultraviolet-subdivergence.md) is required first.

For pure scalar ends, $E_s=0,1,2,3,4$ can require [counterterms](../../../../counterterm.md). [Lorentz invariance](../../../../lorentz-invariance.md) reduces the two-point terms to a [mass counterterm](../../../../mass-counterterm.md) and [wave-function renormalization](../../../../wave-function-renormalization.md); derivatives of a single scalar field are total derivatives, and a one-derivative cubic scalar term cannot be a [Lorentz scalar](../../../../lorentz-scalar.md). With two external [fermions](../../../../fermion.md), $E_s=0$ requires their [kinetic term](../../../../kinetic-term.md) and [mass counterterm](../../../../mass-counterterm.md), while $E_s=1$ requires [Yukawa coupling](../../../../yukawa-interaction.md) renormalization. Four external [fermions](../../../../fermion.md) give $D=-2$, so no independent four-[fermion](../../../../fermion.md) [counterterm](../../../../counterterm.md) is required.

A complete [counterterm Lagrangian](../../../../counterterm-lagrangian.md) consistent with the species symmetry can therefore be written

$$
\boxed{\begin{aligned}
\mathcal L_{\rm ct}={}&\frac{\delta Z_\phi}{2}(\partial\phi)^2
-\frac{\delta m_s^2}{2}\phi^2-\delta t\,\phi
-\frac{\delta\kappa}{3!}\phi^3-\frac{\delta\lambda_4}{4!}\phi^4-\delta\mathcal E\\
&+\sum_{i=1}^2\bar\psi_i(\delta Z_\psi i\not\partial-\delta m_f)\psi_i
-\delta g\,\phi\sum_{i=1}^2\bar\psi_i\psi_i.
\end{aligned}}
$$

The [vacuum energy density](../../../../vacuum-energy-density.md) term matters for an unnormalized [vacuum functional](../../../../vacuum-functional.md) and cancels from normalized [Green functions](../../../../green-s-function-split.md). The [tadpole counterterm](../../../../tadpole-counterterm.md) can impose $\langle\phi\rangle=0$. There is no $\phi\mapsto-\phi$ symmetry of the massive [Yukawa interaction](../../../../yukawa-interaction.md), so linear, cubic and quartic scalar terms cannot be excluded. For instance, in a constant background the divergent [fermion loop](../../../../fermion-loop.md) contribution contains $(m+g\phi)^4$, exhibiting all these powers. This is [counterterm closure of a massive Yukawa theory](../../../../counterterm-closure-of-a-massive-yukawa-theory.md).

The two species have identical couplings, so their common unitary flavour rotations preserve the [Lagrangian density](../../../../lagrangian-density.md) and their [counterterms](../../../../counterterm.md) can be chosen species independent. Equality of the scalar and [fermion](../../../../fermion.md) masses, however, is not protected: $\delta m_s^2$ and $\delta m_f$ are independent. Including the displayed finite set of operators yields a [renormalizable quantum field theory](../../../../renormalizable-quantum-field-theory.md). Restricting the bare [Lagrangian density](../../../../lagrangian-density.md) to the terms printed in the question is not closed under [renormalization](../../../../renormalization.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
