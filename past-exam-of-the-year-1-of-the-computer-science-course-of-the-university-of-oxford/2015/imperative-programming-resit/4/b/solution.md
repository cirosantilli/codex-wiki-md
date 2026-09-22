<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep `u[0..len)` sorted, with the [coupling invariant](../../../../../coupling-invariant.md)

$$
0\leq\mathrm{len}\leq N,\qquad \mathrm{len}=\operatorname{length}(xs),\qquad
u[0..\mathrm{len})=\operatorname{sort}(xs).
$$

The abstract [list](../../../../../list-abstract-data-type.md) retains insertion order, while the concrete [array](../../../../../array-data-structure.md) retains its sorted [multiset](../../../../../multiset.md). Initially both are empty.
```
PROCEDURE Add(x: INTEGER);
VAR i: INTEGER;
BEGIN
  ASSERT(len < N);
  i := len;
  WHILE i > 0 DO
    IF u[i-1] <= x THEN EXIT END;
    u[i] := u[i-1];
    i := i-1
  END;
  u[i] := x;
  len := len+1
END Add;

PROCEDURE Get(k: INTEGER): INTEGER;
BEGIN
  ASSERT((0 <= k) & (k < len));
  RETURN u[k]
END Get;
```
For insertion, conceptually treat index `i` as a hole. If $U$ is the old sorted prefix of length $n$, the [loop invariant](../../../../../loop-invariant.md) is $0\leq i\leq n$, $u[0..i)=U[0..i)$ and $u[i+1..n+1)=U[i..n)$, with every shifted value strictly greater than $x$. The [loop variant](../../../../../loop-variant.md) is $i$. The exit condition gives either no left neighbour or a left neighbour at most $x$; filling the hole establishes [sortedness](../../../../../sortedness.md) and adds exactly one occurrence, preserving the [coupling invariant](../../../../../coupling-invariant.md).

$$
\boxed{\operatorname{get}:\Theta(1),\qquad\operatorname{add}:O(n)\text{ and worst-case }\Theta(n).}
$$

When the new entry is smaller than every old entry, all $n$ old values must move in this contiguous sorted-prefix representation. [Binary search](../../../../../binary-search.md) can reduce comparisons to locate the insertion point, but cannot remove that linear movement cost. Appending a new largest value takes constant time in this implementation.

## ↑ Ancestors (12)

1. [B](../b.md)
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
