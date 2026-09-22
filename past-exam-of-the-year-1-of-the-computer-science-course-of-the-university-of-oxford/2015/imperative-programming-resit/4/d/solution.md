<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Store the current [multiset](../../../../../multiset.md) in an unsorted prefix `a[0..len)`; `Add` appends exactly as in part (a). The [coupling invariant](../../../../../coupling-invariant.md) is equality of length and [multiset](../../../../../multiset.md) with abstract `xs`, rather than equality of insertion order. `Get` applies [quickselect](../../../../../quickselect.md):
```
PROCEDURE Get(k: INTEGER): INTEGER;
VAR l, r, m: INTEGER;
BEGIN
  ASSERT((0 <= k) & (k < len));
  l := 0; r := len;
  LOOP
    m := Partition(l, r);
    IF k = m THEN RETURN a[m]
    ELSIF k < m THEN r := m
    ELSE l := m+1
    END
  END
END Get;
```
The [loop invariant](../../../../../loop-invariant.md) is $0\leq l\leq k<r\leq\mathrm{len}$, the complete [array](../../../../../array-data-structure.md) has its original [multiset](../../../../../multiset.md), every discarded entry on the left is at most every active entry, and every active entry is at most every discarded entry on the right. Thus the desired global [order statistic](../../../../../order-statistic.md) is the local one of rank $k-l$. The [two-way array partition](../../../../../two-way-array-partition.md) result either identifies it or excludes the pivot and the irrelevant side. The positive [loop variant](../../../../../loop-variant.md) $r-l$ strictly decreases unless the procedure returns.

Balanced pivots give $T(n)\leq T(\lceil n/2\rceil)+cn$, whose [geometric series](../../../../../geometric-series.md) is $O(n)$. More generally, choosing a uniformly random pivot before each call, by swapping a random active entry into `a[r-1]`, gives expected $\Theta(n)$ [running time](../../../../../running-time.md) on distinct keys: with constant [probability](../../../../../probability.md), the pivot is in the middle half and the retained side has size at most $3n/4$. Expected work over these shrinking stages is a convergent [geometric series](../../../../../geometric-series.md).

$$
\boxed{\operatorname{add}:\Theta(1);\quad\operatorname{get}:\text{expected }\Theta(n)\text{ under suitable pivot assumptions, worst-case }\Theta(n^2).}
$$

The particular last-entry pivot in the displayed code has no unconditional expected guarantee without an input distribution. Its worst case repeatedly discards one entry. Duplicate keys require further care: on an all-equal segment, the strict partition always returns $l$, so selecting the last rank costs $n+(n-1)+\cdots+1=\Theta(n^2)$ even with randomized pivot positions. A [three-way array partitioning](../../../../../three-way-array-partitioning.md) that groups all keys equal to the pivot restores the usual randomized linear expectation with duplicates; alternatively the stated expectation assumes distinct keys. This is a qualification to the bound, not to the [algorithm correctness](../../../../../algorithm-correctness.md) of the displayed code.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
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
