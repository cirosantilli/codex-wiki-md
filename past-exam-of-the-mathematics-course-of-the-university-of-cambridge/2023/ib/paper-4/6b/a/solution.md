<h1 id="6b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The nonzero [orthogonal polynomials](../../../../../../orthogonal-polynomial.md) $Q_0,\ldots,Q_n$ have distinct degrees and form an orthogonal basis of $\mathcal P_n$. Define

$$
p_n^*=\sum_{k=0}^n
\frac{\langle f,Q_k\rangle}{\langle Q_k,Q_k\rangle}Q_k.
$$

For each $j\leq n$,

$$
\langle f-p_n^*,Q_j\rangle
=\langle f,Q_j\rangle
-\frac{\langle f,Q_j\rangle}{\langle Q_j,Q_j\rangle}
\langle Q_j,Q_j\rangle=0.
$$

Thus the residual $f-p_n^*$ is [orthogonal](../../../../../../orthogonal-vectors.md) to all of $\mathcal P_n$.

For any $p\in\mathcal P_n$, write

$$
f-p=(f-p_n^*)+(p_n^*-p).
$$

The two terms are orthogonal, so the [Pythagorean theorem in an inner-product space](../../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\lVert f-p\rVert^2
=\lVert f-p_n^*\rVert^2+\lVert p_n^*-p\rVert^2
\geq\lVert f-p_n^*\rVert^2.
$$

Equality holds only for $p=p_n^*$. This proves the formula and uniqueness of the [least-squares polynomial in an orthogonal-polynomial basis](../../../../../../least-squares-polynomial-in-an-orthogonal-polynomial-basis.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6B](../../6b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
