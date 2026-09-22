<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Euclidean algorithm](../../../../../euclidean-algorithm.md) with floor quotient and nonnegative remainder, including for a negative numerator:
```
PROCEDURE rat2cf(n, d: INTEGER): fraction;
VAR q, r: INTEGER; p: fraction;
BEGIN
  q := n DIV d; r := n MOD d;
  NEW(p); p.head := q; p.tail := NIL;
  IF r # 0 THEN p.tail := rat2cf(d, r) END;
  RETURN p
END rat2cf;
```
For $d>0$, [Euclidean division](../../../../../euclidean-division.md) gives $n=qd+r$ with $0\leq r<d$. If $r=0$, the singleton `[q]` is exact. Otherwise

$$
\frac nd=q+\frac rd=q+\frac1{d/r},
$$

so the recursive tail represents $d/r$. Its numerator is positive and greater than its denominator, so every tail head is a positive [integer](../../../../../integer-split.md). The new denominator $r$ is strictly smaller than $d$, proving [algorithm termination](../../../../../algorithm-termination.md) by descent through the positive [integers](../../../../../integer-split.md).

**The returned list represents exactly $n/d$.** For example $-7/3=-3+1/(1+1/2)$ gives `[-3,1,2]`; truncating negative division toward zero would violate the required positivity of the tail. There are $O(\log d)$ [Euclidean algorithm](../../../../../euclidean-algorithm.md) steps, with output allocation and recursive stack depth linear in the number of generated nodes.

## ↑ Ancestors (12)

1. [B](../b.md)
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
