<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In the [finite field](../../../../../finite-field.md) $\mathbb F_5=\mathbb Z/5\mathbb Z$, the [characteristic polynomial](../../../../../characteristic-polynomial.md) becomes

$$
\chi_A(\lambda)=(\lambda-1)(\lambda-3)^2,
$$

because $(\lambda-3)^2=\lambda^2-\lambda-1$ modulo $5$. Splitting into linear factors does not by itself guarantee [diagonalizability](../../../../../diagonalizable-matrix.md): the repeated [eigenvalue](../../../../../eigenvalue.md) needs enough [eigenvectors](../../../../../eigenvector.md).

Solving $(A-3I)(x,y,z)^T=0$ gives

$$
2x+y=0,\qquad x+3y=0,\qquad y+3z=0,
$$

so $y=3x$ and $z=4x$. Hence

$$
\ker(A-3I)=\operatorname{span}_{\mathbb F_5}\{(1,3,4)^T\}
$$

has [dimension](../../../../../dimension-vector-space.md) one, although $3$ has [algebraic multiplicity](../../../../../algebraic-multiplicity.md) two. The [geometric multiplicity](../../../../../geometric-multiplicity.md) is too small, and **$A$ is not diagonalizable over $\mathbb F_5$**. This illustrates [diagonalizability depends on the field](../../../../../diagonalizability-depends-on-the-field.md): characteristic zero gave three distinct [eigenvalues](../../../../../eigenvalue.md), while reduction modulo $5$ merges two of them.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
