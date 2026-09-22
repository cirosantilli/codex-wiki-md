# Matrix geometric series

↑ **Parent:** [Linear algebra](linear-algebra-split.md)

The finite [matrix geometric series](matrix-geometric-series.md) telescopes as stated in the title. If its partial sums converge, then their successive differences show $D^{m+1}\to0$. Passing to the limit gives $(I-D)\sum_{j\geq0}D^j=I$, so the sum is the [matrix inverse](matrix-inverse-split.md) $(I-D)^{-1}$. Conversely, existence of the inverse alone does not imply series convergence: the scalar matrix $D=2I$ is a counterexample. The [Neumann series](neumann-series.md) gives a sufficient condition from a matrix norm smaller than one.

For a [nilpotent matrix](nilpotent-matrix.md) with $D^r=0$, convergence is automatic and the inverse is the finite polynomial $I+D+\cdots+D^{r-1}$. Multiplying by $I-D$ directly verifies this inverse without computing a determinant or diagonalizing.

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Matrix geometric series](matrix-geometric-series.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/5/c/solution.md)
