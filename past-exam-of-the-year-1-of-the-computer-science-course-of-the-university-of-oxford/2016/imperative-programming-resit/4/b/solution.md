<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $A$ denote the original [array](../../../../../array-data-structure.md), used only in the proof. Save its first entry before overwriting it:
```
PROCEDURE LeftOne;
VAR saved: T; i: INTEGER;
BEGIN
  saved := a[0]; i := 0;
  WHILE i < N-1 DO
    a[i] := a[i+1]; i := i+1
  END;
  a[N-1] := saved
END LeftOne;
```
The [loop invariant](../../../../../loop-invariant.md) is `saved = A[0]`, $a[j]=A[j+1]$ for $0\leq j<i$, and $a[j]=A[j]$ for $i\leq j<N$. Thus the next source is untouched, and the assignment extends the completed prefix. At exit, the saved entry supplies the last position. The [loop variant](../../../../../loop-variant.md) is $N-1-i$. **The result is $a[j]=A[(j+1)\bmod N]$.** This also handles $N=1$, and uses exactly $N$ element reads and $N$ element writes, counting the saved read and final write, with one extra value of type `T`.

## ↑ Ancestors (12)

1. [B](../b.md)
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
