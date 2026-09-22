<h1 id="18a/solution">Solution</h1>

↑ **Parent:** [18A](../18a.md)

The [expectation value](../../../../../expectation-value.md) of an [observable](../../../../../observable.md) is the mean outcome of repeated measurements on identically prepared systems in the normalized state. For a [self-adjoint](../../../../../self-adjoint-operator.md) $Q$ it is real and equals $\langle\psi,Q\psi\rangle$. Assume the state belongs to the domains needed for the second moments and the commutator below, so all these quantities exist.

For real $\lambda$, positivity of the squared norm gives

$$
0\leq\|(Q+i\lambda P)\psi\|^2=\langle Q^2\rangle+\lambda^2\langle P^2\rangle+i\lambda\langle[Q,P]\rangle.
$$

The commutator expectation is purely imaginary, so this is a real quadratic in $\lambda$. If $\langle P^2\rangle>0$, its minimum is nonnegative exactly when its discriminant is nonpositive. If $\langle P^2\rangle=0$, nonnegativity for all real $\lambda$ forces the linear coefficient to vanish, yielding the same conclusion. Thus

$$
\boxed{\langle Q^2\rangle\langle P^2\rangle\geq\frac14|\langle[Q,P]\rangle|^2.}
$$

Replace the observables by their centred versions $Q-\langle Q\rangle I$, $P-\langle P\rangle I$. Their commutator is unchanged, and their second moments are the [variances](../../../../../variance-split.md) $(\Delta Q)^2,(\Delta P)^2$. Taking square roots gives the [Robertson uncertainty principle](../../../../../robertson-uncertainty-principle.md)

$$
\boxed{\Delta Q\,\Delta P\geq\frac12|\langle[Q,P]\rangle|.}
$$

For the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md), $p=-i\hbar\partial_x$ gives $[x,p]\psi=i\hbar\psi$. The uncentred inequality above consequently gives $\langle x^2\rangle\langle p^2\rangle\geq\hbar^2/4$. The [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) now yields

$$
\langle H\rangle=\frac{\langle p^2\rangle}{2m}+\frac{m\omega^2\langle x^2\rangle}{2}\geq\omega\sqrt{\langle x^2\rangle\langle p^2\rangle}\geq\boxed{\frac12\hbar\omega}.
$$

This is a bound for every normalized state of finite oscillator energy, not just an eigenstate. It is attained by the centred Gaussian ground state, for which $\langle p^2\rangle=m^2\omega^2\langle x^2\rangle$ and the uncertainty product equals $\hbar/2$.

## ↑ Ancestors (10)

1. [18A](../18a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
