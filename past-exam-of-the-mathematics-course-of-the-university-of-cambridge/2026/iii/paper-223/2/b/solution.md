<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed residual $r=y_i-x_i^\top\theta$, choosing $\gamma_i=0$ costs $r^2$, while choosing $\gamma_i=r$ costs $\ell$. No other nonzero choice improves on $\gamma_i=r$. Thus

$$
\inf_{\gamma_i}\{(r-\gamma_i)^2+\ell\mathbf1_{\{\gamma_i\ne0\}}\}
=\min(r^2,\ell)=\rho_L(r)
$$

with $L=\sqrt\ell$. Summing over observations proves the equivalence.

## ↑ Ancestors (11)

1. [B](../b.md)
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
