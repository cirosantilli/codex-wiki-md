<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Append each quotient directly to the output [linked list](../../../../../linked-list.md), retaining a pointer to its last node. The nodes are required output; auxiliary variables remain simple [integers](../../../../../integer-split.md) and [pointers](../../../../../pointer-computer-programming.md).
```
PROCEDURE rat2cf(n, d: INTEGER): fraction;
VAR first, last, p: fraction; q, r: INTEGER;
BEGIN
  first := NIL; last := NIL;
  REPEAT
    q := n DIV d; r := n MOD d;
    NEW(p); p.head := q; p.tail := NIL;
    IF first = NIL THEN first := p
    ELSE last.tail := p
    END;
    last := p;
    n := d; d := r
  UNTIL d = 0;
  RETURN first
END rat2cf;
```
At the start of each iteration, `d` is positive, and the output prefix consists exactly of the quotients already obtained by the [Euclidean algorithm](../../../../../euclidean-algorithm.md). `last` points to its final node, or both `first` and `last` are null when the prefix is empty. The current ratio `n/d` is the unexpanded tail of the original [continued fraction](../../../../../continued-fraction.md). The quotient/remainder step extends that prefix by the same value as the recursive version, then replaces the unexpanded ratio by its reciprocal residual tail. If the remainder is zero, no tail remains and the loop stops before another division.

The [loop variant](../../../../../loop-variant.md) is the positive current denominator, which strictly decreases after each nonfinal iteration. The input denominator is positive, so at least one node is allocated, including for zero or an integral ratio. **This is the same exact conversion with $O(1)$ auxiliary space, excluding the returned list, and no input mutation.**

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
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
