<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Save the last entry and shift in decreasing index order, so no source is overwritten before being used:
```
PROCEDURE RightOne;
VAR saved: T; i: INTEGER;
BEGIN
  saved := a[N-1]; i := N-1;
  WHILE i > 0 DO
    a[i] := a[i-1]; i := i-1
  END;
  a[0] := saved
END RightOne;
```
The [loop invariant](../../../../../loop-invariant.md) is `saved = A[N-1]`, $a[j]=A[j]$ for $0\leq j\leq i$, and $a[j]=A[j-1]$ for $i<j<N$. The decreasing [loop variant](../../../../../loop-variant.md) is $i$. At exit the untouched saved value fills index zero. **The result is $a[j]=A[(j-1)\bmod N]$**, again with $N$ reads, $N$ writes, and one extra value of type `T`. Applying this after part (b) restores every original entry.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
