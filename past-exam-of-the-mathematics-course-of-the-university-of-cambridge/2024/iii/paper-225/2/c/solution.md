<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the null distribution is a [centrally symmetric probability distribution](../../../../../../centrally-symmetric-probability-distribution.md), so $X_i$ and $-X_i$ have the same law. A [sign-flip randomization test](../../../../../../sign-flip-randomization-test.md) draws signs $s_i\in\{-1,1\}$ independently and recomputes, for example,

$$
T(s)=n\left\lVert\frac1n\sum_{i=1}^ns_iX_i\right\rVert^2.
$$

The exact p-value averages over all $2^n$ sign vectors:

$$
p=2^{-n}\#\{s:T(s)\geq T(1,\ldots,1)\}.
$$

With $B$ random sign vectors, including the observed configuration, the standard Monte Carlo version is $(1+\#\{b:T_b\geq T_0\})/(B+1)$, where $T_0$ is the observed statistic. Joint sign invariance under the null makes this finite-sample valid.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
