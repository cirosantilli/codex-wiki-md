<h1 id="7b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem.md) says that every square complex matrix satisfies its own [characteristic polynomial](../../../../../../characteristic-polynomial.md): if $\chi_A(t)=t^n+c_{n-1}t^{n-1}+\cdots+c_0$, then

$$
\boxed{\chi_A(A)=A^n+c_{n-1}A^{n-1}+\cdots+c_0I=0.}
$$

For a $2\times2$ [diagonalisable matrix](../../../../../../diagonalizable-matrix.md), write $A=SDS^{-1}$ with $D=\operatorname{diag}(\lambda_1,\lambda_2)$. The [characteristic polynomial](../../../../../../characteristic-polynomial.md) is $(t-\lambda_1)(t-\lambda_2)$, including repeated roots. Evaluating it at $D$ gives zero in each diagonal position, and polynomial evaluation respects [matrix similarity](../../../../../../matrix-similarity.md): $\chi_A(A)=S\chi_A(D)S^{-1}=0$. This proves the requested case.

For the final assertion, let $\lambda$ be any complex [eigenvalue](../../../../../../eigenvalue.md) of $B$, with nonzero [eigenvector](../../../../../../eigenvector.md) $\mathbf v$. From $B^k=0$ we obtain $0=B^k\mathbf v=\lambda^k\mathbf v$, so $\lambda=0$. The [characteristic polynomial](../../../../../../characteristic-polynomial.md) of this [nilpotent linear map](../../../../../../nilpotent-linear-map.md) is therefore $t^n$. Applying the full [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem.md) yields **$\boxed{B^n=0}$**. This argument does not assume $B$ is diagonalisable.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
