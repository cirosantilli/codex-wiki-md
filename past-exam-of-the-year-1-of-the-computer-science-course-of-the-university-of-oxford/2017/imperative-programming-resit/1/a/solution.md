<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the supplied pointer-to-record representation and allocate a fresh record:

```
PROCEDURE mkRat(n,d: INTEGER): rational;
VAR z: rational;
BEGIN
  ASSERT(d # 0);
  NEW(z); z.num := n; z.den := d;
  reduce(z);
  RETURN z
END mkRat;
```

The [rational number](../../../../../rational-number.md) constructor returns a value with positive denominator in lowest terms, using part (b). Zero is represented as $0/1$. Arithmetic below uses exact integers, or inputs whose intermediate values fit the chosen implementation; fixed-width overflow would otherwise invalidate exact arithmetic.

## ↑ Ancestors (12)

1. [A](../a.md)
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
