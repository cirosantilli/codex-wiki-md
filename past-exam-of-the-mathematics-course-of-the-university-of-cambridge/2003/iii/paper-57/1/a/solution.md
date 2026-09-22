<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $M$ be an oriented smooth $m$-dimensional [manifold with boundary](../../../../../../manifold-with-boundary.md) and $\alpha$ a smooth compactly supported $(m-1)$-[differential form](../../../../../../differential-form-split.md). Give $\partial M$ the outward-normal-first [orientation](../../../../../../orientation-of-a-simplex.md). A [partition of unity](../../../../../../partition-of-unity.md) subordinate to oriented interior and boundary charts reduces the proof to a compactly supported form on $\mathbb R^m$ or on a half-space. Indeed $\alpha=\sum_j\chi_j\alpha$, so $d\alpha=\sum_jd(\chi_j\alpha)$; the sum of terms involving $d\chi_j$ is zero. [Exterior derivative](../../../../../../exterior-derivative.md) commutes with chart [pullbacks](../../../../../../pullback-category-theory.md), so each summand can be calculated in coordinates.

Write the local form as

$$
\alpha=\sum_{j=1}^m(-1)^{j-1}f_j\,dx^1\wedge\cdots\wedge\widehat{dx^j}\wedge\cdots\wedge dx^m,
\qquad d\alpha=\left(\sum_j\partial_jf_j\right)dx^1\wedge\cdots\wedge dx^m.
$$

For an interior chart, integrate each derivative using the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md): its integral is zero because $f_j$ has compact support. For a boundary chart modeled on $x^m\geq0$, all tangential derivatives again integrate to zero, while $\int_0^\infty\partial_mf_m\,dx^m=-f_m(x',0)$. The outward normal is $-\partial_m$; its contraction with the volume form gives exactly this sign in the induced boundary integral of $\alpha$. Summing the chart identities proves the [Generalized Stokes theorem](../../../../../../generalized-stokes-theorem.md):

$$
\boxed{\int_Md\alpha=\int_{\partial M}\alpha.}
$$

Compact support can be replaced by compactness of $M$; on a noncompact [manifold](../../../../../../topological-manifold.md), sufficient support or convergence conditions are necessary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
