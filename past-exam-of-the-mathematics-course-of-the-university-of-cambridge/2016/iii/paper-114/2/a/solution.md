<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Give the [closed orientable surface](../../../../../../closed-orientable-surface.md) its standard [CW complex](../../../../../../cw-complex.md) structure: one zero-cell, $2g$ one-cells, and one two-cell attached by the product of $g$ commutators. The cellular boundary of the two-cell is zero, since every edge occurs once with each orientation in that word; the one-cell boundaries are also zero. Hence

$$
H^q(\Sigma_g;\mathbb Z)\cong\begin{cases}\mathbb Z,&q=0,2,\\\mathbb Z^{2g},&q=1,\\0,&\text{otherwise}.\end{cases}
$$

Here we use the [cellular homology theorem](../../../../../../cellular-homology-theorem.md), identifying cellular and singular homology, and the [universal coefficient theorem for cohomology](../../../../../../universal-coefficient-theorem-for-cohomology.md): its exact sequence has terms $\operatorname{Ext}(H_{q-1},\mathbb Z)$ and $\operatorname{Hom}(H_q,\mathbb Z)$. All the homology groups here are free, so the Ext terms vanish.

The ring structure comes from [Poincare duality](../../../../../../poincare-duality.md) and [algebraic intersection number of curves on an oriented surface](../../../../../../algebraic-intersection-number-of-curves-on-an-oriented-surface.md). For a closed oriented surface, cap product with its [fundamental class](../../../../../../fundamental-class.md) identifies degree-one [cohomology](../../../../../../cohomology-split.md) with degree-one homology; evaluating the [cup product](../../../../../../cup-product.md) of two such classes equals the signed intersection number of their dual one-cycles. Choose the usual $g$ pairs of handle curves, each pair meeting positively once, and distinct pairs disjoint. Their dual classes can accordingly be named $a_1,b_1,\ldots,a_g,b_g$ so that, for the positive orientation class $\omega$,

$$
\boxed{a_i\smile b_j=\delta_{ij}\omega,\qquad b_j\smile a_i=-\delta_{ij}\omega,\qquad a_i\smile a_j=b_i\smile b_j=0.}
$$

These formulas include squares. More generally, [graded commutativity of the cup product](../../../../../../graded-commutativity-of-the-cup-product.md) kills every degree-one square here because $H^2$ is torsion-free. The unit generates $H^0$, and products involving $\omega$ and any positive-degree class vanish for dimensional reasons. These additive groups and multiplication rules completely describe the [cohomology ring of a closed oriented surface](../../../../../../cohomology-ring-of-a-closed-oriented-surface.md), including $g=0$, when there are no degree-one generators. The intersection pairing is integral and unimodular, rather than merely nondegenerate over a field.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
