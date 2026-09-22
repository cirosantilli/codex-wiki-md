<h1 id="10g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem.md) states that every square complex [matrix](../../../../../../matrix.md) satisfies its own [characteristic polynomial](../../../../../../characteristic-polynomial.md): if $\chi_A(t)=\det(tI-A)=t^n+c_{n-1}t^{n-1}+\cdots+c_0$, then

$$
\boxed{A^n+c_{n-1}A^{n-1}+\cdots+c_0I=0.}
$$

For a proof, expand the [adjugate matrix](../../../../../../adjugate-matrix.md) as $\operatorname{adj}(tI-A)=\sum_{k=0}^{n-1}B_kt^k$. The [adjugate identity](../../../../../../adjugate-identity.md) gives

$$
(tI-A)\sum_{k=0}^{n-1}B_kt^k=\chi_A(t)I.
$$

Comparing coefficients yields $-AB_0=c_0I$, $B_{k-1}-AB_k=c_kI$ for $1\le k\le n-1$, and $B_{n-1}=I$. Multiply the middle identities on the left by $A^k$, include the first identity, and add $A^nB_{n-1}=A^n$. The terms involving the $B_k$ cancel consecutively:

$$
-AB_0+\sum_{k=1}^{n-1}(A^kB_{k-1}-A^{k+1}B_k)+A^nB_{n-1}=0.
$$

Their right sides sum to $c_0I+\sum_{k=1}^{n-1}c_kA^k+A^n$. This proves the theorem without any substitution of noncommuting [matrices](../../../../../../matrix.md) into a scalar [polynomial](../../../../../../polynomial-split.md) identity.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10G](../../10g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
