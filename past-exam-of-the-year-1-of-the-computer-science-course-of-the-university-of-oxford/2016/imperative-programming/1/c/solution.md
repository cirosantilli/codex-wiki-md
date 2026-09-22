<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The cyclic strict comparisons in the hint identify a head that cannot be the answer:
```
PROCEDURE common3(a, N, b, M, c, L): INTEGER;
VAR i, j, k: INTEGER;
BEGIN
  i := 0; j := 0; k := 0;
  WHILE (a[i] # b[j]) OR (b[j] # c[k]) DO
    IF a[i] < b[j] THEN i := i + 1
    ELSIF b[j] < c[k] THEN j := j + 1
    ELSE k := k + 1
    END
  END;
  RETURN a[i]
END common3;
```
Let $z=a[p]=b[q]=c[r]$ be the smallest common value. The [loop invariant](../../../../../loop-invariant.md) is $0\leq i\leq p<N$, $0\leq j\leq q<M$, $0\leq k\leq r<L$, and every discarded entry is not common to all three [arrays](../../../../../array-data-structure.md). If $a[i]<b[j]$, the entry $a[i]$ cannot occur in the unprocessed part of $b$, so discard it. The branch $b[j]<c[k]$ has the analogous justification. If neither comparison holds but the heads are not all equal, the hint guarantees $c[k]<a[i]$, so discard $c[k]$.

A pointer at its target position cannot be advanced: for example $i=p$ and $a[i]<b[j]$ would imply $z<b[j]\leq z$. Thus all reads stay within [array bounds](../../../../../array-bounds.md). The [loop variant](../../../../../loop-variant.md) $(p-i)+(q-j)+(r-k)$ decreases. At exit all heads equal $z$. **The cost is $O(N+M+L)$ time and $O(1)$ auxiliary space.**

## ↑ Ancestors (12)

1. [C](../c.md)
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
