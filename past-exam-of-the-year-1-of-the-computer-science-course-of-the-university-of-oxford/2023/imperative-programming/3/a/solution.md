<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use an [abstract data type](../../../../../abstract-data-type.md) with two total count [functions](../../../../../function-split.md), $I,O:U\to\{0,\ldots,M\}$, where $U=\{1,\ldots,99999999\}$ and $M=2^{31}-1$. $I(u)$ counts incoming payments and $O(u)$ outgoing payments. Initially **$I(u)=O(u)=0$ for every valid user**. A user without a stored record is therefore observable as two zero counts; no separate registration operation is necessary.

The explicit bound $M$ matches the source's `Int` record fields. Increment operations require space in the relevant count, so no [integer overflow](../../../../../integer-overflow.md) is permitted. An unbounded mathematical counting [abstract data type](../../../../../abstract-data-type.md) would instead require an arbitrary-precision representation or an explicit overflow policy. The large user domain does not require allocating a record for every user: a [sparse map with a default value](../../../../../sparse-map-with-a-default-value.md) can realize these total [functions](../../../../../function-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
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
