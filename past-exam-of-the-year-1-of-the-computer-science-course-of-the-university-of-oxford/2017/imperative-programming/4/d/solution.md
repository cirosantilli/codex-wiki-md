<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Add the unit fractions one at a time, reducing after each addition:

```
procedure toRat(e; var m,n)
    require 0 <= e.i <= N and every stored denominator is positive
    m := 0
    n := 1
    j := 0
    while j < e.i do
        q := e.x[j]
        m := m*q+n
        n := n*q
        Reduce(m,n)
        j := j+1
```

The [loop invariant](../../../../../loop-invariant.md) is that $m/n$ is the [reduced fraction](../../../../../reduced-fraction.md) equal to the sum of the first $j$ terms, with $m\geq0,n>0$. The update is exactly $m/n+1/q=(mq+n)/(nq)$, and the [greatest common divisor](../../../../../greatest-common-divisor.md) reduction preserves it. The [loop variant](../../../../../loop-variant.md) $e.i-j$ decreases to zero. The empty sum gives **$0/1$**.

An arbitrary stored Egyptian sum can be at least one, so this uses the broader nonnegative-numerator contract of the implementation in part (a), not an unjustified assumption that every intermediate fraction is proper.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
