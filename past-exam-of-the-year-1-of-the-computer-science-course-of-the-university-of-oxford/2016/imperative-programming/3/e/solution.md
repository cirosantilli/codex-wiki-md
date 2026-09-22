<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Accumulate the product of the $2\times2$ [matrices](../../../../../matrix.md) from left to right, which matches forward [linked list](../../../../../linked-list.md) traversal.
```
PROCEDURE cf2rat(f: fraction; VAR n, d: INTEGER);
VAR p: fraction; a, b, c, e, x: INTEGER;
BEGIN
  a := 1; b := 0; c := 0; e := 1;
  p := f;
  WHILE p # NIL DO
    x := p.head;
    a, b, c, e := a*x+b, a, c*x+e, c;
    p := p.tail
  END;
  n := a; d := c
END cf2rat;
```
The four-value assignment is simultaneous, as permitted by the source. With $M(x)=\left(\begin{smallmatrix}x&1\\1&0\end{smallmatrix}\right)$, the [loop invariant](../../../../../loop-invariant.md) after reading the prefix $x_0,\ldots,x_{t-1}$ is

$$
\begin{pmatrix}a&b\\c&e\end{pmatrix}=M(x_0)\cdots M(x_{t-1}),
$$

with the empty product initialized to the [identity matrix](../../../../../identity-matrix.md). Multiplication on the right by $M(x)$ produces exactly the four assignments above. The [associativity of matrix multiplication](../../../../../associativity-of-matrix-multiplication.md) allows this left-to-right accumulation even though the recursive conversion groups operations from the right.

At completion, the first column is the numerator/denominator pair for the whole [continued fraction](../../../../../continued-fraction.md): the last factor sends $(1,0)^T$ to $(x_n,1)^T$, and each earlier factor applies the recurrence from part (d). The vector $(1,0)^T$ is an algebraic device, not a finite input ratio requiring division by zero. For a nonempty list the resulting $c$ is positive; for a singleton it is $1$. The product has [determinant](../../../../../determinant.md) $(-1)^{n+1}$, so its first-column entries are coprime. **Return $(a,c)$ in linear node-processing time and $O(1)$ auxiliary space**, without changing the list.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
