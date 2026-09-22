<h1 id="16f/solution">Solution</h1>

↑ **Parent:** [16F](../16f.md)

The inductive definition of [ordinal addition](../../../../../ordinal-addition.md) is

$$
\alpha+0=\alpha,\qquad\alpha+(\beta+1)=(\alpha+\beta)+1,
\qquad\alpha+\lambda=\sup_{\beta<\lambda}(\alpha+\beta)
$$

for nonzero limit [ordinals](../../../../../ordinal.md) $\lambda$. The synthetic definition is the [order type](../../../../../order-type.md) of a disjoint copy of $\alpha$ followed by a disjoint copy of $\beta$, retaining the order within each block and declaring every element of the first block smaller than every element of the second.

These are equivalent by [transfinite induction](../../../../../transfinite-induction.md) in the second argument. An empty second block leaves $\alpha$; a successor block appends one final point; and a limit block is the increasing union of its proper initial blocks, whose order types have the indicated [supremum](../../../../../supremum.md). Thus the synthetic construction satisfies exactly the inductive recursion, which determines the operation uniquely. It is not commutative: **$1+\omega=\omega$, whereas $\omega+1>\omega$**.

## ↑ Ancestors (10)

1. [16F](../16f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
