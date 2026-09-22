<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Allocate a fresh coefficient [array](../../../../../array-data-structure.md), add matching [polynomial coefficients](../../../../../coefficient-of-a-polynomial.md), and normalize to remove any cancellation of leading terms.
```
PROCEDURE Add(VAR sum: Poly; a, b: Poly);
VAR result: Poly; d, cap, i: INTEGER;
BEGIN
  d := a.degree;
  IF b.degree > d THEN d := b.degree END;
  cap := d+1; IF cap < 1 THEN cap := 1 END;
  result.degree := d; NEW(result.coeff, cap);
  result.coeff[0] := 0.0;
  FOR i := 0 TO d DO
    result.coeff[i] := 0.0;
    IF i <= a.degree THEN
      result.coeff[i] := result.coeff[i] + a.coeff[i]
    END;
    IF i <= b.degree THEN
      result.coeff[i] := result.coeff[i] + b.coeff[i]
    END
  END;
  Normalize(result); sum := result
END Add;
```
The [loop invariant](../../../../../loop-invariant.md) says that every completed coefficient equals the corresponding coefficient of $a+b$, treating missing coefficients as zero. `Normalize` changes no represented [polynomial](../../../../../polynomial-split.md), and can reduce the result to the [zero polynomial](../../../../../zero-polynomial.md).

$$
\boxed{(a+b)_i=a_i+b_i;\quad\text{time }O(1+\max(\deg a,\deg b)).}
$$

Neither input coefficient [array](../../../../../array-data-structure.md) is changed. Output variables are separate from input record variables; the fresh result also remains safe when the two inputs share a coefficient [array](../../../../../array-data-structure.md).

## ↑ Ancestors (12)

1. [B](../b.md)
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
