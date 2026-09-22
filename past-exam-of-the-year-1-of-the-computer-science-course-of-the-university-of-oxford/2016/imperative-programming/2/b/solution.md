<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Test each possible positive [divisor](../../../../../divisor.md) directly:
```
PROCEDURE divisors(n: INTEGER): INTEGER;
VAR i, count: INTEGER;
BEGIN
  i := 1; count := 0;
  WHILE i <= n DO
    IF n MOD i = 0 THEN count := count + 1 END;
    i := i + 1
  END;
  RETURN count
END divisors;
```
For $n\geq1$, the [loop invariant](../../../../../loop-invariant.md) is $1\leq i\leq n+1$ and `count` $=|\{d:1\leq d<i,\ d\mid n\}|$. Testing $i$ adds exactly the next possible [divisor](../../../../../divisor.md). The [loop variant](../../../../../loop-variant.md) $n+1-i$ decreases, and the divisor in `MOD` is always positive. At exit the interval $1\leq d\leq n$ contains every positive [divisor](../../../../../divisor.md). **This computes the [divisor function](../../../../../divisor-function.md) $\tau(n)$ using $n$ remainder operations, $\Theta(n)$ time, and $O(1)$ auxiliary space.**

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
