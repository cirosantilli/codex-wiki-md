<h1 id="16b/solution">Solution</h1>

↑ **Parent:** [16B](../16b.md)

The [expectation value](../../../../../expectation-value.md) is the mean outcome over many identically prepared measurements of the [observable](../../../../../observable.md). For real $\lambda$, positivity of the [norm](../../../../../norm.md) in the [Hilbert space](../../../../../hilbert-space-split.md) gives

$$
0\leq\|(Q+i\lambda P)\psi\|^2
=\langle Q^2\rangle+\lambda^2\langle P^2\rangle+i\lambda\langle[Q,P]\rangle.
$$

This real quadratic has nonpositive [quadratic discriminant](../../../../../quadratic-discriminant.md), so

$$
\langle Q^2\rangle\langle P^2\rangle\geq\frac14|\langle[Q,P]\rangle|^2.
$$

Apply this to the centered observables $Q-\langle Q\rangle$ and $P-\langle P\rangle$ to obtain the [Robertson uncertainty principle](../../../../../robertson-uncertainty-principle.md)

$$
\boxed{\Delta Q\,\Delta P\geq\frac12|\langle[Q,P]\rangle|.}
$$

For the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md), $[x,p]=i\hbar$ and

$$
E=\frac{\langle p^2\rangle}{2m}+\frac{m\omega^2\langle x^2\rangle}{2}
\geq\frac{(\Delta p)^2}{2m}+\frac{m\omega^2(\Delta x)^2}{2}.
$$

The [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) and $\Delta x\Delta p\geq\hbar/2$ now give

$$
\boxed{E\geq\omega\Delta x\Delta p\geq\frac12\hbar\omega.}
$$

## ↑ Ancestors (10)

1. [16B](../16b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
