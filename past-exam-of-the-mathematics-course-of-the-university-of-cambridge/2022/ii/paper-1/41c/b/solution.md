<h1 id="41c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $A$ is [symmetric positive definite](../../../../../../hermitian-positive-definite-matrix.md),

$$
\nabla f(x)=Ax-b,\qquad \nabla^2f(x)=A\succ0.
$$

Thus the only stationary point is $x_*=A^{-1}b$, and

$$
f(x)=f(x_*)+\frac12(x-x_*)^TA(x-x_*).
$$

The final term is positive unless $x=x_*$, proving that $A^{-1}b$ is the unique minimizer.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [41C](../../41c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
