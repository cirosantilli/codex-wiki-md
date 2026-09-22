<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Represent the two recursively split [arrays](../../../../../array-data-structure.md) by adjacent half-open ranges of the original [array](../../../../../array-data-structure.md). This avoids allocating a fresh pair at every call. The caller supplies a distinct work [array](../../../../../array-data-structure.md) with at least as many elements as `a`; only that work [array](../../../../../array-data-structure.md) is used for merging. The [Oberon](../../../../../oberon-programming-language.md) code is

```
PROCEDURE SortRange(VAR a, work: ARRAY OF INTEGER;
                    l, r: INTEGER);
  VAR m, i, j, k: INTEGER;
BEGIN
  IF r-l > 1 THEN
    m := l + (r-l) DIV 2;
    SortRange(a, work, l, m);
    SortRange(a, work, m, r);
    i := l; j := m; k := l;
    WHILE (i < m) & (j < r) DO
      IF a[i] <= a[j] THEN
        work[k] := a[i]; i := i+1
      ELSE
        work[k] := a[j]; j := j+1
      END;
      k := k+1
    END;
    WHILE i < m DO
      work[k] := a[i]; i := i+1; k := k+1
    END;
    WHILE j < r DO
      work[k] := a[j]; j := j+1; k := k+1
    END;
    k := l;
    WHILE k < r DO
      a[k] := work[k]; k := k+1
    END
  END
END SortRange;

PROCEDURE MergeSort(VAR a, work: ARRAY OF INTEGER);
BEGIN
  SortRange(a, work, 0, LEN(a))
END MergeSort;
```

For a range of length $n>1$, the left length is $p=\lfloor n/2\rfloor$ and the right length is $q=\lceil n/2\rceil$, so $p\leq q\leq p+1$ as required. Both are positive and smaller than $n$, giving the recursive [loop variant](../../../../../loop-variant.md) analogue $r-l$ for [algorithm termination](../../../../../algorithm-termination.md). Empty ranges are also harmless, although the question supplies a nonempty [array](../../../../../array-data-structure.md).

For the first merge loop, regard the two sorted ranges as fixed input sequences $B=a[l:m)$ and $C=a[m:r)$. They are not overwritten during the merge. A [loop invariant](../../../../../loop-invariant.md) is that $l\leq i\leq m$, $m\leq j\leq r$, $k-l=(i-l)+(j-m)$, and `work[l:k)` is the stable sorted merge of the consumed prefixes `a[l:i)` and `a[m:j)`. Every emitted element is at most every remaining element. Taking the smaller head preserves this property, and choosing the left head on equality preserves [stable sorting](../../../../../stable-sorting.md). The [loop variant](../../../../../loop-variant.md) is

$$
(m-i)+(r-j)=r-k.
$$

It is nonnegative and decreases by one per iteration. On exit at least one range is exhausted.

For the second loop, the remaining left range is already sorted and any right remainder is absent whenever that loop runs. Appending the next left element preserves the same merge [loop invariant](../../../../../loop-invariant.md); its [loop variant](../../../../../loop-variant.md) is $m-i$. For the third loop, the left range is exhausted and the right remainder is appended in order; its [loop variant](../../../../../loop-variant.md) is $r-j$. On completing both loops, `work[l:r)` is the complete sorted merge and $k=r$.

In the final copying loop, the [loop invariant](../../../../../loop-invariant.md) is that `a[l:k)` equals `work[l:k)`, `work[l:r)` remains the correct sorted answer, and positions outside `a[l:r)` are unchanged. Its [loop variant](../../../../../loop-variant.md) is $r-k$. At exit the whole answer has been copied back. By [strong induction](../../../../../strong-induction.md) on range length, the recursive calls sort their halves, and the merge preserves the original [multiset](../../../../../multiset.md). Thus

$$
\boxed{\texttt{MergeSort}\text{ returns a sorted permutation of its input}.}
$$

The work [array](../../../../../array-data-structure.md) must not alias `a`: overwriting the source while merging would invalidate the merge [loop invariant](../../../../../loop-invariant.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
