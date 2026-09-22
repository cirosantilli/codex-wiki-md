<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Store a second [array](../../../../../array-data-structure.md) `weight` with `weight[k] = 2^k`. Descending through the [binary digits](../../../../../binary-digit.md) of the answer gives this [greedy algorithm](../../../../../greedy-algorithm.md):
```
PROCEDURE FastLog(b, n: INTEGER): INTEGER;
VAR b2, weight: ARRAY enough OF INTEGER;
    top, k, i, p: INTEGER;
BEGIN
  b2[0] := b; weight[0] := 1; top := 0;
  WHILE b2[top]*b2[top] <= n DO
    b2[top+1] := b2[top]*b2[top];
    weight[top+1] := weight[top]+weight[top];
    top := top+1
  END;
  i := 0; p := 1; k := top;
  WHILE k >= 0 DO
    IF p*b2[k] <= n THEN
      p := p*b2[k]; i := i+weight[k]
    END;
    k := k-1
  END;
  RETURN i
END FastLog;
```
For the second loop, write $L=\lfloor\log_b n\rfloor$. Immediately before processing $k$, its [loop invariant](../../../../../loop-invariant.md) is

$$
p=b^i\leq n,\qquad i\leq L<i+2^{k+1}.
$$

Initially the failed squaring guard gives $L<2^{\mathrm{top}+1}$; this also holds when $b>n$, since then $L=0$. The test succeeds exactly when $i+2^k\leq L$. If successful, adding $2^k$ selects that [binary digit](../../../../../binary-digit.md); otherwise the upper bound tightens to $L<i+2^k$. Either way the invariant holds for the next smaller $k$. At $k=-1$, $i\leq L<i+1$, so **`i = L`**.

There are $O(1+\log(1+\log_b n))$ squarings and descending tests. For fixed $b$, this is **$O(1+\log\log n)$ arithmetic operations**, hence logarithmic in the [bit length](../../../../../bit-length.md) of $n$, and also within the weaker $O(\log n)$ bound. This counts arithmetic operations on [integers](../../../../../integer-split.md) as unit cost; [bit complexity](../../../../../bit-complexity.md) would also charge for the growing operands. No division is used.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
