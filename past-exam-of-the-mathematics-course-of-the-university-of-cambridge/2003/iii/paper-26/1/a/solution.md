<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The standard [CW complex](../../../../../../cw-complex.md) structure on [Complex projective space](../../../../../../complex-projective-space.md) $\mathbb{CP}^3$ has one cell in each dimension $0,2,4,6$ and no other cells. Its [cellular chain complex](../../../../../../cellular-chain-complex.md) therefore has zero differentials: each boundary has an odd-dimensional target group, which is zero. The product of the usual two-cell structures on $S^2$ and $S^4$ likewise has exactly one cell in dimensions $0,2,4,6$. Thus [cellular homology](../../../../../../cellular-chain-complex.md) gives, for both spaces,

$$
\boxed{H_i(-;\mathbb Z)\cong\begin{cases}\mathbb Z,&i=0,2,4,6,\\0,&\text{otherwise}.\end{cases}}
$$

The [cohomology rings](../../../../../../cohomology-ring.md) detect more than these additive groups. Let $c\in H^2(\mathbb{CP}^3;\mathbb Z)$ be the hyperplane class. The [cohomology ring of complex projective space](../../../../../../cohomology-ring-of-complex-projective-space.md) is

$$
H^*(\mathbb{CP}^3;\mathbb Z)=\mathbb Z[c]/(c^4),\qquad |c|=2.
$$

For the normalization, a hyperplane is [Poincare dual](../../../../../../poincare-dual.md) to $c$; intersecting three generic hyperplanes gives one point with positive complex [orientation](../../../../../../orientation-of-a-simplex.md), so $\langle c^3,[\mathbb{CP}^3]\rangle=1$. Together with the computed additive groups this makes $c,c^2,c^3$ generators in their respective degrees.

Let $u$ and $v$ be the pullbacks of the [orientation](../../../../../../orientation-of-a-simplex.md) classes of $S^2$ and $S^4$. The [Künneth theorem](../../../../../../kunneth-theorem.md) and naturality of the [cup product](../../../../../../cup-product.md) give

$$
H^*(S^2\times S^4;\mathbb Z)=\mathbb Z[u,v]/(u^2,v^2),\qquad |u|=2,\quad |v|=4,
$$

where $uv$ generates degree six. In particular, every degree-two class on the product has square zero, whereas $c^2\ne0$. Any graded ring isomorphism would send $c$ to $\pm u$, contradicting this product relation. A [homotopy equivalence](../../../../../../homotopy-equivalence.md) induces an isomorphism of [cohomology rings](../../../../../../cohomology-ring.md), so **the spaces have isomorphic integral [homology](../../../../../../homology-split.md) but are not [homotopy](../../../../../../homotopy.md) equivalent**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
