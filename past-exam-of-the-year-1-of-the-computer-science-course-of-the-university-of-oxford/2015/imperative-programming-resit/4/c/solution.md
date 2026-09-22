<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The original page permits $m=r$, but also indexes $a[m]$. The meaningful pivot-position contract is the stronger $l\leq m<r$, with $a[l..m)<a[m]$ and $a[m..r)\geq a[m]$. Implement this [two-way array partition](../../../../../two-way-array-partition.md) by reserving the last entry as pivot:
```
PROCEDURE Partition(l, r: INTEGER): INTEGER;
VAR pivot, i, j, tmp: INTEGER;
BEGIN
  ASSERT(l < r);
  pivot := a[r-1];
  i := l; j := l;
  WHILE j < r-1 DO
    IF a[j] < pivot THEN
      tmp := a[i]; a[i] := a[j]; a[j] := tmp;
      i := i+1
    END;
    j := j+1
  END;
  tmp := a[i]; a[i] := a[r-1]; a[r-1] := tmp;
  RETURN i
END Partition;
```
The [loop invariant](../../../../../loop-invariant.md) is

$$
l\leq i\leq j\leq r-1,\qquad
a[l..i)<\mathrm{pivot},\qquad a[i..j)\geq\mathrm{pivot},\qquad a[r-1]=\mathrm{pivot}.
$$

The segment's [multiset](../../../../../multiset.md) is preserved and entries outside $[l,r)$ are unchanged. The unclassified part is $[j,r-1)$. A smaller entry is swapped into the left group; if $i<j$, the displaced entry belongs to the greater-or-equal group. Otherwise the entry simply joins that group. The [loop variant](../../../../../loop-variant.md) is $r-1-j$.

At exit the final [swap](../../../../../swap.md) installs the pivot at `i`, giving

$$
\boxed{m=i\in[l,r),\quad a[l..m)<a[m]\leq a[m..r),\quad T=\Theta(r-l).}
$$

A singleton segment is handled without loop iterations. Equality belongs on the pivot's right side, as required by the printed strict left inequality.

## ↑ Ancestors (12)

1. [C](../c.md)
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
