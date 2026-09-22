<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Replace the existence-dependent bounds proof with explicit bounds tests. Neither input [array](../../../../../array-data-structure.md) is changed or copied.
```
PROCEDURE commonOrNone(a, N, b, M);
VAR i, j: INTEGER;
BEGIN
  i := 0; j := 0;
  WHILE (i < N) AND (j < M) DO
    IF a[i] = b[j] THEN RETURN Some(a[i])
    ELSIF a[i] < b[j] THEN i := i + 1
    ELSE j := j + 1
    END
  END;
  RETURN None
END commonOrNone;
```
The [loop invariant](../../../../../loop-invariant.md) is $0\leq i\leq N$, $0\leq j\leq M$, and every common value of the original [arrays](../../../../../array-data-structure.md) lies in both remaining suffixes $a[i..N)$ and $b[j..M)$. Equivalently neither discarded prefix contains a common value. Advancing the smaller current value preserves this for the same ordering reason as in part (a).

Both [array bounds](../../../../../array-bounds.md) are checked before any element is read. If the remaining heads are equal, all later entries are larger, so the returned value is the smallest. If either suffix becomes empty, the [loop invariant](../../../../../loop-invariant.md) proves there is no common value. The [loop variant](../../../../../loop-variant.md) $(N-i)+(M-j)$ decreases on each unsuccessful comparison. **The result is `Some(smallest common value)` or `None`, with $O(N+M)$ time and $O(1)$ auxiliary space**, including empty-input cases. A language without short-circuit operators can use nested tests; the guard here itself contains no array reads.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
