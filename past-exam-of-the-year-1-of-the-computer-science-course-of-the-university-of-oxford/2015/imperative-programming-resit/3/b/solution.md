<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a [merge algorithm](../../../../../merge-algorithm.md) with one unread index in each run. Here `u` is the module's [array](../../../../../array-data-structure.md); the destination $[d,d+c-a)$ is disjoint from the source and lies within the [array bounds](../../../../../array-bounds.md):
```
PROCEDURE Merge(a, b, c, d: INTEGER);
VAR i, j, k: INTEGER;
BEGIN
  i := a; j := b; k := d;
  WHILE (i < b) & (j < c) DO
    IF u[i] <= u[j] THEN
      u[k] := u[i]; i := i+1
    ELSE
      u[k] := u[j]; j := j+1
    END;
    k := k+1
  END;
  WHILE i < b DO
    u[k] := u[i]; i := i+1; k := k+1
  END;
  WHILE j < c DO
    u[k] := u[j]; j := j+1; k := k+1
  END
END Merge;
```
Let $A,B$ denote the original two runs. The first [loop invariant](../../../../../loop-invariant.md) says $k-d=(i-a)+(j-b)$ and $u[d..k)$ is the sorted merge of $A[0..i-a)$ and $B[0..j-b)$; moreover each emitted value is at most every unread value. Choosing the smaller head preserves that condition. Equal heads are taken from the first run, giving [stable sorting](../../../../../stable-sorting.md) within this merge. The [loop variant](../../../../../loop-variant.md) is $(b-i)+(c-j)$.

For each copying loop, the output remains the sorted merge of the consumed prefixes, at least one source run is exhausted, and only the indicated suffix remains. The respective [loop variants](../../../../../loop-variant.md) are $b-i$ and $c-j$. At exit both source runs are exhausted:

$$
\boxed{u[d..d+c-a)=\operatorname{merge}(A,B),\qquad T=\Theta(c-a+1).}
$$

The destination's [multiset](../../../../../multiset.md) is the sum of the two source [multisets](../../../../../multiset.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
