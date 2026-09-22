<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With the usual meaning of [totally disconnected skew Young diagram](../../../../../../../totally-disconnected-skew-young-diagram.md), the assertion in the PDF is false. For example, $\lambda=(3)$ and $\mu=(1)$ give two adjacent cells in one row, so the skew shape is connected, but its sole [standard skew Young tableau](../../../../../../../standard-skew-young-tableau.md) affords the [trivial representation](../../../../../../../trivial-representation.md) of $S_2$. The multiplicity is one, not zero. The correct criterion is a [horizontal strip](../../../../../../../horizontal-strip.md):

$$
\boxed{\dim(V^{\lambda/\mu})^{S_k}=\begin{cases}1&\lambda/\mu\text{ is a horizontal strip},\\0&\text{otherwise}.\end{cases}}
$$

If the course uses “totally disconnected” specifically for no repeated column, its terminology must be read as this criterion; it cannot mean disconnected into individual cells.

For necessity, a non-horizontal strip has two vertically adjacent cells. They form a cover in the cell [partial order](../../../../../../../partially-ordered-set.md), and some [linear extension of a partially ordered set](../../../../../../../linear-extension.md) places them consecutively. To justify that assertion, put all predecessors of the lower cell other than the upper cell first, then the upper and lower cells, and complete the order; the cover property prevents any missing intermediate predecessor. The corresponding [standard skew Young tableau](../../../../../../../standard-skew-young-tableau.md) has consecutive entries in one column. The relevant adjacent [transposition](../../../../../../../transposition-permutation.md) acts on its vector by $-1$ in the [Young orthogonal form](../../../../../../../young-orthogonal-form.md). That vector is cyclic, so the [cyclic eigenvector obstruction to invariant vectors](../../../../../../../cyclic-eigenvector-obstruction-to-invariant-vectors.md) excludes invariants.

For sufficiency one can construct an invariant vector explicitly. In a [horizontal strip](../../../../../../../horizontal-strip.md), the occupied column intervals of different rows are disjoint, with every upper interval to the right of every lower interval. Thus an upper-row cell $x$ has content $c(x)$ at least two greater than a lower-row cell $y$ with which it is incomparable. Choose row-reading order as a reference, and for each [standard skew Young tableau](../../../../../../../standard-skew-young-tableau.md) set

$$
b_T=\prod_{\substack{x\text{ precedes }y\text{ in row order}\\T(x)>T(y)}}\sqrt{\frac{c(x)-c(y)+1}{c(x)-c(y)-1}}.
$$

Only pairs in different rows occur in this product; its factors are positive. Put $u=\sum_Tb_Tw_T$. For an admissible swap $R=s_iT$ with $d=c_T(i+1)-c_T(i)$, changing the one inversion in the product gives

$$
\frac{b_R}{b_T}=\frac{1-d^{-1}}{\sqrt{1-d^{-2}}}.
$$

The two-dimensional [Young orthogonal form](../../../../../../../young-orthogonal-form.md) then fixes $b_Tw_T+b_Rw_R$. A nonadmissible swap is within one row and acts by $+1$. Every generator therefore fixes $u\ne0$, proving existence.

Finally an invariant projection of a cyclic vector generates the invariant subspace, because projection identifies all its translates. That subspace has dimension at most one. This proves the exact multiplicity, including the totally disconnected special case, without asserting the incorrect converse in the PDF.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
