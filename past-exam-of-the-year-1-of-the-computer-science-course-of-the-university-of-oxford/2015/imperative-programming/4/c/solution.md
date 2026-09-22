<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [polynomial convolution](../../../../../polynomial-convolution.md). If either input is the [zero polynomial](../../../../../zero-polynomial.md), return the [zero polynomial](../../../../../zero-polynomial.md) immediately.
```
PROCEDURE Mul(VAR prod: Poly; a, b: Poly);
VAR result: Poly; d, i, j: INTEGER;
BEGIN
  IF (a.degree < 0) OR (b.degree < 0) THEN
    Zero(result)
  ELSE
    d := a.degree+b.degree;
    result.degree := d; NEW(result.coeff, d+1);
    FOR i := 0 TO d DO result.coeff[i] := 0.0 END;
    FOR i := 0 TO a.degree DO
      FOR j := 0 TO b.degree DO
        result.coeff[i+j] := result.coeff[i+j]
                              + a.coeff[i]*b.coeff[j]
      END
    END;
    Normalize(result)
  END;
  prod := result
END Mul;
```
Each pair of terms contributes $a_i b_j x^{i+j}$, so the final [polynomial coefficient](../../../../../coefficient-of-a-polynomial.md) of $x^k$ is

$$
\boxed{(ab)_k=\sum_{i+j=k}a_i b_j.}
$$

With exact arithmetic on [real numbers](../../../../../real-number.md), the product of the leading nonzero [polynomial coefficients](../../../../../coefficient-of-a-polynomial.md) is nonzero, giving degree $\deg a+\deg b$. The nested loops implement precisely this sum, preserve the input coefficient [arrays](../../../../../array-data-structure.md), and take $O((\deg a+1)(\deg b+1))$ time for nonzero inputs.

## ↑ Ancestors (12)

1. [C](../c.md)
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
