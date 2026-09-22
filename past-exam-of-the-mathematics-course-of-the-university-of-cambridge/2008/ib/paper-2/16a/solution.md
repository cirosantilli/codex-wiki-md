<h1 id="16a/solution">Solution</h1>

↑ **Parent:** [16A](../16a.md)

For a normalized wavefunction, $\langle A\rangle_\psi$ is the statistical mean of measurements of the [quantum observable](../../../../../observable.md) $A$ over identically prepared systems, not necessarily the outcome of one measurement. Assume the state is in the required operator domains and the second moments are finite. Hermiticity gives

$$
0\le\|(A+i\lambda B)\psi\|^2
=\langle A^2\rangle+\lambda^2\langle B^2\rangle+i\lambda\langle[A,B]\rangle.
$$

The commutator expectation is purely imaginary, so $i\langle[A,B]\rangle$ is real. A real quadratic nonnegative for every $\lambda$ has nonpositive discriminant; if its quadratic coefficient vanishes, its linear coefficient must also vanish. Consequently

$$
\boxed{\langle A^2\rangle\langle B^2\rangle\ge\frac14|\langle[A,B]\rangle|^2.}
$$

Apply the same inequality to $A-\langle A\rangle I$ and $B-\langle B\rangle I$. Their commutator is unchanged and their second moments are the variances, yielding the [quantum uncertainty](../../../../../quantum-uncertainty.md) relation

$$
\boxed{\Delta A\,\Delta B\ge\frac12|\langle[A,B]\rangle|.}
$$

For the [harmonic oscillator](../../../../../simple-harmonic-motion.md), $p=-i\hbar\partial_x$ gives $[x,p]\psi=i\hbar\psi$ by the product rule. The uncentered inequality above therefore implies $\langle x^2\rangle\langle p^2\rangle\ge\hbar^2/4$. The [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) now gives

$$
\langle H\rangle=\frac{\langle p^2\rangle}{2m}+\frac{m\omega^2\langle x^2\rangle}{2}
\ge\omega\sqrt{\langle p^2\rangle\langle x^2\rangle}
\ge\boxed{\frac{\hbar\omega}{2}}.
$$

No assumption that the position or momentum means vanish is needed.

## ↑ Ancestors (10)

1. [16A](../16a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
