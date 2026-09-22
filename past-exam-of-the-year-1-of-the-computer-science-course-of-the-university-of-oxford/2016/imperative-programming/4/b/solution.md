<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Exchange symmetric pairs, stopping before the middle:
```
PROCEDURE reverse(i, n: INTEGER);
VAR t: INTEGER;
BEGIN
  t := 0;
  WHILE t < n DIV 2 DO
    swap(i+t, i+n-1-t);
    t := t + 1
  END
END reverse;
```
Writing $m_0$ for the pre-call [array](../../../../../array-data-structure.md), the [loop invariant](../../../../../loop-invariant.md) says that the first and last `t` positions of the segment already satisfy $m[i+s]=m_0[i+n-1-s]$, all positions between them retain their original values, and positions outside the segment are unchanged. Each [swap](../../../../../swap.md) fixes the next symmetric pair. The [loop variant](../../../../../loop-variant.md) $\lfloor n/2\rfloor-t$ decreases; the two indices are distinct and in bounds whenever the body executes. **Exactly $\lfloor n/2\rfloor$ swaps reverse the segment**, with the odd-length middle element left in place and no accesses for $n\leq1$.

## ↑ Ancestors (12)

1. [B](../b.md)
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
