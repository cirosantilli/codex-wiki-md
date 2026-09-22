<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First suppose $A=P+N$, with $P$ a real [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md) and $N$ a symmetric [nonnegative matrix](../../../../../../nonnegative-matrix.md). Factor $P=B^TB$, and write $v(z)=(z_1^2,\ldots,z_n^2)^T$. Then

$$
p(z)=\|Bv(z)\|^2+\sum_i N_{ii}(z_i^2)^2+\sum_{i<j}2N_{ij}(z_iz_j)^2.
$$

Each term is a square multiplied by a nonnegative scalar, so $p$ is a [sum of squares polynomial](../../../../../../polynomial-sos.md).

Conversely, suppose $p=\sum_\ell q_\ell^2$. Because $p$ is a degree-four [homogeneous polynomial](../../../../../../homogeneous-polynomial.md), the [homogeneous sum of squares representation](../../../../../../homogeneous-sum-of-squares-representation.md) allows every $q_\ell$ to be quadratic and homogeneous. Explicitly, higher-degree parts cannot cancel in a sum of squares; constant parts vanish because $p(0)=0$, and the degree-two part $\sum_\ell(q_\ell^{(1)})^2$ forces all linear parts to vanish. Write

$$
q_\ell(z)=\sum_i a_{\ell i}z_i^2+\sum_{i<j}b_{\ell ij}z_iz_j.
$$

Since $p$ is invariant under every coordinate sign change, [sign averaging of a sum of squares](../../../../../../sign-averaging-of-a-sum-of-squares.md) over independent [Rademacher random variables](../../../../../../rademacher-distribution.md) gives

$$
p(z)=\sum_\ell\left(\sum_i a_{\ell i}z_i^2\right)^2
+\sum_{i<j}\left(\sum_\ell b_{\ell ij}^2\right)z_i^2z_j^2.
$$

The cross terms vanish because their sign products contain an [odd](../../../../../../odd-function.md) power of at least one independent sign. Set

$$
P=\sum_\ell a_\ell a_\ell^T,\qquad N_{ii}=0,\qquad N_{ij}=N_{ji}=\frac12\sum_\ell b_{\ell ij}^2\quad(i<j).
$$

Then $P$ is a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md) and $N$ is a symmetric [nonnegative matrix](../../../../../../nonnegative-matrix.md). Comparing the coefficients of $z_i^4$ and $z_i^2z_j^2$ gives $A=P+N$. This proves the [sum of squares criterion for a biquadratic form](../../../../../../sum-of-squares-criterion-for-a-biquadratic-form.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
