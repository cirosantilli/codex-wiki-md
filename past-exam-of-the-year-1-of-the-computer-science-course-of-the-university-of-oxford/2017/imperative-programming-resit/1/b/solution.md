<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Divide numerator and denominator by their positive [greatest common divisor](../../../../../greatest-common-divisor.md), then fix the sign:

```
PROCEDURE reduce(x: rational);
VAR g: INTEGER;
BEGIN
  ASSERT(x.den # 0);
  g := gcd(ABS(x.num),ABS(x.den));
  x.num := x.num DIV g; x.den := x.den DIV g;
  IF x.den < 0 THEN
    x.num := -x.num; x.den := -x.den
  END
END reduce;
```

The denominator condition ensures $g>0$, including when the numerator is zero. Dividing both components by the same nonzero integer preserves the fraction, and the final simultaneous sign change preserves it again. The resulting numerator and denominator are [coprime](../../../../../coprime-integers.md); for zero the denominator becomes one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
