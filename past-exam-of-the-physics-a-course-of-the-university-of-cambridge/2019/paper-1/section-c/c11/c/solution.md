<h1 id="section-c/c11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [observable](../../../../../../observable.md) is represented by a [self-adjoint operator](../../../../../../self-adjoint-operator.md). For an ideal [projective measurement](../../../../../../projective-measurement.md), let $P_a$ be its spectral projector for outcome $a$. The [Born rule](../../../../../../born-rule.md) gives $p(a)=\langle\psi|P_a|\psi\rangle$, or $p(a)=\operatorname{tr}(\rho P_a)$ for a [density matrix](../../../../../../density-matrix-split.md) $\rho$. Conditional on obtaining $a$, the [Lüders rule](../../../../../../luders-rule.md) gives

$$
\boxed{|\psi\rangle\longmapsto\frac{P_a|\psi\rangle}{\sqrt{p(a)}},\qquad \rho\longmapsto\frac{P_a\rho P_a}{p(a)}.}
$$

For a degenerate outcome this projects onto the whole associated [eigenspace](../../../../../../eigenspace.md), rather than arbitrarily selecting a vector within it. An immediate repeated ideal measurement returns the same outcome, provided there is no intervening evolution or disturbance.

Commuting finite-dimensional [observables](../../../../../../observable.md) admit a common [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md); their projectors commute and ideal joint measurements are compatible. Noncommuting [observables](../../../../../../observable.md) generally have no complete common [eigenbasis](../../../../../../eigenbasis.md), and measurement order can affect the subsequent statistics. Particular common [eigenvectors](../../../../../../eigenvector.md) can nevertheless exist, so a nonzero [commutator](../../../../../../commutator.md) does not mean that every state has a nonzero uncertainty in both quantities.

For a quantitative constraint, apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) to $(A-\langle A\rangle)|\psi\rangle$ and $(B-\langle B\rangle)|\psi\rangle$. The imaginary part of their [inner product](../../../../../../inner-product-split.md) is $\langle[A,B]\rangle/(2i)$, giving the [Robertson uncertainty principle](../../../../../../robertson-uncertainty-principle.md)

$$
\boxed{\Delta A\,\Delta B\geq\frac12|\langle[A,B]\rangle|.}
$$

The [canonical commutation relation](../../../../../../canonical-commutation-relation.md) $[x,p]=i\hbar$ gives $\Delta x\,\Delta p\geq\hbar/2$. Retaining the real part of the same [inner product](../../../../../../inner-product-split.md) gives the stronger [Robertson-Schrödinger uncertainty relation](../../../../../../robertson-schrodinger-uncertainty-relation.md), including a [covariance](../../../../../../covariance.md) term. These are constraints on the preparation of a [quantum state](../../../../../../quantum-state.md), not simply statements about a poorly calibrated instrument.

A sequential [spin one-half](../../../../../../spin-one-half.md) example makes the change in statistics explicit. Prepare $|+z\rangle$. An immediate $S_z$ measurement is certainly positive. If an $S_x$ measurement is inserted first, its outcomes each have [probability](../../../../../../probability.md) $1/2$ and leave states $|\pm x\rangle$. Each then yields either $S_z$ result with [probability](../../../../../../probability.md) $1/2$, so the final positive fraction is $1/2$. The change reflects projection onto incompatible [spin eigenstates](../../../../../../spin-eigenstate.md), even with ideal measuring apparatus. The theory of [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) allows more general state-update rules, but the operator description and the [Born rule](../../../../../../born-rule.md) still constrain their [probabilities](../../../../../../probability.md).

## ↑ Ancestors (15)

1. [C](../c.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
