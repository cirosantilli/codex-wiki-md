<h1 id="19d/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [orthogonal matrix](../../../../../../../orthogonal-matrix.md) $Q$ preserves the [Euclidean norm](../../../../../../../euclidean-norm.md), so

$$
\|Ax-b\|^2=\|Rx-Q^Tb\|^2,
\qquad Q^Tb=\begin{pmatrix}98/25\\35\\4\\-3\end{pmatrix}.
$$

The first three entries of $Rx-Q^Tb$ can be set to zero by [backward substitution in a triangular system](../../../../../../../backward-substitution-in-a-triangular-system.md), while its fourth entry is always $3$. Solving the triangular system gives $x_3=16/5$, $x_2=(35-2x_3)/5=143/25$, and $x_1=(98/25-x_2-x_3)/3=-5/3$. Thus **the unique [least-squares solution](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) and residual norm are**

$$
\boxed{x^*=\begin{pmatrix}-5/3\\143/25\\16/5\end{pmatrix},\qquad\|Ax^*-b\|=3.}
$$

Uniqueness follows from the nonzero diagonal entries of the top triangular block, equivalently the full column rank of $A$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [19D](../../../19d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
