<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Separate [integer partitions](../../../../../integer-partition.md) according to whether they contain a part equal to $i$. Removing one such part is a [bijection](../../../../../bijection.md) to partitions of $n-i$ whose parts are at most $i$. The alternatives are disjoint, giving

$$
\boxed{p(i,n)=p(i-1,n)+p(i,n-i)\quad(i\geq1,\ n\geq1).}
$$

Use $p(i,0)=1$, because the empty [integer partition](../../../../../integer-partition.md) is counted once, and $p(0,n)=0$ for $n>0$, with $p(i,n)=0$ for $n<0$. This [Oberon](../../../../../oberon-programming-language.md) implementation avoids negative recursive arguments:
```
PROCEDURE P(i, n: INTEGER): INTEGER;
VAR answer: INTEGER;
BEGIN
  IF n = 0 THEN answer := 1
  ELSIF i = 0 THEN answer := 0
  ELSIF i > n THEN answer := P(i-1, n)
  ELSE answer := P(i-1, n) + P(i, n-i)
  END;
  RETURN answer
END P;

PROCEDURE Partitions(n: INTEGER): INTEGER;
BEGIN
  RETURN P(n, n)
END Partitions;
```
The [precondition](../../../../../precondition.md) is $i,n\geq0$. Each [recursive call](../../../../../recursive-call.md) reduces $i+n$, proving [algorithm termination](../../../../../algorithm-termination.md). Every positive part of a partition of $n$ is at most $n$, so **the required one-argument count is $P(n,n)$**. Counts require a sufficiently wide [integer](../../../../../integer-split.md) representation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
