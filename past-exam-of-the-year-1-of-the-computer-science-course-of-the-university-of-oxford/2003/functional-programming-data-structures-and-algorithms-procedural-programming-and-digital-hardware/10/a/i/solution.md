<h1 id="10/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An $n$-[bit](../../../../../../bit.md) [two's complement](../../../../../../two-s-complement.md) word $b_{n-1}\cdots b_1b_0$ represents the [integer](../../../../../../integer-split.md)

$$
\boxed{x=-b_{n-1}2^{n-1}+\sum_{i=0}^{n-2}b_i2^i,\qquad
-2^{n-1}\leq x\leq2^{n-1}-1.}
$$

The leading [bit](../../../../../../bit.md) has negative weight. Words beginning with zero encode the nonnegative values; words beginning with one encode the negative values. Equivalently, interpret the whole word as unsigned and subtract $2^n$ when its leading [bit](../../../../../../bit.md) is one. For example, the four-bit words `0111`, `1000`, and `1111` encode $7$, $-8$, and $-1$ respectively. The range is asymmetric: the most negative value has no positive counterpart in the same number of [bits](../../../../../../bit.md).

For a nonzero representable magnitude, complementing all [bits](../../../../../../bit.md) and adding one obtains its negative modulo $2^n$. Fixed-width addition can therefore use the same low-order [binary numeral system](../../../../../../binary-numeral-system.md) addition circuitry for signed and unsigned operands; interpreting the result as signed requires detecting [integer overflow](../../../../../../integer-overflow.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [10](../../../10.md)
4. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
