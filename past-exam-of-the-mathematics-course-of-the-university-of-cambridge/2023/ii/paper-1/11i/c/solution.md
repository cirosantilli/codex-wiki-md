<h1 id="11i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Every row of the channel matrix is a permutation of $(1-2\alpha,\alpha,\alpha)$, and every column sum is one. It is therefore a weakly symmetric channel. The uniform input makes the output uniform, with entropy $\log_2 3$, while the conditional output entropy is the entropy of one row:

$$
H(Y\mid X)
=-(1-2\alpha)\log_2(1-2\alpha)
 -2\alpha\log_2\alpha.
$$

The [weakly symmetric channel capacity](../../../../../../weakly-symmetric-channel-capacity.md) formula now gives the [ternary symmetric channel capacity](../../../../../../ternary-symmetric-channel-capacity.md)

$$
\boxed{
C=\log_2 3
 +(1-2\alpha)\log_2(1-2\alpha)
 +2\alpha\log_2\alpha
}
$$

bits per channel use, for $0\leq\alpha\leq1/2$, with the convention $0\log_2 0=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11I](../../11i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
