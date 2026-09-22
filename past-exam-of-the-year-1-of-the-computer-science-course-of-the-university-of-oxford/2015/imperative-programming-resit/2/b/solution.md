<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [binary search](../../../../../binary-search.md) on an interval with unequal endpoint values. The [array](../../../../../array-data-structure.md) need not be sorted:
```
l := 0; r := n;
WHILE r-l > 1 DO
  m := l + (r-l) DIV 2;
  IF b[l] # b[m] THEN r := m ELSE l := m END
END;
k := l;
```
The [loop invariant](../../../../../loop-invariant.md) is

$$
0\leq l<r\leq n,\qquad b[l]\ne b[r].
$$

It holds initially by the given endpoint inequality, which also implies $n\geq1$. When $r-l>1$, $l<m<r$. If $b[l]\ne b[m]$, replacing $r$ maintains unequal endpoints. Otherwise $b[m]=b[l]\ne b[r]$, so replacing $l$ maintains them. This does not require monotonicity or even just two possible values.

The positive [integer](../../../../../integer-split.md) width $r-l$ is a [loop variant](../../../../../loop-variant.md), reduced to at most its old half rounded up. On exit $r=l+1$, giving

$$
\boxed{0\leq k<n,\qquad b[k]\ne b[k+1],\qquad T(n)=\Theta(1+\log n).}
$$

There are at most $\lceil\log_2 n\rceil$ iterations. The additive constant handles $n=1$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
