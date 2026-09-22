<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

The [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md) states that every square matrix satisfies its [characteristic polynomial](../../../../../characteristic-polynomial.md): if $\chi_A(t)=\det(tI-A)$, then $\chi_A(A)=0$.

For the proof, the [adjugate identity](../../../../../adjugate-identity.md) gives

$$
(tI-A)\operatorname{adj}(tI-A)=\chi_A(t)I.
$$

Write $\operatorname{adj}(tI-A)=B_0+B_1t+\cdots+B_{n-1}t^{n-1}$ and compare coefficients. Multiplying the resulting recurrence by successive powers of $A$ and summing telescopically yields $\chi_A(A)=0$.

By [polynomial division](../../../../../polynomial-division.md), $p=q\chi_A+r$ with $\deg r<n$. Therefore $p(A)=r(A)$ by Cayley-Hamilton, while $p(\lambda)=r(\lambda)$ for every [eigenvalue](../../../../../eigenvalue.md) $\lambda$, since $\chi_A(\lambda)=0$.

For the displayed matrix,

$$
\chi_A(t)=(t-2)(t^2+1).
$$

The remainder of $t^{1000}$ modulo this polynomial has the form $at^2+c$, because its values at $i$ and $-i$ are both $1$. The equations $-a+c=1$ and $4a+c=2^{1000}$ give

$$
r(t)=\frac{2^{1000}-1}{5}t^2+\frac{2^{1000}+4}{5}.
$$

Since $(A^2)_{11}=3$, the requested entry is

$$
\boxed{(A^{1000})_{11}=\frac{4\cdot2^{1000}+1}{5}.}
$$

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
