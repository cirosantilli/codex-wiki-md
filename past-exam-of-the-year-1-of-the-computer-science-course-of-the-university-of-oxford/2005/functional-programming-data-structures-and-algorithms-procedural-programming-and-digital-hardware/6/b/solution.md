<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [tail recursion](../../../../../tail-recursion.md), each recursive call is a [tail call](../../../../../tail-call.md): its result is returned directly, with no suspended addition or other work. A compiler can then reuse an activation record, giving constant stack use. This is a possible optimization, not a guarantee made by the source syntax. The direct [Fibonacci number](../../../../../fibonacci-number.md) procedure in part (a) must retain information while waiting to add two recursive results.

Extend the [Fibonacci numbers](../../../../../fibonacci-number.md) with $F_0=0$ and use the suggested quantity $g(n,a,b)=aF_n+bF_{n-1}$. For $n>1$,

$$
aF_n+bF_{n-1}=(a+b)F_{n-1}+aF_{n-2}
=g(n-1,a+b,a),
$$

while $g(1,a,b)=a$. This gives the [Oberon](../../../../../oberon-programming-language.md) procedures

```
PROCEDURE G(n, a, b: INTEGER): INTEGER;
  VAR result: INTEGER;
BEGIN
  IF n = 1 THEN
    result := a
  ELSE
    result := G(n-1, a+b, a)
  END;
  RETURN result
END G;

PROCEDURE FibTail(n: INTEGER): INTEGER;
BEGIN
  RETURN G(n, 1, 0)
END FibTail;
```

The assignment of the recursive result does not perform arithmetic after the call; it merely passes that result to `RETURN`, so the call is in [tail recursion](../../../../../tail-recursion.md). A dialect permitting an immediate `RETURN G(...)` in the branch expresses the same control flow. The decreasing argument $n-1$ proves [algorithm termination](../../../../../algorithm-termination.md), and the displayed identity proves correctness by [mathematical induction](../../../../../mathematical-induction.md). Thus

$$
\boxed{F_n=g(n,1,0),\qquad g(n,a,b)=g(n-1,a+b,a)\ (n>1).}
$$

There are $n-1$ recursive steps, giving $O(n)$ arithmetic operations. Stack use is $O(1)$ with [tail call](../../../../../tail-call.md) elimination and $O(n)$ without it. With unbounded [integers](../../../../../integer-split.md), the growing [Fibonacci numbers](../../../../../fibonacci-number.md) also make arithmetic costs grow; the linear bound counts arithmetic operations.

## ↑ Ancestors (12)

1. [B](../b.md)
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
