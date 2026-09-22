<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Add [polynomials](../../../../../polynomial-split.md) by adding equal-power coefficients, interpreting a missing coefficient as zero. Compute into a local record before assigning the output, so the result may safely be the same actual record as either input.

```
PROCEDURE Add(VAR p, q, result: Polynomial);
  VAR t: Polynomial; i: INTEGER; u, v: REAL;
BEGIN
  t.len := p.len;
  IF q.len > t.len THEN t.len := q.len END;
  i := 0;
  WHILE i < t.len DO
    u := 0.0; v := 0.0;
    IF i < p.len THEN u := p.coeff[i] END;
    IF i < q.len THEN v := q.coeff[i] END;
    t.coeff[i] := u+v;
    i := i+1
  END;
  result := t
END Add;
```

With $L=\max(p.\texttt{len},q.\texttt{len})$, the [loop invariant](../../../../../loop-invariant.md) is $0\leq i\leq L$ and, for $0\leq k<i$, `t.coeff[k]` is the sum of the two extended input coefficients at $k$. The [loop variant](../../../../../loop-variant.md) is $L-i$. The inputs remain unchanged throughout the loop, and at exit every active coefficient is correct. The [time complexity](../../../../../time-complexity.md) is $O(L)$ for the active arithmetic; assigning the fixed-capacity record can additionally copy its full capacity.

For the product, each pair of input terms contributes $a_ib_jx^{i+j}$. Initialize the active result to zero, then accumulate these pairwise contributions:

```
PROCEDURE Multiply(VAR p, q, result: Polynomial);
  VAR t: Polynomial; i, j, k: INTEGER;
BEGIN
  t.len := 0;
  IF (p.len > 0) & (q.len > 0) THEN
    t.len := p.len + q.len - 1
  END;
  (* Precondition: t.len <= Capacity. *)
  k := 0;
  WHILE k < t.len DO
    t.coeff[k] := 0.0; k := k+1
  END;
  IF t.len > 0 THEN
    i := 0;
    WHILE i < p.len DO
      j := 0;
      WHILE j < q.len DO
        t.coeff[i+j] := t.coeff[i+j]
                          + p.coeff[i]*q.coeff[j];
        j := j+1
      END;
      i := i+1
    END
  END;
  result := t
END Multiply;
```

The input [representation invariants](../../../../../representation-invariant.md) and the capacity [precondition](../../../../../precondition.md) are assumed. No coefficient is accessed when either input is the zero [polynomial](../../../../../polynomial-split.md). The initialization [loop invariant](../../../../../loop-invariant.md) says coefficients below $k$ are zero; its [loop variant](../../../../../loop-variant.md) is `t.len-k`.

For positive input lengths $m,n$, the outer [loop invariant](../../../../../loop-invariant.md) says that $0\leq i\leq m$ and each coefficient $t_k$ equals

$$
\sum_{0\leq u<i}\ \sum_{\substack{0\leq v<n\\u+v=k}}a_ub_v.
$$

The inner [loop invariant](../../../../../loop-invariant.md) adds the contributions with $u=i$ and $0\leq v<j$ to that sum, while $0\leq j\leq n$. The update adds exactly the next missing term at index $i+j$, preserving the inner [loop invariant](../../../../../loop-invariant.md). The [loop variants](../../../../../loop-variant.md) are $m-i$ for the outer loop and $n-j$ for the inner loop. On exit all pairs have contributed, yielding

$$
\boxed{(p+q)_k=a_k+b_k,\qquad
(pq)_k=\sum_{i+j=k}a_ib_j.}
$$

The product uses $O(mn+m+n)$ arithmetic operations and a temporary coefficient [array](../../../../../array-data-structure.md) of capacity `Capacity`. Both operations allow trailing zeros; no extra normalization loop is required. Only the active coefficients are meaningful, so inactive record entries are never read by these operations. As in part (a), floating-point coefficients implement these formulas subject to rounding.

## ↑ Ancestors (12)

1. [B](../b.md)
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
