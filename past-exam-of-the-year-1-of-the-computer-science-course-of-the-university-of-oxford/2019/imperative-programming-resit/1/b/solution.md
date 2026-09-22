<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a positive remaining [fraction](../../../../../fraction.md) $n/d$, the condition $1/q\leq n/d$ is equivalent to $q\geq d/n$. Since $1/q$ decreases as the positive [integer](../../../../../integer-split.md) $q$ increases, **choose $q=\lceil d/n\rceil$**. The zero [fraction](../../../../../fraction.md) needs no term. This is the [greedy Egyptian fraction expansion](../../../../../greedy-egyptian-fraction-expansion.md).

The remaining [fraction](../../../../../fraction.md) is

$$
\frac nd-\frac1q=\frac{nq-d}{dq}.
$$

The defining inequalities $q-1<d/n\leq q$ give $0\leq nq-d<n$. Therefore the unreduced new numerator is a nonnegative [integer](../../../../../integer-split.md) strictly smaller than the old positive numerator. Passing to a [reduced fraction](../../../../../reduced-fraction.md) can only reduce it further. That numerator is a [loop variant](../../../../../loop-variant.md), so the process terminates. The increasing denominators are not the termination argument; their size need not be bounded in advance.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
