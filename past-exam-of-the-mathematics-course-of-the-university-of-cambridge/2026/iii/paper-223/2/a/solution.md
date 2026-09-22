<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For residual $r=y_i-x_i^\top\theta$, minimize

$$
\frac{(r-\gamma)^2}{2\sigma}+k|\gamma|
$$

over $\gamma$. [Soft thresholding](../../../../../../soft-thresholding.md) gives $\widehat\gamma=\operatorname{sgn}(r)(|r|-k\sigma)_+$, and the minimized value is

$$
\begin{cases}
r^2/(2\sigma),&|r|\leq k\sigma,\\
k|r|-k^2\sigma/2,&|r|>k\sigma.
\end{cases}
$$

This is $\sigma\rho_k(r/\sigma)$ for the usual [Huber loss](../../../../../../huber-loss.md). Multiplication by the positive constant $\sigma$ does not change the minimizing $\theta$, proving equivalence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
