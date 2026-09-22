<h1 id="16f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The inductive definition of [ordinal addition](../../../../../../ordinal-addition.md) is

$$
\alpha+0=\alpha,\qquad
\alpha+(\beta+1)=(\alpha+\beta)+1,\qquad
\alpha+\lambda=\sup_{\beta<\lambda}(\alpha+\beta)
$$

for a [limit ordinal](../../../../../../limit-ordinal.md) $\lambda$.

The synthetic definition takes the [order type](../../../../../../order-type.md) of the [disjoint union](../../../../../../disjoint-union.md) of a copy of $\alpha$ followed by a copy of $\beta$: every point of the first copy precedes every point of the second, and each copy retains its original [total order](../../../../../../total-order.md).

Fix $\alpha$ and use [transfinite induction](../../../../../../transfinite-induction.md) on $\beta$. The synthetic sum with the [empty order](../../../../../../empty-order.md) is $\alpha$. Appending a [greatest element](../../../../../../greatest-element.md) produces the [successor ordinal](../../../../../../successor-ordinal.md) rule. At a [limit ordinal](../../../../../../limit-ordinal.md) $\lambda$, the second copy is the union of its [initial segments](../../../../../../initial-segment.md) of types $\beta<\lambda$, so the whole order has type  
$\sup_{\beta<\lambda}(\alpha+\beta)$. Thus the synthetic operation satisfies the inductive recursion; uniqueness in [transfinite recursion](../../../../../../transfinite-recursion.md) proves the definitions equivalent.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16F](../../16f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
