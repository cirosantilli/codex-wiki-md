<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [dynamic programming](../../../../../dynamic-programming.md) in increasing order of the maximum permitted part and then of the remaining sum. Let `Count` be a sufficiently wide [integer](../../../../../integer-split.md) type and let `table` have dimensions `(MaxN+1)` by `(MaxN+1)`:
```
PROCEDURE CountPartitions(n: INTEGER): Count;
VAR i, j: INTEGER;
    table: ARRAY MaxN+1, MaxN+1 OF Count;
BEGIN
  table[0,0] := 1; j := 1;
  WHILE j <= n DO table[0,j] := 0; j := j+1 END;
  i := 1;
  WHILE i <= n DO
    table[i,0] := 1; j := 1;
    WHILE j <= n DO
      table[i,j] := table[i-1,j];
      IF j >= i THEN
        table[i,j] := table[i,j] + table[i,j-i]
      END;
      j := j+1
    END;
    i := i+1
  END;
  RETURN table[n,n]
END CountPartitions;
```
Require $0\leq n\leq\texttt{MaxN}$. The outer [loop invariant](../../../../../loop-invariant.md) says all rows below $i$ equal $p(\cdot,\cdot)$. The inner [loop invariant](../../../../../loop-invariant.md) additionally says entries before column $j$ in the current row are correct. Its dependencies are the previous row and the earlier column $j-i$, so no future entry is read. **Each state is evaluated once, giving $\Theta(n^2)$ arithmetic operations and $\Theta(n^2)$ stored counts.** A [memoization](../../../../../memoization.md) table around part (a)'s recursion is another valid way to share states; its entries need a separate “computed” flag because zero is a legitimate answer. Growing count sizes affect [bit complexity](../../../../../bit-complexity.md) and can cause [integer overflow](../../../../../integer-overflow.md) in a fixed-width `Count`.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
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
