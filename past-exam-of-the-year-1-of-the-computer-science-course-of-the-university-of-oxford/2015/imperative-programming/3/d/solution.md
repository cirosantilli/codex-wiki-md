<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Reuse `p` as `q`'s header and allocate one new header for `r`. Cut after $k=\lfloor n/2\rfloor$ data elements, allowing $k=0$.
```
PROCEDURE Split(p: List; VAR q, r: List);
VAR n, k, i: INTEGER; last: Tail;
BEGIN
  n := p.count; k := n DIV 2;
  q := p; NEW(r);
  last := q;
  FOR i := 1 TO k DO last := last.tail END;
  r.tail := last.tail; last.tail := NIL;
  q.count := k; r.count := n-k
END Split;
```
The traversal starts at the [dummy header node](../../../../../sentinel-node.md), so after $k$ steps `last` precedes the suffix assigned to `r`. Cutting that link produces two finite disjoint [linked lists](../../../../../linked-list.md). Their concatenated [abstraction function](../../../../../abstraction-function.md) is the original [list](../../../../../list-abstract-data-type.md), with order preserved, and

$$
\boxed{|q|=\lfloor n/2\rfloor,\quad |r|=\lceil n/2\rceil,\quad\alpha(p_{\mathrm{old}}.\mathrm{tail})=\alpha(q.\mathrm{tail})\mathbin{+\!+}\alpha(r.\mathrm{tail}).}
$$

Both empty and singleton inputs work without special traversal cases. The [time complexity](../../../../../time-complexity.md) is $O(n)$ and only one header is allocated.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
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
