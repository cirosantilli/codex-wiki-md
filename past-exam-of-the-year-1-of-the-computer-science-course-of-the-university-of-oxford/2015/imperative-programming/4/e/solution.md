<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Scan the [polynomial coefficients](../../../../../coefficient-of-a-polynomial.md) from highest degree downward. Omit zero terms, omit coefficient magnitude one on nonconstant terms, print `-` for negative terms, and print `+` only before a positive term after the first. A helper prints small integral magnitudes without a decimal suffix; other [real numbers](../../../../../real-number.md) use `Out.Real`.
```
PROCEDURE OutMagnitude(c: REAL);
VAR n: INTEGER;
BEGIN
  IF c < MAX(INTEGER) THEN
    n := ENTIER(c);
    IF c = n THEN Out.Int(n, 0) ELSE Out.Real(c, 0) END
  ELSE
    Out.Real(c, 0)
  END
END OutMagnitude;

PROCEDURE OutPoly(p: Poly);
VAR i: INTEGER; c, magnitude: REAL; first: BOOLEAN;
BEGIN
  IF p.degree < 0 THEN Out.String("0"); RETURN END;
  first := TRUE; i := p.degree;
  WHILE i >= 0 DO
    c := p.coeff[i];
    IF c # 0.0 THEN
      IF c < 0.0 THEN Out.Char("-")
      ELSIF ~first THEN Out.Char("+")
      END;
      magnitude := ABS(c);
      IF (i = 0) OR (magnitude # 1.0) THEN
        OutMagnitude(magnitude)
      END;
      IF i > 0 THEN
        Out.Char("x");
        IF i > 1 THEN Out.Char("^"); Out.Int(i, 0) END
      END;
      first := FALSE
    END;
    DEC(i)
  END
END OutPoly;
```
The [representation invariant](../../../../../representation-invariant.md) ensures a nonzero [polynomial](../../../../../polynomial-split.md) prints at least one term. Constant $1$ and $-1$ retain their coefficients, whereas $x$ and $-x$ omit magnitude one. Thus the requested example prints

$$
\boxed{x^4-3x^2+7x-1.}
$$

Different `Out.Real` implementations may use decimal or scientific notation for nonintegral coefficients; either denotes the appropriate [real number](../../../../../real-number.md). The number of coefficient inspections is linear in the stored [polynomial degree](../../../../../degree-of-a-polynomial.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
