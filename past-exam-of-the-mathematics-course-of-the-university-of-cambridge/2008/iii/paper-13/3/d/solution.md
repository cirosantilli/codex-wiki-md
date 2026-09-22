<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First, multiplication by $w$ maps $W_0^{1,2}$ into $L^2$ by the Hölder and Sobolev estimates just given. Thus a [weak solution](../../../../../../weak-solution.md) $u$ of the perturbed equation has $v=\Delta u=f+wu\in L^2$. Uniqueness for the unperturbed [Dirichlet problem](../../../../../../dirichlet-problem.md) gives $u=Tv$. Its equation becomes

$$
\boxed{(I-K)v=f.}
$$

Conversely, if this equation has a solution $v\in L^2$, then $u=Tv$ belongs to $W_0^{1,2}$ and satisfies $\Delta u=v=f+wTv=f+wu$ weakly. These constructions are inverse to one another.

The [Fredholm alternative for a compact operator](../../../../../../fredholm-alternative.md) states that, on a [Banach space](../../../../../../banach-space-split.md), $I-K$ for compact $K$ is bijective if and only if its kernel is zero; in that case its inverse is bounded. Apply it on $L^2$. Kernels correspond under $T$: a nonzero $v$ with $v=wTv$ gives a nonzero $u=Tv$, since $\Delta Tv=v$; a nonzero homogeneous solution $u$ gives $v=wu$, which cannot be zero because a zero-boundary harmonic [weak solution](../../../../../../weak-solution.md) is zero. Therefore triviality of the homogeneous PDE kernel is equivalent to triviality of $\ker(I-K)$ and hence to unique solvability for every $f\in L^2$. The reverse implication also follows immediately by taking $f=0$. No sign assumption on $w$ is required.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
