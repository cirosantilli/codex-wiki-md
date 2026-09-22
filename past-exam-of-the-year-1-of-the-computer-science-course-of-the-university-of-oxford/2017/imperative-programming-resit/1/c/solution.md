<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the ordinary fraction identities, returning fresh records rather than changing either argument:

```
PROCEDURE addRat(x,y: rational): rational;
BEGIN
  RETURN mkRat(x.num*y.den + y.num*x.den, x.den*y.den)
END addRat;

PROCEDURE mulRat(x,y: rational): rational;
BEGIN
  RETURN mkRat(x.num*y.num, x.den*y.den)
END mulRat;

PROCEDURE negRat(x: rational): rational;
BEGIN
  RETURN mkRat(-x.num,x.den)
END negRat;
```

Every result is reduced by `mkRat`. This preserves the [representation invariant](../../../../../representation-invariant.md) even if an input was initially unreduced, provided its denominator is nonzero. [Aliasing](../../../../../aliasing.md) between the arguments causes no problem because their fields are only read.

## ↑ Ancestors (12)

1. [C](../c.md)
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
