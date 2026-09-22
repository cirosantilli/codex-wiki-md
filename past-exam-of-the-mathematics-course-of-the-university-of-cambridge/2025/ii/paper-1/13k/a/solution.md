<h1 id="13k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Conditionally on $X$, the log likelihood differs from

$$
-\frac1{2\sigma^2}(Y-X\beta)^T\Sigma^{-1}(Y-X\beta)
$$

only by terms independent of $\beta$. [Differentiation](../../../../../../differentiation.md) gives the weighted normal equations

$$
X^T\Sigma^{-1}X\widehat\beta=X^T\Sigma^{-1}Y,
$$

and therefore

$$
\boxed{\widehat\beta(\Sigma)=(X^T\Sigma^{-1}X)^{-1}X^T\Sigma^{-1}Y.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13K](../../13k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
