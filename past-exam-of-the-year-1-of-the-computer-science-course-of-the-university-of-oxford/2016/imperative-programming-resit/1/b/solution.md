<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep both the exponent and its power. This [Oberon](../../../../../oberon-programming-language.md) procedure uses only the permitted arithmetic:
```
PROCEDURE IntLog(b, n: INTEGER): INTEGER;
VAR i, p: INTEGER;
BEGIN
  i := 0; p := 1;
  WHILE p*b <= n DO
    p := p*b; i := i+1
  END;
  RETURN i
END IntLog;
```
The [loop invariant](../../../../../loop-invariant.md) is $i\geq0$ and $p=b^i\leq n$. It holds initially because $n>0$. A successful guard permits the next power, and the two assignments preserve the relation between $p$ and $i$. At exit, $p\leq n<pb$, which is exactly part (a). Each iteration increases $i$, and only finitely many powers of $b\geq2$ are at most $n$, proving [algorithm termination](../../../../../algorithm-termination.md). **The returned value is $\lfloor\log_b n\rfloor$.** Its [running time](../../../../../running-time.md) is $\Theta(1+\log_b n)$ arithmetic operations; [integer overflow](../../../../../integer-overflow.md) is deferred to part (e).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
