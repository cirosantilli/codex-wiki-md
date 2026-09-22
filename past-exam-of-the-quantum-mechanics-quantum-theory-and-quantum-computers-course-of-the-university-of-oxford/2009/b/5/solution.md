<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a nonzero trial vector use the [Rayleigh quotient](../../../../rayleigh-quotient.md) $\mathcal E(\psi)=\langle\psi,H\psi\rangle/\langle\psi,\psi\rangle$. Its first variation in any allowed direction $\eta$ is

$$
\delta\mathcal E=\frac{2\operatorname{Re}\langle\eta,(H-\mathcal E)\psi\rangle}{\|\psi\|^2}.
$$

Vanishing for all complex directions implies $(H-\mathcal E)\psi=0$; an [eigenvector](../../../../eigenvector.md) conversely makes it vanish. The ground [energy](../../../../energy-split.md) is the infimum of this quotient for a lower-bounded [Hamiltonian](../../../../hamiltonian.md), so minimizing over a trial family provides an upper bound to it, exact when that family contains a ground [eigenvector](../../../../eigenvector.md).

Set $a=\langle\phi,H\phi\rangle$, $b=\langle\phi,I\phi\rangle$ and $c=\langle\phi,HI\phi\rangle$. All three are real: $H,I$ are [self-adjoint](../../../../self-adjoint-operator.md) and commute. Also $I^\dagger I=I^2=1$. Expansion of the numerator and norm gives

$$
\boxed{\mathcal E(t)=\frac{(1+t^2)a+2tc}{1+t^2+2tb}.}
$$

Differentiate the quotient, retaining only nonzero trial vectors:

$$
\mathcal E'(t)=\frac{2(c-ab)(1-t^2)}{(1+t^2+2tb)^2}.
$$

Thus the stationarity equation is $\boxed{(t^2-1)(c-ab)=0}$. If $c=ab$, the quotient is identically $a$ wherever defined. Otherwise $t=\pm1$ are the two extrema, with

$$
\boxed{\mathcal E_\pm=\frac{a\pm c}{1\pm b},\qquad \mathcal E_+-\mathcal E_-=\frac{2(c-ab)}{1-b^2}.}
$$

In this nonconstant case $|b|<1$, so both denominators are positive. If $c-ab>0$, the plus value is the maximum and the minus value the minimum; the assignments reverse when $c-ab<0$. One can also see global extremality by resolving the trial vector into the orthogonal $I=\pm1$ sectors: its [energy](../../../../energy-split.md) is a weighted mean of their two fixed projected energies.

The null-vector exception matters. If $|b|=1$, then $I\phi=\pm\phi$, the covariance $c-ab$ vanishes and one of $\phi\pm I\phi$ is zero. That value has no [Rayleigh quotient](../../../../rayleigh-quotient.md) and is not an extra stationary physical state.

For particle exchange, change of integration variables shows that $I\phi(x_1,x_2)=\phi(x_2,x_1)$ is [unitary](../../../../unitary-connection.md) and $I^2=1$, hence [self-adjoint](../../../../self-adjoint-operator.md). Exchanging coordinates interchanges the two kinetic derivatives and leaves the symmetric potential unchanged, so $[I,H]=0$. The vectors $\phi\pm I\phi$ lie in its symmetric and antisymmetric sectors. Their normalized nonzero versions are respectively [bosonic](../../../../boson.md) and [fermionic](../../../../fermion.md) spatial trial [wavefunctions](../../../../wave-function-split.md).

Because the [energy](../../../../energy-split.md) of a general trial state is the weighted average of its sector energies, at least one nonzero symmetry [projection](../../../../projection-linear-algebra.md) has [energy](../../../../energy-split.md) no greater than the original trial. Thus minimizing can be performed in a definite exchange-symmetry sector. This is a variational approximation within the trial subspace; it does not assert that projecting an arbitrary trial vector produces an exact [eigenvector](../../../../eigenvector.md) of $H$. For particles with a prescribed statistics sector one minimizes within that physical sector.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
