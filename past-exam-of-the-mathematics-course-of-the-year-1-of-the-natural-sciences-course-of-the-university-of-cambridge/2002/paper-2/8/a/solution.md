<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [orthogonal matrix](../../../../../orthogonal-matrix.md) satisfies $A^{-1}=A^T$, while a [symmetric matrix](../../../../../symmetric-matrix.md) satisfies $A^T=A$. Combining them gives $\boxed{A^{-1}=A}$. For the product with the [antisymmetric matrix](../../../../../skew-symmetric-matrix.md) $B$, the rule for the [transpose](../../../../../transpose.md) of a [matrix product](../../../../../matrix-product.md) gives

$$
(AB)^T=B^TA^T=-BA.
$$

Thus $AB$ is an [antisymmetric matrix](../../../../../skew-symmetric-matrix.md) exactly when $AB=BA$. The hypotheses do not force this [commutativity](../../../../../commutativity.md). For a counterexample, take

$$
A=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad B=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad AB=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

Here $A$ is a [symmetric matrix](../../../../../symmetric-matrix.md) and an [orthogonal matrix](../../../../../orthogonal-matrix.md), and $B$ is an [antisymmetric matrix](../../../../../skew-symmetric-matrix.md) and an [orthogonal matrix](../../../../../orthogonal-matrix.md), but $AB$ is a nonzero [symmetric matrix](../../../../../symmetric-matrix.md), so it is not an [antisymmetric matrix](../../../../../skew-symmetric-matrix.md). On the other hand, the product of two [orthogonal matrices](../../../../../orthogonal-matrix.md) is always an [orthogonal matrix](../../../../../orthogonal-matrix.md):

$$
(AB)^T(AB)=B^TA^TAB=B^TB=I.
$$

Therefore the answers are $\boxed{\text{(i) no; (ii) yes.}}$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
