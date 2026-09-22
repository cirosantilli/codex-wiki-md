<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [transportation problem](../../../../../../transportation-problem.md) chooses nonnegative shipments $x_{ij}$ from $n$ suppliers to $m$ consumers so that row sums equal supplies and column sums equal demands, while minimizing $\sum c_{ij}x_{ij}$.

The north-west corner rule gives

$$
X_{NW}=
\begin{pmatrix}
3&3&0&0\\
0&2&2&0\\
0&0&5&3
\end{pmatrix}.
$$

It has $3+4-1=6$ positive cells and its support contains no cycle, so it is a nondegenerate [basic feasible solution](../../../../../../basic-feasible-solution.md).

A degenerate basic feasible solution is

$$
\boxed{
X_D=
\begin{pmatrix}
3&0&3&0\\
0&0&4&0\\
0&5&0&3
\end{pmatrix}}.
$$

Its five positive cells form a forest with two balanced components; adding one zero cell that joins the components completes a basis of six cells. Thus at least one basic variable is zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
