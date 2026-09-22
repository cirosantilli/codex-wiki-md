<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For fixed $p\ge1$, the complement of the [simple matching coefficient](../../../../../../../simple-matching-coefficient.md) is the fraction of coordinates that disagree:

$$
1-S_1(x,y)=\frac1p\sum_{r=1}^p\mathbf1\{x_r\ne y_r\}.
$$

This is the [normalized Hamming distance](../../../../../../../normalized-hamming-distance.md). It is nonnegative, symmetric, and is zero exactly when every coordinate agrees. At each coordinate,

$$
\mathbf1\{x_r\ne z_r\}\le
\mathbf1\{x_r\ne y_r\}+\mathbf1\{y_r\ne z_r\}.
$$

Summing and dividing by $p$ proves the [triangle inequality](../../../../../../../triangle-inequality.md). Therefore **$d_1$ is a [metric](../../../../../../../metric.md)** on the binary vectors.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
