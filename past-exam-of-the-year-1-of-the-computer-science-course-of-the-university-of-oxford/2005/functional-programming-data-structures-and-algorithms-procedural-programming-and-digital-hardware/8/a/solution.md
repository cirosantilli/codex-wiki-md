<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use an [Oberon](../../../../../oberon-programming-language.md) record containing an active coefficient count and a bounded [array](../../../../../array-data-structure.md) of coefficients in ascending power order. A count of zero represents the zero [polynomial](../../../../../polynomial-split.md); a count $n+1$ represents $a_0+\cdots+a_nx^n$. Trailing zero coefficients are allowed, so the count need not be the [degree of a polynomial](../../../../../degree-of-a-polynomial.md) plus one.

```
CONST Capacity = 1024;
TYPE Polynomial = RECORD
  len: INTEGER;
  coeff: ARRAY Capacity OF REAL
END;

PROCEDURE Horner(VAR p: Polynomial; x: REAL): REAL;
  VAR i: INTEGER; value: REAL;
BEGIN
  i := p.len; value := 0.0;
  WHILE i > 0 DO
    i := i-1;
    value := p.coeff[i] + x*value
  END;
  RETURN value
END Horner;
```

The [representation invariant](../../../../../representation-invariant.md) is $0\leq\texttt{len}\leq\texttt{Capacity}$, with only indices below `len` significant. The parameter is passed by reference to avoid a full record copy; the procedure does not modify it.

Let $L$ be the original coefficient count. At each guard test the [loop invariant](../../../../../loop-invariant.md) is

$$
0\leq i\leq L,\qquad
v=\sum_{j=i}^{L-1}a_jx^{j-i}.
$$

The empty sum is zero initially. If the old index is $i>0$, after decrementing and updating,

$$
v_{\mathrm{new}}=a_{i-1}+x\sum_{j=i}^{L-1}a_jx^{j-i}
=\sum_{j=i-1}^{L-1}a_jx^{j-(i-1)},
$$

which preserves the [loop invariant](../../../../../loop-invariant.md). The [loop variant](../../../../../loop-variant.md) is $i$, decreasing by one until zero. At exit,

$$
\boxed{v=\sum_{j=0}^{L-1}a_jx^j=p(x).}
$$

This is exactly the right-to-left nesting of [Horner's method](../../../../../horner-s-method.md), matching the supplied [right fold](../../../../../list-fold.md). It uses $O(L)$ arithmetic operations and $O(1)$ additional scalar storage. `REAL` gives ordinary floating-point evaluation; the displayed identities specify the ideal arithmetic calculation, with the usual rounding in an actual floating-point implementation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
