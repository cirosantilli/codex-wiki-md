<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the given [sorted array](../../../../../sorted-array.md), the complete [lower-bound search](../../../../../lower-bound-search.md) behavior is $0$ for $x\leq1$, $1$ for $2\leq x\leq4$, $3$ for $5\leq x\leq10$, and $4$ for $x\geq11$. In particular, **index $2$ is never the correct answer** because the two equal entries share the same first insertion position.

These [unit tests](../../../../../unit-testing.md) cover every value boundary, equality case and missing-value interval:

- Below all entries, including the smallest machine [integer](../../../../../integer-split.md): `ternarySearch(a, Int.MinValue) == 0` and `ternarySearch(a, 0) == 0`.
- Equality with the first entry: `ternarySearch(a, 1) == 0`.
- Values in the first gap: `ternarySearch(a, 2) == 1` and `ternarySearch(a, 3) == 1`.
- Repeated equality must return the first duplicate: `ternarySearch(a, 4) == 1`.
- Values in the second gap: `ternarySearch(a, 5) == 3` and `ternarySearch(a, 9) == 3`.
- Equality with the final entry: `ternarySearch(a, 10) == 3`.
- Beyond the final entry: `ternarySearch(a, 11) == 4` and `ternarySearch(a, Int.MaxValue) == 4`.

For every tested target, also assert that the [array](../../../../../array-data-structure.md) is unchanged, the result lies in $[0,4]$, every entry before it is strictly smaller, and every entry from it onward is at least the target. These [postconditions](../../../../../postcondition.md) check the intended partition directly rather than merely accepting any equal occurrence.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
