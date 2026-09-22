<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use [merge sort](../../../../../merge-sort.md), stopping before an empty or singleton [linked list](../../../../../linked-list.md) would be split.
```
PROCEDURE MergeSort(less: LESS; VAR p: List);
VAR q, r: List;
BEGIN
  IF p.count > 1 THEN
    Split(p, q, r);
    MergeSort(less, q); MergeSort(less, r);
    Merge(less, q, r, p)
  END
END MergeSort;
```
By [induction](../../../../../mathematical-induction.md) on the length, each recursive call returns a sorted [permutation](../../../../../permutation.md) of its input. Part (d) makes both child lengths smaller than the parent whenever the parent length exceeds one; part (e) combines the sorted children. No data [linked list nodes](../../../../../linked-list-node.md) are newly allocated or lost. Unreachable headers may be reclaimed by [garbage collection](../../../../../garbage-collection.md).

At each level the total splitting and [merge algorithm](../../../../../merge-algorithm.md) work is linear; approximately equal halves give logarithmic depth. Consequently

$$
\boxed{\text{Stable ascending sort in }O(n\log(n+1))\text{ time, with }O(\log(n+1))\text{ call-stack depth}.}
$$

There are $O(n)$ header allocations over the whole execution; those allocations should not be confused with the logarithmic [call stack](../../../../../call-stack.md) bound.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
