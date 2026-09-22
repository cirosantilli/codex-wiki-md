<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a normal [half-precision floating-point number](../../../../../half-precision-floating-point-format.md), write the stored fields as sign $s$, biased [exponent](../../../../../exponent.md) $E$ and ten-[bit](../../../../../bit.md) fraction $f$. The value is $(-1)^s(1.f)_2\,2^{E-15}$ for $1\leq E\leq30$. The leading one is implicit: the ten stored fraction [bits](../../../../../bit.md) give eleven significant [binary digits](../../../../../binary-digit.md) including that one. The normalized [binary representations](../../../../../binary-number.md) and stored fields are

| Value | Normalized [binary representation](../../../../../binary-number.md) | Sign, biased [exponent](../../../../../exponent.md), fraction |
| --- | --- | --- |
| $1/2$ | $1.0_2\,2^{-1}$ | `0 01110 0000000000` |
| $5/8$ | $1.01_2\,2^{-1}$ | `0 01110 0100000000` |
| $-3/16$ | $-1.1_2\,2^{-3}$ | `1 01100 1000000000` |
| $15\frac12$ | $1.1111_2\,2^3$ | `0 10010 1111000000` |

Thus the four 16-[bit](../../../../../bit.md) words are

$$
\boxed{0011100000000000,\quad0011100100000000,\quad1011001000000000,\quad0100101111000000.}
$$

Every conversion is exact: all four numbers have terminating [binary representations](../../../../../binary-number.md) within the available precision.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
