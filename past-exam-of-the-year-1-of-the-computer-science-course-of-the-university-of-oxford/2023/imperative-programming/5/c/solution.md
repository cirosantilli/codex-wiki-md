<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A sufficient [representation invariant](../../../../../representation-invariant.md) is:

- Both [arrays](../../../../../array-data-structure.md) have length `capacity`, with $capacity>0$ and $0\leq used\leq capacity$.
- The active keys `elements(0 until used)` are pairwise distinct.
- For each active index $k$, `representatives(k)` equals some active key `elements(j)`.
- Every such representative is fixed: if `representatives(k) == elements(j)`, then `representatives(j) == elements(j)`.

The [abstraction function](../../../../../abstraction-function.md) is

$$
rep=\{\,elements(k)\mapsto representatives(k)\mid0\leq k<used\,\}.
$$

The last two conditions ensure each representative is a genuine member of its own block and that the abstract [function](../../../../../function-split.md) is [idempotent function](../../../../../idempotent-function.md). Cells beyond `used` are unconstrained and ignored. When `used == 0`, these conditions hold vacuously and the [abstraction function](../../../../../abstraction-function.md) yields the empty map. This is an explicit-key version of [quick-find](../../../../../quick-find.md), rather than a parent-pointer [disjoint-set forest](../../../../../disjoint-set-forest.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
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
