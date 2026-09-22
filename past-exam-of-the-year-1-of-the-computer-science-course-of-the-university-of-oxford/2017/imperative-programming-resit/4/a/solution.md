<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A suitable [Oberon](../../../../../oberon-programming-language.md) linked representation is

```
TYPE
  poly = POINTER TO term;
  term = RECORD
    coeff: T;
    power: INTEGER;
    next: poly
  END;
```

`NIL` denotes the zero polynomial. Each power is a nonnegative integer, and the intended sparse representation omits zero coefficients. No sorted-order assumption is needed for the operations below. Coefficients are treated as values with equality to zero, addition and multiplication; mutable coefficient objects would need the corresponding copying discipline.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
