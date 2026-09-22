<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume every indicated segment lies within [array bounds](../../../../../array-bounds.md), and lengths are nonnegative. Use a temporary value of element type `T`:
```
PROCEDURE swap(i, j: INTEGER);
VAR x: T;
BEGIN
  x := m[i]; m[i] := m[j]; m[j] := x
END swap;

PROCEDURE blockswap(i, j, n: INTEGER);
VAR t: INTEGER;
BEGIN
  t := 0;
  WHILE t < n DO
    swap(i+t, j+t);
    t := t + 1
  END
END blockswap;
```
The first procedure even works for $i=j$. For the second, disjointness ensures that each [swap](../../../../../swap.md) exchanges the two original entries at offset `t` without disturbing any other pair. Its [loop invariant](../../../../../loop-invariant.md) says that offsets below `t` have been exchanged, offsets from `t` through $n-1$ retain their original values, and everything outside the two segments is unchanged. The [loop variant](../../../../../loop-variant.md) $n-t$ proves [algorithm termination](../../../../../algorithm-termination.md). **A block exchange uses $n$ swaps and $O(1)$ auxiliary space.** The stray `wp` printed after this source subpart is not an additional requirement.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
