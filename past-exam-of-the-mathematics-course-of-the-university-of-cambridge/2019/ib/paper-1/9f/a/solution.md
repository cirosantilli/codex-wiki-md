<h1 id="9f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [adjugate matrix](../../../../../../adjugate-matrix.md) is the transpose of the cofactor matrix, and it satisfies

$$
M\operatorname{adj}(M)=\operatorname{adj}(M)M=(\det M)I.
$$

Put $M=tI-A$ and substitute the two given expansions into this identity:

$$
(tI-A)\sum_{i=0}^{n-1}B_it^{n-1-i}
=\sum_{j=0}^nc_jt^{n-j}I.
$$

Comparing coefficients of powers of $t$ gives

$$
\boxed{B_0=c_0I=I,
\qquad B_i=AB_{i-1}+c_iI\quad(1\leq i\leq n-1),
\qquad -AB_{n-1}=c_nI}.
$$

Here $c_0=1$ because the [characteristic polynomial](../../../../../../characteristic-polynomial.md) is monic.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
