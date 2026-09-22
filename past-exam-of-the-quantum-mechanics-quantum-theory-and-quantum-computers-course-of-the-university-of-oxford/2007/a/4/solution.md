<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [pure state](../../../../pure-state.md) is a unit vector in a complex [Hilbert space](../../../../hilbert-space-split.md), with vectors differing by a [global phase](../../../../global-phase.md) representing the same physical state. An [observable](../../../../observable.md) is a [self-adjoint operator](../../../../self-adjoint-operator.md), with [measurement](../../../../measurement.md) probabilities determined by its [spectral projections](../../../../spectral-projection.md). For vectors in the relevant [operator domains](../../../../operator-domain.md),

$$
\boxed{E_\psi[A]=\langle\psi,A\psi\rangle,\qquad
\Delta_\psi[A]^2=\langle\psi,A^2\psi\rangle-E_\psi[A]^2
=\|(A-E_\psi[A])\psi\|^2.}
$$

A squared norm vanishes exactly when its vector vanishes. Therefore zero [dispersion](../../../../wave-dispersion.md) is equivalent to $A\psi=E_\psi[A]\psi$.

In the position representation, $(X\psi)(x)=x\psi(x)$ and $(P\psi)(x)=-i\hbar\psi'(x)$. On a common differentiable invariant domain,

$$
(XP-PX)\psi=-i\hbar x\psi'+i\hbar(x\psi)'=i\hbar\psi,
$$

so $\boxed{[X,P]=i\hbar I}$.

For two [observables](../../../../observable.md) set $a=\|A\psi\|^2$, $b=\|B\psi\|^2$, $c=E_\psi[i[A,B]]$. For real $t$,

$$
0\leq\|(A-itB)\psi\|^2=a-ct+bt^2.
$$

If $b>0$, nonpositivity of its discriminant yields $\boxed{4ab\geq c^2}$. Equality holds exactly when the minimum squared norm vanishes, namely

$$
\boxed{A\psi=itB\psi\quad\text{for some real }t,\quad t=c/(2b).}
$$

The degenerate case must also be included: if $B\psi=0$, then $b=c=0$ and equality holds for every $A\psi$. Thus the complete criterion is that $B\psi=0$, or that the displayed real-$t$ relation holds. This includes $A\psi=0$ by choosing $t=0$ when $b>0$.

Apply the inequality to centred operators $A=P-E_\psi[P]I$, $B=X-E_\psi[X]I$. Their squared norms are the [variances](../../../../variance-split.md) and their [commutator](../../../../commutator.md) is $[P,X]=-i\hbar I$, giving

$$
\boxed{\Delta_\psi[P]^2\Delta_\psi[X]^2\geq\frac{\hbar^2}{4}.}
$$

An [eigenvector](../../../../eigenvector.md) of either operator would have its corresponding [dispersion](../../../../wave-dispersion.md) zero, contradicting this positive lower bound if the other [dispersion](../../../../wave-dispersion.md) were finite and the stated domain conditions held. In the usual $L^2(\mathbb R)$ representation there are in fact no [normalizable](../../../../normalizable-wavefunction.md) exact position or momentum [eigenvectors](../../../../eigenvector.md); their generalized [eigenvectors](../../../../eigenvector.md) are not counterexamples. The equality condition above is the [uncentered second-moment commutator inequality](../../../../uncentered-second-moment-commutator-inequality.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
