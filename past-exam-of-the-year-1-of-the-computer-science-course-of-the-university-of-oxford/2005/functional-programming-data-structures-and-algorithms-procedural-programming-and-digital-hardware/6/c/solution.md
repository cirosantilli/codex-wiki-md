<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Replace the recursive transfer in part (b) by simultaneous state updates, using a temporary variable to preserve the old `a`:

```
PROCEDURE FibIter(n: INTEGER): INTEGER;
  VAR k, a, b, oldA: INTEGER;
BEGIN
  k := n; a := 1; b := 0;
  WHILE k > 1 DO
    oldA := a;
    a := a + b;
    b := oldA;
    k := k - 1
  END;
  RETURN a
END FibIter;
```

For original input $N\geq1$, a [loop invariant](../../../../../loop-invariant.md) is

$$
\boxed{1\leq k\leq N,\qquad aF_k+bF_{k-1}=F_N.}
$$

It holds initially because $a=1,b=0,k=N$. Each iteration preserves it by the identity from part (b). The [loop variant](../../../../../loop-variant.md) is $k-1$, a nonnegative [integer](../../../../../integer-split.md) that decreases by one whenever the guard holds. On exit $k=1$, so the [loop invariant](../../../../../loop-invariant.md) gives $aF_1+bF_0=a=F_N$, exactly the returned answer. The procedure uses $O(n)$ arithmetic operations and $O(1)$ stored [integer](../../../../../integer-split.md) variables, without depending on compiler treatment of [tail calls](../../../../../tail-call.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
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
