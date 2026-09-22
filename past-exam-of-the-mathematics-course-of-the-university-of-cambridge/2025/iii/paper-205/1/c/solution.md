<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The differentiable loss has gradient $X^T(X\beta-Y)/n$. The [subdifferential sum rule](../../../../../../subdifferential-sum-rule.md) and part (b) give

$$
\partial Q(\beta)=\frac1nX^T(X\beta-Y)+\lambda\sqrt m\,u,
$$

where blockwise

$$
\boxed{u^{(k)}=\frac{\beta^{(k)}}{\lVert\beta^{(k)}\rVert_2}
\quad\text{if }\beta^{(k)}\ne0,
\qquad
\lVert u^{(k)}\rVert_2\leq1
\quad\text{if }\beta^{(k)}=0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
