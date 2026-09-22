<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [canonical momenta](../../../../canonical-momentum.md) are $\pi_k=\dot\phi_k$, so

$$
Q=\int d^3x\,(\phi_2\pi_1-\phi_1\pi_2).
$$

Different species commute at equal times, so these products have no ordering ambiguity and $Q$ is [Hermitian](../../../../hermitian-operator.md). Write $\int_{\mathbf p}=\int d^3p/(2\pi)^3$. Substituting the [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md) and using the spatial [Fourier transform](../../../../fourier-transform-split.md) identity gives

$$
\int d^3x\,\phi_2\pi_1
=-\frac i2\int_{\mathbf p}
(a_{2,\mathbf p}+a_{2,-\mathbf p}^\dagger)
(a_{1,-\mathbf p}-a_{1,\mathbf p}^\dagger).
$$

Subtract the expression with species interchanged. The two-annihilator terms cancel after $\mathbf p\mapsto-\mathbf p$, as do the two-creator terms. Commuting different species in the remaining terms yields

$$
\boxed{Q=-i\int_{\mathbf p}
(a_{2,\mathbf p}^\dagger a_{1,\mathbf p}-a_{1,\mathbf p}^\dagger a_{2,\mathbf p}).}
$$

There is no infinite [vacuum](../../../../vacuum.md) contribution to the [Noether charge](../../../../noether-charge.md) to subtract: the contractions that would generate a species-diagonal constant are absent.

The bosonic [canonical commutation relations](../../../../canonical-commutation-relation.md) give

$$
[Q,a_{1,\mathbf p}^\dagger]=-ia_{2,\mathbf p}^\dagger,
\qquad [Q,a_{2,\mathbf p}^\dagger]=ia_{1,\mathbf p}^\dagger.
$$

Define the [creation operators](../../../../creation-operator.md)

$$
c_{+,\mathbf p}^\dagger=\frac{a_{1,\mathbf p}^\dagger-ia_{2,\mathbf p}^\dagger}{\sqrt2},
\qquad
c_{-,\mathbf p}^\dagger=\frac{a_{1,\mathbf p}^\dagger+ia_{2,\mathbf p}^\dagger}{\sqrt2}.
$$

Their [commutators](../../../../commutator.md) with $Q$ are $[Q,c_\pm^\dagger]=\pm c_\pm^\dagger$. Since $Q|0\rangle=0$, the [one-particle states](../../../../one-particle-state.md) have

$$
\boxed{Q\,c_{\pm,\mathbf p}^\dagger|0\rangle
=\pm c_{\pm,\mathbf p}^\dagger|0\rangle.}
$$

The fixed-[momentum](../../../../momentum-split.md) states are delta-function normalized; a square-integrable [wave packet](../../../../wave-packet.md) of either species is a normalizable state with the same [Noether charge](../../../../noether-charge.md) [eigenvalue](../../../../eigenvalue.md). In this basis $Q=\int_{\mathbf p}(c_+^\dagger c_+-c_-^\dagger c_-)$, so it measures a difference of occupation numbers. The equal-time identity $i[Q,\phi_1]=\phi_2$, $i[Q,\phi_2]=-\phi_1$ independently checks the sign against [a](../a.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
