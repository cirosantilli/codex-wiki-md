<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

An [invariant subspace](../../../../invariant-subspace.md) $W$ satisfies $D(g)W\subseteq W$ for every $g\in G$; applying the inverse gives equality. The representation is [irreducible](../../../../irreducible-representation.md) when the only invariant subspaces are $0$ and the full space.

The inverse and [conjugate transpose](../../../../conjugate-transpose.md) each reverse multiplication order, so their combination preserves it:

$$
D_2(gh)=[D_1(h^{-1})D_1(g^{-1})]^\dagger=D_1(g^{-1})^\dagger D_1(h^{-1})^\dagger=D_2(g)D_2(h).
$$

Its values are invertible, so this is the [conjugate contragredient representation](../../../../conjugate-contragredient-representation.md).

If $W$ is invariant under $D_2$, take $w\in W$ and $v\in W^\perp$. For the standard [Hermitian inner product](../../../../hermitian-inner-product.md),

$$
\langle w,D_1(g)v\rangle=\langle D_1(g)^\dagger w,v\rangle=\langle D_2(g^{-1})w,v\rangle=0,
$$

since $D_2(g^{-1})w\in W$. Hence $D_1(g)v\in W^\perp$, proving its invariance. If $D_1$ is irreducible, $W^\perp$ is either zero or the whole space; finite-dimensional orthogonal complementation makes $W$ the whole space or zero, respectively. Thus **$D_2$ is irreducible whenever $D_1$ is irreducible**.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2006](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
