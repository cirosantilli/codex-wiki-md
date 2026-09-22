<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write parts in nonincreasing order. The [array](../../../../../array-data-structure.md) `part` stores the current prefix, and `Emit(i,r,len)` completes it using parts at most $i$ with remaining sum $r$. With `Out` as the [Oberon](../../../../../oberon-programming-language.md) output module:
```
VAR part: ARRAY MaxParts OF INTEGER;

PROCEDURE Emit(i, r, len: INTEGER);
VAR j: INTEGER;
BEGIN
  IF r = 0 THEN
    j := 0;
    WHILE j < len DO
      IF j > 0 THEN Out.Char("+") END;
      Out.Int(part[j], 0); j := j+1
    END;
    Out.Ln
  ELSIF i > 0 THEN
    IF i <= r THEN
      part[len] := i;
      Emit(i, r-i, len+1)
    END;
    Emit(i-1, r, len)
  END
END Emit;

PROCEDURE PrintPartitions(n: INTEGER);
BEGIN
  Emit(n, n, 0)
END PrintPartitions;
```
The [recursion invariant](../../../../../recursion-invariant.md) is that `part[0..len)` is nonincreasing, has sum $n-r$, and every further part must be at most $i$ and at most the last existing part. The first branch includes the next part $i$; the second excludes it. These alternatives partition all completions, so each [integer partition](../../../../../integer-partition.md) is printed exactly once. A [recursive call](../../../../../recursive-call.md) reduces $i+r$; the printing loop's [loop invariant](../../../../../loop-invariant.md) is that the first $j$ entries have been printed with exactly the necessary separators.

For $n>0$, no partition has more than $n$ parts, and the all-ones partition has exactly $n$. Thus **the fixed [array](../../../../../array-data-structure.md) requires $0\leq n\leq\texttt{MaxParts}$** to handle every partition. When a write occurs, $r>0$ and therefore `len < n`, so this bound prevents an out-of-range write. Zero prints one empty line, representing the empty [integer partition](../../../../../integer-partition.md). Available [call stack](../../../../../call-stack.md) space imposes a further practical limit.

## ↑ Ancestors (12)

1. [C](../c.md)
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
