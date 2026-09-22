<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) to write $X^*=V\Lambda V^T$, with $V$ orthogonal and $\Lambda$ diagonal and nonnegative. For any sign vector, $\xi_j^2=1$, so

$$
\|\widehat x(\xi)\|_2^2=\xi^T\Lambda\xi=\sum_j\lambda_j=\operatorname{tr}X^*.
$$

This is an exact identity for every sign choice. Put $M(\xi)=\max_i|a_i^T\widehat x(\xi)|$. When $M>0$, the [Rademacher rounding for a semidefinite relaxation](../../../../../../rademacher-rounding-for-a-semidefinite-relaxation.md) gives

$$
|a_i^Tx(\xi)|=\frac{|a_i^T\widehat x(\xi)|}{M}\le1,\qquad
\boxed{\|x(\xi)\|_2^2=\frac{\operatorname{tr}X^*}{M(\xi)^2}.}
$$

Hence $x(\xi)$ is feasible. In the finite spanning case from part (a), $\operatorname{tr}X^*>0$ makes $\widehat x\ne0$, and the spanning condition then gives $M>0$. If a nonzero $\widehat x$ instead had $M=0$, it would be an unbounded feasible direction rather than a vector to divide by zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
