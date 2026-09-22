<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $n\geq3$ and use periodic indices for the [Jacobi method](../../../../../../jacobi-method.md). At iteration $r$, it is

$$
\boxed{x_j^{(r+1)}=\tfrac12\bigl(x_{j-1}^{(r)}+x_{j+1}^{(r)}-b_j\bigr),\qquad x_0=x_n,\quad x_{n+1}=x_1.}
$$

All values on its right side belong to the old iterate. For lexicographic [Gauss-Seidel iteration](../../../../../../gauss-seidel-method.md), compute in the order $1,\ldots,n$ and use a newly available coordinate immediately:

$$
\begin{aligned}
x_1^{(r+1)}&=\tfrac12(x_2^{(r)}+x_n^{(r)}-b_1),\\
x_j^{(r+1)}&=\tfrac12(x_{j-1}^{(r+1)}+x_{j+1}^{(r)}-b_j),\quad 2\leq j\leq n-1,\\
x_n^{(r+1)}&=\tfrac12(x_1^{(r+1)}+x_{n-1}^{(r+1)}-b_n).
\end{aligned}
$$

The wrap-around term in the last row uses the new $x_1$, while the wrap-around term in the first row uses the old $x_n$. This is important for the actual [iteration matrix](../../../../../../iteration-matrix.md) and its convergence behavior.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
