<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the standard coordinate generators of $\mathbb Z^d$. Its [word metric](../../../../../../word-metric.md) is the $\ell^1$ metric, so its radius-$r$ ball consists of integer points satisfying $\sum_i|x_i|\le r$. For $d\ge1$ it contains the cube $|x_i|\le\lfloor r/d\rfloor$ and is contained in the cube $|x_i|\le r$. Thus

$$
(2\lfloor r/d\rfloor+1)^d\le\beta_{\mathbb Z^d}(r)\le(2r+1)^d,
$$

and its growth is bounded above and below by constant multiples of $r^d$ for large $r$.

If $\mathbb Z^n$ and $\mathbb Z^m$ are quasi-isometric, part (i) gives equivalent [growth functions of a finitely generated group](../../../../../../growth-function-of-a-finitely-generated-group.md). For positive $n>m$, the required comparison $r^n\lesssim r^m$ would bound a positive constant times $r^n$ by $O(r^m+r)$, impossible as $r\to\infty$. Interchanging $n,m$ rules out $m>n$. Hence $n=m$. Conversely, for equal dimensions the identity is an isometry with standard generators; changing finite generators preserves [quasi-isometry](../../../../../../quasi-isometry.md) by Q2(ii). Therefore

$$
\boxed{\mathbb Z^n\text{ and }\mathbb Z^m\text{ are quasi-isometric if and only if }n=m.}
$$

If dimension zero is allowed, $\mathbb Z^0$ is bounded and cannot be quasi-isometric to an unbounded positive-dimensional lattice. This boundedness argument is needed because the additive linear term in $\sim_e$ makes constant and linear [growth functions of a finitely generated group](../../../../../../growth-function-of-a-finitely-generated-group.md) equivalent; growth equivalence alone would not distinguish dimensions zero and one.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
