<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $z=\widehat\beta_{\mathrm{OLS}}=X^TY/n$. Under $X^TX=nI_p$, the objective separates by coordinates. Completing the square and applying the [soft-thresholding operator](../../../../../../soft-thresholding.md) $S(u,t)=\operatorname{sign}(u)(|u|-t)_+$ gives

$$
(\widehat\beta_{\alpha,\lambda})_j
=\frac{S(z_j,\lambda\alpha)}{1+\lambda(1-\alpha)}.
$$

For a fixed $z_j$, its magnitude lies between the ridge endpoint $|z_j|/(1+\lambda)$ and the lasso endpoint $(|z_j|-\lambda)_+$; this follows directly on the two intervals $\lambda\alpha\geq|z_j|$ and $\lambda\alpha<|z_j|$ by cross-multiplication. Thus the stated endpoint inequality holds.

For $alpha>0$ and $z_j\ne0$, the coordinate first vanishes when the soft threshold reaches $|z_j|$, so

$$
(\lambda_α^*)_j=\frac{|z_j|}{\alpha}.
$$

This is strictly decreasing in $\alpha$, and it diverges to infinity as $\alpha\downarrow0$. This agrees with the fact that pure ridge shrinkage does not set a nonzero coordinate exactly to zero at any finite penalty.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
