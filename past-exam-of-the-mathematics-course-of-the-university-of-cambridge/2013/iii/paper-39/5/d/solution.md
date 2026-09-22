<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Each floating payment in the [interest rate swap](../../../../../../interest-rate-swap.md) has initial value $P_0(t-1)-P_0(t)$ by the previous replication. Their sum telescopes to $1-P_0(T)$. The fixed leg pays $s$ at each of the same dates, so its initial value is $s\sum_{t=1}^T P_0(t)$. Consequently the [par swap rate](../../../../../../par-swap-rate.md) is

$$
\boxed{s=\frac{1-P_0(T)}{\sum_{t=1}^T P_0(t)}.}
$$

The denominator is positive. This is for unit accrual periods and the printed floating-minus-fixed payments. No extra exchange of principal occurs in the contract; the principal-like terms appear only because the floating-leg replication telescopes.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
