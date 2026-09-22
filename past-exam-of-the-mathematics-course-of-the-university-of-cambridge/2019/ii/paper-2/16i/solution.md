<h1 id="16i/solution">Solution</h1>

↑ **Parent:** [16I](../16i.md)

The inductive definition of [ordinal addition](../../../../../ordinal-addition.md) is the [transfinite recursion](../../../../../transfinite-recursion.md)

$$
\alpha+0=\alpha,
\qquad
\alpha+(\beta+1)=(\alpha+\beta)+1,
\qquad
\alpha+\lambda=\sup_{\gamma<\lambda}(\alpha+\gamma)
$$

for every nonzero [limit ordinal](../../../../../limit-ordinal.md) $\lambda$. The synthetic definition takes disjoint [well-orders](../../../../../well-order.md) $A$ and $B$ of order types $\alpha$ and $\beta$, puts every member of $A$ before every member of $B$, and defines $\alpha+\beta$ to be the order type of this ordered sum.

These definitions agree by [transfinite induction](../../../../../transfinite-induction.md) on $\beta$. The empty second order contributes nothing; adjoining a greatest element gives the successor clause; and a limit well-order is the union of all of its proper initial segments, so its ordered sum with $A$ has order type $\sup_{\gamma<\lambda}(\alpha+\gamma)$.

## ↑ Ancestors (10)

1. [16I](../16i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
