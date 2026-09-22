<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Represent the [zero polynomial](../../../../../zero-polynomial.md) by `degree = -1`, with an allocated one-element [array](../../../../../array-data-structure.md) whose element is zero. Its coefficient prefix is empty; the spare cell is merely convenient storage. For every nonzero [polynomial](../../../../../polynomial-split.md), require `degree >= 0`, sufficient allocated capacity, and a nonzero leading [polynomial coefficient](../../../../../coefficient-of-a-polynomial.md).
```
PROCEDURE Zero(VAR p: Poly);
BEGIN
  p.degree := -1; NEW(p.coeff, 1); p.coeff[0] := 0.0
END Zero;

PROCEDURE Normalize(VAR p: Poly);
BEGIN
  WHILE p.degree >= 0 DO
    IF p.coeff[p.degree] # 0.0 THEN RETURN END;
    DEC(p.degree)
  END
END Normalize;
```
Thus

$$
\boxed{\deg_{\mathrm{stored}}0=-1;\qquad p\ne0\Longrightarrow p_{p.\mathrm{degree}}\ne0.}
$$

The sentinel $-1$ is a representation convention, not an assertion that the mathematical [degree of the zero polynomial](../../../../../degree-of-the-zero-polynomial.md) is an ordinary integer. In parts (b)–(e), algebraic correctness uses exact arithmetic on [real numbers](../../../../../real-number.md); ordinary [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md) introduces rounding and needs an additional numerical policy if exact zero tests are to be replaced.

## ↑ Ancestors (12)

1. [A](../a.md)
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
