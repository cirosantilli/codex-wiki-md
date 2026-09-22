<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Require a nonzero divisor. [Polynomial long division](../../../../../polynomial-long-division.md) repeatedly subtracts the multiple of $b$ that cancels the leading term of the current [polynomial remainder](../../../../../remainder-of-polynomial-division.md). Use fresh [arrays](../../../../../array-data-structure.md) for both outputs.
```
PROCEDURE DivMod(VAR div, mod: Poly; a, b: Poly);
VAR q, r: Poly; cap, i, j, k, old: INTEGER; t: REAL;
BEGIN
  ASSERT(b.degree >= 0);
  cap := a.degree+1; IF cap < 1 THEN cap := 1 END;
  r.degree := a.degree; NEW(r.coeff, cap);
  r.coeff[0] := 0.0;
  FOR i := 0 TO a.degree DO r.coeff[i] := a.coeff[i] END;
  IF a.degree < b.degree THEN
    Zero(q)
  ELSE
    q.degree := a.degree-b.degree;
    NEW(q.coeff, q.degree+1);
    FOR i := 0 TO q.degree DO q.coeff[i] := 0.0 END;
    WHILE r.degree >= b.degree DO
      old := r.degree; k := old-b.degree;
      t := r.coeff[old]/b.coeff[b.degree];
      q.coeff[k] := q.coeff[k]+t;
      FOR j := 0 TO b.degree-1 DO
        r.coeff[k+j] := r.coeff[k+j]-t*b.coeff[j]
      END;
      r.coeff[old] := 0.0;
      DEC(r.degree); Normalize(r)
    END;
    Normalize(q)
  END;
  div := q; mod := r
END DivMod;
```
The [loop invariant](../../../../../loop-invariant.md) is the [polynomial identity](../../../../../polynomial-identity.md) $a=qb+r$. Setting $t=r_{\mathrm{old}}/b_{\deg b}$ and $k=\mathrm{old}-\deg b$ replaces $q$ by $q+tx^k$ and $r$ by $r-tx^kb$, preserving this identity. The leading coefficient of that difference is exactly zero, so setting its stored value to zero and decreasing `degree` implements its exact cancellation. Each iteration strictly decreases the degree of the [polynomial remainder](../../../../../remainder-of-polynomial-division.md).

At termination,

$$
\boxed{a=\mathrm{div}\,b+\mathrm{mod},\qquad\mathrm{mod}=0\text{ or }\deg\mathrm{mod}<\deg b.}
$$

The [zero polynomial](../../../../../zero-polynomial.md) dividend, a lower-degree dividend, and a constant divisor are all covered. Division by the [zero polynomial](../../../../../zero-polynomial.md) is undefined. The two output record variables must be distinct and separate from the input record variables; no input coefficient [array](../../../../../array-data-structure.md) is written. For $\deg a\geq\deg b$, the work is $O((\deg a-\deg b+1)(\deg b+1))$.

## ↑ Ancestors (12)

1. [D](../d.md)
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
