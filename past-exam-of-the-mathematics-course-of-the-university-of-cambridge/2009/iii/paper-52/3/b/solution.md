<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Subtract a [steady state](../../../../../../steady-state.md) to obtain $e(t)=s(t)-s_*$ with $\dot e=Ae$, hence $e(t)=e^{At}e(0)$. The [steady state](../../../../../../steady-state.md) attracts every initial condition exactly when

$$
\boxed{\operatorname{Re}\mu<0\quad\text{for every eigenvalue }\mu\text{ of }A.}
$$

In other words, $A$ must be a [Hurwitz stable matrix](../../../../../../hurwitz-stable-matrix.md). To see sufficiency without assuming diagonalizability, each block in its [Jordan normal form](../../../../../../jordan-normal-form.md) contributes terms of the form $t^k e^{\mu t}$ with finite $k$. Negative real part makes every such term tend to zero, so the whole [matrix exponential](../../../../../../matrix-exponential.md) tends to zero.

For necessity, an eigenmode with positive real part grows, and a mode with zero real part persists or oscillates instead of decaying. For a complex [eigenvalue](../../../../../../eigenvalue.md) of a real matrix, take the real and imaginary parts of its eigenvector to obtain real nondecaying solutions. Thus any [eigenvalue](../../../../../../eigenvalue.md) in the closed right half-plane prevents convergence of all deviations. Physical [density operators](../../../../../../density-matrix.md) span the trace-one affine space, so convergence from all physical initial states also forces decay on every traceless direction.

This gives global [asymptotic stability](../../../../../../asymptotic-stability.md) for the affine linear system and uniqueness of its [steady state](../../../../../../steady-state.md). A merely negative-semidefinite symmetric part proves only nonincrease of a particular norm, not this necessary-and-sufficient condition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
