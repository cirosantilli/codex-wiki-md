<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

[Equivalence partitioning](../../../../../equivalence-partitioning.md) divides the input domain into classes expected to exercise the same relevant behavior, then chooses representatives and boundary cases from each class. It is a way to select tests, not a proof that every member of a class must behave identically in a faulty implementation.

Useful classes for this parser include [integer](../../../../../integer-split.md)-only inputs, a leading point, a trailing point, and digits on both sides; all-zero inputs and inputs containing ones; leading or trailing zeroes; one-digit and longer blocks; and large [integer](../../../../../integer-split.md) or tiny fractional magnitudes near [floating-point rounding](../../../../../floating-point-rounding.md), [floating-point overflow](../../../../../floating-point-overflow.md) and [floating-point underflow](../../../../../floating-point-underflow.md) boundaries. For instance, compare `'1'`, `'1.'`, `'.1'`, `'1.1'`, `'0001.1000'`, and digit [strings](../../../../../string.md) just beyond the exact [integer](../../../../../integer-split.md) precision of `Double`. Empty digit blocks have the zero convention used above. If a surrounding validator rejects an entirely empty representation or a bare point, test those as separate invalid-format classes. Unexpected digits and multiple points are likewise validator tests, since the conversion fragments assume well-formed input. **Include representatives with independently calculated positional values**, rather than relying only on inverse conversion.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
