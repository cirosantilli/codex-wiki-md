<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the convention **$a_{\mathrm{new}}[j]=A[p[j]]$**, as required by the paper's rotation example. Follow each [permutation cycle](../../../../../permutation-cycle.md) once. Temporarily encode a visited value $v\in[0,N)$ as $-v-1$, and restore the whole permutation before returning:
```
PROCEDURE Permute(VAR p: ARRAY OF INTEGER);
VAR s, j, next: INTEGER; saved: T;
BEGIN
  s := 0;
  WHILE s < N DO
    IF p[s] >= 0 THEN
      IF p[s] = s THEN
        p[s] := -p[s]-1
      ELSE
        saved := a[s]; j := s;
        next := p[j]; p[j] := -next-1;
        WHILE next # s DO
          a[j] := a[next]; j := next;
          next := p[j]; p[j] := -next-1
        END;
        a[j] := saved
      END
    END;
    s := s+1
  END;
  s := 0;
  WHILE s < N DO p[s] := -p[s]-1; s := s+1 END
END Permute;
```
Require `LEN(p) >= N` and that `p[0..N)` is the stipulated [permutation](../../../../../permutation.md). Its cells must be writable and distinct from the data [array](../../../../../array-data-structure.md). The marking map is reversible and fits whenever the original valid indices and $N$ fit in the signed [integer](../../../../../integer-split.md) type.

At each outer test, all marked indices belong to fully completed cycles; all unmarked cycles still contain their original data and permutation entries. Within a cycle the same shifting [loop invariant](../../../../../loop-invariant.md) as part (d) applies, with successor given by the original `p`: all previously filled positions have their final values, and `saved` preserves the overwritten first source. A [permutation](../../../../../permutation.md) has no path into a different cycle, so every new successor is unmarked until it returns to `s`; no encoded negative value is used as a source index. At outer-loop exit every index is marked and correct. The restoration loop has decoded precisely the indices below `s`.

**The procedure uses one extra value of type `T`, $O(N)$ time, and at most $N$ data reads plus $N$ data writes**, with no data access for fixed points. It returns `p` unchanged, though it marks it temporarily. If `p` must remain read-only even during execution, test whether each index is its cycle's smallest member by traversing `p` before moving that cycle. That preserves constant space and the same optimal data accesses, but can require $O(N^2)$ index-array accesses.

## ↑ Ancestors (12)

1. [E](../e.md)
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
