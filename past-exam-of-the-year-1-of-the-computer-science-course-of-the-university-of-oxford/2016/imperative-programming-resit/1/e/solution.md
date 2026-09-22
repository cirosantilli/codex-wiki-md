<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $M$ be the maximum positive machine [integer](../../../../../integer-split.md). A positive product $xy$ suffers [integer overflow](../../../../../integer-overflow.md) when $x>M\mathbin{\mathrm{DIV}}y$. The vulnerable expressions are `p*b` in part (b), `b2[top]*b2[top]` in the table guard, and `p*b2[k]` in the descending search. Even a rejected candidate must be evaluated before its comparison with $n$.

The table guard becomes dangerous as soon as its current entry exceeds $\sqrt M$: approximately $46340$ for signed 32-bit [integers](../../../../../integer-split.md), or $3.04\times10^9$ for signed 64-bit [integers](../../../../../integer-split.md). These are thresholds for the intermediate power, not for $n$ alone. For example, with 32-bit arithmetic, $b=2$ and $n=65536$ reach the stored power $65536$ and then try its overflowing square $2^{32}$. If $b>46340$, even the initial square may overflow for a tiny $n$. In part (b), the final test can overflow when the next power above $n$ exceeds $M$; at $b=2$, this already happens for $n\geq2^{30}$.

For positive operands, [integer division](../../../../../integer-division.md) gives the exact equivalence $xy\leq n\iff x\leq n\mathbin{\mathrm{DIV}}y$. Therefore replace the three guards respectively by
```
p <= n DIV b
b2[top] <= n DIV b2[top]
p <= n DIV b2[k]
```
and perform each multiplication only after its guard succeeds. Every accepted product is then at most $n\leq M$. **With these guarded products and sufficient table capacity, the algorithms work throughout $2\leq b\leq M$, $1\leq n\leq M$.** The stored exponents and weights also fit in those machine ranges. Checking for overflow after multiplying would be too late.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
