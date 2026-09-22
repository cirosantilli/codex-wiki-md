<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the stored [bits](../../../../../bit.md) be $b_{15},\ldots,b_0$ and let $s=b_{15}$. The [sign extension](../../../../../sign-extension.md) performed by `ldrsh` keeps output [bit](../../../../../bit.md) $i$ equal to $b_i$ for $0\le i\le15$, and sets every output [bit](../../../../../bit.md) $16\le i\le31$ to $s$. Thus a nonnegative halfword gets sixteen leading zero [bits](../../../../../bit.md), while a negative halfword gets sixteen leading one [bits](../../../../../bit.md).

Its signed 32-[bit](../../../../../bit.md) [two's complement](../../../../../two-s-complement.md) value is

$$
-s2^{31}+s\sum_{i=16}^{30}2^i+\sum_{i=0}^{15}b_i2^i
=-s2^{16}+s2^{15}+\sum_{i=0}^{14}b_i2^i
=\boxed{-s2^{15}+\sum_{i=0}^{14}b_i2^i}.
$$

The last expression is exactly the original signed 16-[bit](../../../../../bit.md) value. The equality uses the finite [geometric series](../../../../../geometric-series.md) $\sum_{i=16}^{30}2^i=2^{31}-2^{16}$. In particular, simply inserting zero [bits](../../../../../bit.md) would be wrong for a negative halfword: its [unsigned interpretation](../../../../../unsigned-interpretation-of-a-bit-string.md) differs from its signed value by $2^{16}$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
