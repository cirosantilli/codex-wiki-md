<h1 id="6e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose two [base-p expansions](../../../../../../base-p-expansion.md) represent the same nonnegative [integer](../../../../../../integer.md). Pad the shorter one by trailing zero digits so that both have the same length. Reducing modulo $p$ shows that their first digits satisfy $k_0\equiv k'_0\pmod p$. Since both digits lie between $0$ and $p-1$, they are equal as [integers](../../../../../../integer.md).

Subtract that common digit and divide by $p$. The remaining equality is an equality of two [base-p expansions](../../../../../../base-p-expansion.md) with one fewer digit. Repeating this argument shows that every pair of corresponding digits agrees. Equivalently, repeated [Euclidean division](../../../../../../euclidean-division.md) recovers the digits as remainders. **The digits are unique up to padding by zeroes.** The finite nonnegative-digit representation presupposes $k\ge0$; a negative [integer](../../../../../../integer.md) has no such expansion.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
