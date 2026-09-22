<h1 id="18h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let

$$
H=X(X^TX)^{-1}X^T
$$

be the [hat matrix](../../../../../../hat-matrix.md). Then

$$
\widehat\beta=(X^TX)^{-1}X^T(HY)
$$

depends only on the orthogonal projection $HY$, while

$$
n\widehat\sigma^2=\|(I-H)Y\|^2
$$

depends only on the orthogonal residual projection $(I-H)Y$.

The random vectors $HY$ and $(I-H)Y$ are jointly [multivariate normal](../../../../../../multivariate-normal-distribution.md), and their cross-covariance is

$$
\sigma^2H(I-H)=0.
$$

Uncorrelated jointly Gaussian vectors are [independent](../../../../../../independent-random-variables.md). Therefore

$$
\boxed{\widehat\beta\ \text{and}\ \widehat\sigma^2
\text{ are independent}}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
