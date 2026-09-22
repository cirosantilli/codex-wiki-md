<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [logical right shift](../../../../../logical-right-shift.md) by $k$ moves $a_{i+k}$ into position $i$ and fills the high positions with zero. Its [unsigned interpretation](../../../../../unsigned-interpretation-of-a-bit-string.md) is

$$
\operatorname{bin}(A\mathbin{\mathrm{LSR}}k)=\sum_{i=k}^{n-1}a_i2^{i-k}=:q.
$$

Meanwhile the original [unsigned interpretation](../../../../../unsigned-interpretation-of-a-bit-string.md) decomposes as

$$
a=2^kq+\underbrace{\sum_{i=0}^{k-1}a_i2^i}_{r},\qquad 0\leq r\leq2^k-1.
$$

By [integer division](../../../../../integer-division.md), **$q=\lfloor a/2^k\rfloor$**, exactly the unsigned quotient. Thus the source instruction puts the required quotient into `r1`. This is a proof from [binary representation](../../../../../binary-number.md), rather than an assumption that every kind of right shift implements every kind of division. The displayed [bit](../../../../../bit.md) argument applies to $0\leq k\leq n$, with endpoint operations implemented as a copy or zero where appropriate.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [Digital systems](../../digital-systems.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
