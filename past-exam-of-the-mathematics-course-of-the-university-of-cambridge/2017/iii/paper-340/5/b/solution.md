<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Computing $P_Cg$ is equivalent to minimizing $F(p)=\tfrac12\|g-D^*p\|_2^2$ over $P_\lambda$, since $D^*p$ ranges over precisely $C$. Differentiating with the [adjoint operator](../../../../../../adjoint-operator.md) gives $\nabla F(p)=D(D^*p-g)$, whose [Lipschitz constant](../../../../../../lipschitz-constant.md) is $L=\|DD^*\|=\|D\|^2$. Starting with any $p^0\in P_\lambda$, for example zero, the [projected-gradient dual total variation algorithm](../../../../../../projected-gradient-dual-total-variation-algorithm.md) is

$$
\boxed{r^k=p^k+\tau D(g-D^*p^k),\qquad p^{k+1}_{i,j}=\frac{r^k_{i,j}}{\max(1,|r^k_{i,j}|_2/\lambda)},\qquad u^k=g-D^*p^k.}
$$

The block formula is the [Euclidean projection onto a convex set](../../../../../../euclidean-projection-onto-a-convex-set.md) $P_\lambda$, since it clips each two-dimensional block to a Euclidean ball of radius $\lambda$. Both components must be clipped together for the isotropic [block mixed norm](../../../../../../block-mixed-norm.md).

For the unscaled forward differences, $\|D_x^+u\|_2^2\le4\|u\|_2^2$ and likewise in the other direction, so $L\le8$. More exactly, for $N>1$ the one-dimensional path difference has [eigenvalues](../../../../../../eigenvalue.md) $4\sin^2(k\pi/(2N))$, $0\le k<N$, and the square-grid operator sums two such spectra. Thus $L=8\cos^2(\pi/(2N))$. Finite-dimensional [projected gradient descent](../../../../../../projected-gradient-descent.md) for a [convex](../../../../../../convex-function.md) objective with an $L$-Lipschitz [gradient](../../../../../../gradient.md) converges from every feasible starting point to a dual minimizer for fixed $0<\tau<2/L$. The theorem assumes a nonempty closed [convex set](../../../../../../convex-set.md), a [convex](../../../../../../convex-function.md) [differentiable](../../../../../../differentiable-function.md) objective with globally Lipschitz [gradient](../../../../../../gradient.md), and a nonempty minimizer set. All hold here: $P_\lambda$ is [compact](../../../../../../compact-space.md) and [convex](../../../../../../convex-function.md), and $F$ is a [continuous](../../../../../../continuous-function.md) [convex](../../../../../../convex-function.md) quadratic. Finite-dimensional convergence is of the full [sequence](../../../../../../sequence.md), rather than only its objective values.

Consequently **any fixed step with $0<\tau<1/4$ is safe on this grid**; the more conservative $0<\tau\le1/8$ is also safe. The dual minimizer need not be unique because $D^*$ has a [null space](../../../../../../kernel-of-a-linear-map.md), but $D^*p^k\to P_Cg$ and $u^k\to u$ uniquely. For $N=1$, the [gradient](../../../../../../gradient.md) penalty vanishes and $u=g$, so no positive-$L$ step restriction is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
