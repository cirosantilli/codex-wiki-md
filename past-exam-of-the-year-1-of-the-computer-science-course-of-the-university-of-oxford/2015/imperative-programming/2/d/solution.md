<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Implement [staircase matrix search](../../../../../staircase-matrix-search.md) from the top-right corner. In the following [Oberon](../../../../../oberon-programming-language.md)-style code, `&` denotes short-circuit conjunction; all guarded accesses respect [array bounds](../../../../../array-bounds.md).
```
PROCEDURE Staircase(x: INTEGER; VAR i, j: INTEGER): BOOLEAN;
VAR r, c: INTEGER;
BEGIN
  r := 0; c := N-1;
  WHILE (r < M) & (c >= 0) DO
    IF f[r,c] = x THEN i := r; j := c; RETURN TRUE
    ELSIF f[r,c] < x THEN INC(r)
    ELSE DEC(c)
    END
  END;
  RETURN FALSE
END Staircase;
```
The [loop invariant](../../../../../loop-invariant.md) is that every occurrence not yet returned lies in

$$
[r,M)\times[0,c+1).
$$

Initially this is the whole [array](../../../../../array-data-structure.md). If $f[r,c]<x$, every entry of row $r$ in the candidate rectangle is smaller than $x$, so increasing $r$ discards no possible answer. If $f[r,c]>x$, every entry of column $c$ in that rectangle is greater than $x$, so decreasing $c$ is safe. These conclusions follow from [monotonicity](../../../../../monotonic-function.md) even when repeated values occur.

The [loop variant](../../../../../loop-variant.md) $(M-r)+(c+1)$ decreases on every unsuccessful iteration. If a dimension becomes empty, the [loop invariant](../../../../../loop-invariant.md) proves absence. For positive dimensions the path inspects at most $M+N-1$ entries; an initially empty dimension causes no inspection. Thus

$$
\boxed{\text{Time }O(M+N),\qquad\text{auxiliary space }O(1).}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
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
