<h1 id="31l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $x_{1:n}$ put $A_\sigma=\sum_i\sigma_i x_ix_i^T$. Then

$$
\widehat{\mathcal R}(H(x_{1:n}))
=\frac1n\mathbb E_\sigma\sup_{M\succeq0,\operatorname{tr}M\leq s}
\operatorname{tr}(MA_\sigma)
\leq\frac s n\mathbb E_\sigma\lVert A_\sigma\rVert_{\rm op}
\leq\frac s n\mathbb E_\sigma\lVert A_\sigma\rVert_F.
$$

Jensen's inequality and cancellation of cross terms between independent signs give

$$
\mathbb E_\sigma\lVert A_\sigma\rVert_F
\leq\left(\sum_i\operatorname{tr}[(x_ix_i^T)^2]\right)^{1/2}
=\left(\sum_i\lVert x_i\rVert_2^4\right)^{1/2}
\leq C^2\sqrt n.
$$

Therefore

$$
\boxed{\mathcal R_n(H)\leq\frac{C^2s}{\sqrt n}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31L](../../31l.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
