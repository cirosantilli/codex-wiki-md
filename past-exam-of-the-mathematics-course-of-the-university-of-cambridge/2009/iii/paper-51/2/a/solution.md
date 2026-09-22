<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $N=|A|$. For $N>1$, the unmarked [computational basis](../../../../../../computational-basis.md) vectors in $A$ give the normalized vector

$$
\boxed{|\omega\rangle=\frac1{\sqrt{N-1}}\sum_{x\in A\setminus\{a\}}|x\rangle
=\frac{\sqrt N|\psi_A\rangle-|a\rangle}{\sqrt{N-1}}.}
$$

Its norm is one and $\langle a|\omega\rangle=0$, so these two vectors form an [orthonormal basis](../../../../../../orthonormal-basis.md) for $\mathcal V$. Splitting the [uniform superposition state](../../../../../../uniform-superposition-state.md) into its marked and unmarked terms gives

$$
|\psi_A\rangle=\frac1{\sqrt N}|a\rangle+\sqrt{\frac{N-1}{N}}|\omega\rangle,
\qquad\boxed{\theta=\arcsin\frac1{\sqrt N}.}
$$

The nonnegative coefficients select the specified angle in $[0,\pi/2]$.

There is one degenerate boundary case: if $N=1$, then $|\psi_A\rangle=|a\rangle$ and $\mathcal V$ is one-dimensional. No vector in $\mathcal V$ can complete $|a\rangle$ to a two-element [orthonormal basis](../../../../../../orthonormal-basis.md). Thus the printed two-dimensional description needs $N>1$. For $N=1$ the search itself is already solved, with $\theta=\pi/2$ and no query.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
