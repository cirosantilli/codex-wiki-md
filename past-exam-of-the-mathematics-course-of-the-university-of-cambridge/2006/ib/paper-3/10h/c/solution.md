<h1 id="10h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the permitted triangularization to write $A=TUT^{-1}$ with $U$ upper triangular and diagonal $\lambda_1,\ldots,\lambda_n$. Products of upper-triangular [matrices](../../../../../../matrix.md) are upper triangular, and their diagonal entries multiply, so

$$
0=\operatorname{tr}(A^k)=\operatorname{tr}(U^k)=\sum_{j=1}^n\lambda_j^k
\qquad(1\le k\le n).
$$

The result of part b makes every $\lambda_j$ zero. Thus $U$ is strictly upper triangular. To see directly that $U^n=0$, a potentially nonzero entry in a product of $n$ factors requires a chain

$$
i=i_0<i_1<\cdots<i_n=j
$$

of $n+1$ indices in $\{1,\ldots,n\}$, which is impossible. Hence

$$
\boxed{A^n=TU^nT^{-1}=0.}
$$

This is [nilpotence from vanishing traces of powers](../../../../../../nilpotence-from-vanishing-traces-of-powers.md). It proves nilpotence without substituting an unproved diagonalization for the allowed triangularization.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10H](../../10h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
