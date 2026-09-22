<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [matrix exponential](../../../../../../../matrix-exponential.md) is the absolutely convergent power series

$$
\boxed{B(t)=e^{Lt}=\sum_{m=0}^\infty\frac{t^mL^m}{m!}.}
$$

It converges in any finite-dimensional [operator norm](../../../../../../../operator-norm.md), since $\|L^m\|\le\|L\|^m$. Termwise differentiation gives $B'=LB$, $B(0)=I$, so the solution is $q(t)=B(t)q_0$. Also $e^{Lt}e^{-Lt}=I$, proving invertibility without requiring $L$ itself to be invertible.

The question's expansion in eigenvectors tacitly needs an eigenbasis: an invertible matrix alone need not be a [diagonalizable matrix](../../../../../../../diagonalizable-matrix.md). The exponential solution and the singular-value arguments remain valid without that assumption.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
