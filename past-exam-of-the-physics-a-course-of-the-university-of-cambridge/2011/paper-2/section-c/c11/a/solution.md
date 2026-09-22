<h1 id="section-c/c11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [observables](../../../../../../observable.md) $A,B$, nonzero $[A,B]$ obstructs a complete common [eigenbasis](../../../../../../eigenbasis.md). In a finite-dimensional system, commuting [Hermitian operators](../../../../../../hermitian-operator.md) can be simultaneously diagonalized; [quantum degeneracy](../../../../../../degenerate-energy-levels.md) may require choosing an appropriate basis inside the degenerate [eigenspace](../../../../../../eigenspace.md). Noncommuting [observables](../../../../../../observable.md) can still share particular [eigenvectors](../../../../../../eigenvector.md), so incompatibility is not a claim that every individual state must have nonzero spreads in both quantities.

The [Robertson uncertainty relation](../../../../../../robertson-uncertainty-principle.md) follows by applying [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) to $(A-\langle A\rangle)|\psi\rangle$ and $(B-\langle B\rangle)|\psi\rangle$:

$$
\boxed{\Delta A\,\Delta B\geq\frac12|\langle[A,B]\rangle|}.
$$

In particular $[x,p_x]=i\hbar$ gives $\Delta x\,\Delta p_x\geq\hbar/2$. These are preparation spreads, not necessarily [measurement errors](../../../../../../measurement-error.md). A zero [commutator](../../../../../../commutator.md) expectation can make this bound zero even when the [linear operators](../../../../../../linear-operator.md) do not commute.

Measurement order can matter: preparing $|+z\rangle$, measuring $S_x$, then measuring $S_z$ gives both z outcomes with [probability](../../../../../../probability.md) $1/2$ when the intermediate result is ignored. A direct z measurement would give $+\hbar/2$ certainly. Finally the [Heisenberg equation of motion](../../../../../../heisenberg-equation-of-motion.md) $dA/dt=(i/\hbar)[H,A]+\partial A/\partial t$ relates commutation to conservation: an [observable](../../../../../../observable.md) with no explicit time dependence and $[H,A]=0$ is conserved. For [unbounded self-adjoint operators](../../../../../../unbounded-self-adjoint-operator.md) these statements require the appropriate common domains; a formal commutator calculation alone need not justify simultaneous spectral measurements.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2011](../../../../split.md)
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
