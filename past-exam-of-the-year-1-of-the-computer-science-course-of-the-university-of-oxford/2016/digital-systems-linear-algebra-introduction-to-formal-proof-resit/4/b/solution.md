<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Gram-Schmidt process](../../../../../gram-schmidt-process.md) constructs the vectors in order:

$$
v_j=x_j-\sum_{i<j}\langle q_i,x_j\rangle q_i,\qquad q_j=\frac{v_j}{\lVert v_j\rVert},\qquad j=1,\ldots,k.
$$

The empty sum at $j=1$ is zero. Each subtraction removes the projection onto one previous [unit vector](../../../../../unit-vector.md), so $v_j$ is orthogonal to their span. [Linear independence](../../../../../linear-independence.md) of the inputs ensures $v_j\ne0$ in exact arithmetic, and normalization gives unit length.

In [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md), subtracting nearly equal projections can amplify roundoff and cause loss of orthogonality, especially for nearly dependent columns. [Modified Gram-Schmidt](../../../../../modified-gram-schmidt.md), reorthogonalization, or [Householder QR factorization](../../../../../householder-qr-decomposition.md) can improve numerical behaviour; no implementation can remove the underlying sensitivity of nearly dependent input data.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
