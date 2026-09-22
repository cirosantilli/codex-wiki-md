<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

A [well-order](../../../../../well-order.md) is a linearly ordered set in which every nonempty subset has a least element. First note that a [well-order](../../../../../well-order.md) cannot be isomorphic to a proper [initial segment](../../../../../initial-segment.md) of itself: the least element moved by such an isomorphism would have exactly the same predecessor set on each side, forcing it to be fixed. The same least-disagreement argument makes an isomorphism between [initial segments](../../../../../initial-segment.md) unique.

Match $a\in A$ to $b\in B$ exactly when their strict predecessor sets are order-isomorphic. The preceding observation makes each match unique. Matches preserve order and fill [initial segments](../../../../../initial-segment.md) on both sides, since restricting an isomorphism matches every earlier element. If both sides had an unmatched element, take the least unmatched $a$ and $b$. Their predecessor sets would be exactly the already matched segments, so they too would match, a contradiction. Therefore the matching exhausts at least one [well-order](../../../../../well-order.md) and gives an isomorphism of that whole set onto an [initial segment](../../../../../initial-segment.md) of the other. Uniqueness follows from the same predecessor-set argument. The whole set is allowed as an [initial segment](../../../../../initial-segment.md); this includes equal [order types](../../../../../order-type.md).

For [ordinal](../../../../../ordinal.md) division, let $\beta>0$ and choose

$$
\gamma=\sup\{\eta:\beta\eta\leq\alpha\}.
$$

This supremum is a set [ordinal](../../../../../ordinal.md) because $\beta\eta\geq\eta$ bounds the displayed [ordinals](../../../../../ordinal.md) by $\alpha$. Strict increase and [continuity](../../../../../continuous-function.md) of multiplication in the right argument imply $\beta\gamma\leq\alpha<\beta(\gamma+1)$. Take the [order type](../../../../../order-type.md) $\delta$ of the remaining tail of $\alpha$ after its [initial segment](../../../../../initial-segment.md) of type $\beta\gamma$. Then $\alpha=\beta\gamma+\delta$; if $\delta\geq\beta$ it would contradict the strict upper inequality. Thus

$$
\boxed{\alpha=\beta\gamma+\delta,\qquad\delta<\beta.}
$$

The half-open intervals $[\beta\eta,\beta(\eta+1))$ are disjoint, so $\gamma$ is unique, and uniqueness of the tail gives uniqueness of $\delta$. This is left-divisor [ordinal](../../../../../ordinal.md) division: the order of multiplication cannot be interchanged.

Apply it with $\beta=\omega$. The remainder is finite. A nonzero remainder makes $\omega\gamma+\delta$ a successor, while a nonzero $\omega\gamma$ is a limit: for successor $\gamma$ it ends in a full block of type $\omega$, and for limit $\gamma$ it is the supremum of the earlier blocks. Consequently

$$
\boxed{\lambda\ne0\text{ is a limit ordinal}\quad\Longleftrightarrow\quad\lambda=\omega\gamma\text{ for some }\gamma>0.}
$$

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
