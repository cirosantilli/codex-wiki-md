<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For nonnegative [integer](../../../../../integer-split.md) `x` and positive [integer](../../../../../integer-split.md) `y`, initialize the quotient to zero and subtract one divisor at a time:

```
q := 0; r := x;
WHILE r >= y DO
  r := r-y;
  q := q+1
END
```

The [loop invariant](../../../../../loop-invariant.md) is $x=qy+r$, $q\geq0$, $r\geq0$, with `x` and `y` unchanged. It is true initially. A body execution changes $qy+r$ to $(q+1)y+(r-y)=qy+r$ and keeps $r$ nonnegative because of the guard. The nonnegative [integer](../../../../../integer-split.md) [loop variant](../../../../../loop-variant.md) $r$ strictly decreases by $y>0$, so termination follows. At exit the guard supplies $r<y$; hence

$$
\boxed{q=\left\lfloor\frac{x}{y}\right\rfloor,\qquad r=x-qy,\qquad0\leq r<y.}
$$

There are exactly $\lfloor x/y\rfloor$ body executions. Under the [unit-cost model](../../../../../unit-cost-model.md), the [time complexity](../../../../../time-complexity.md) including initialization and the final test is $\Theta(1+\lfloor x/y\rfloor)$, which is $O(x)$ for [integer](../../../../../integer-split.md) $y\geq1$. This is a bound in the value of `x`, rather than in its encoded [bit](../../../../../bit.md) length.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
