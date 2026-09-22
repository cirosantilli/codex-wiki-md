<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The printed values appear to favor model 2 because $-12.529<336.381$. They are not directly comparable: model 2 reports the Gaussian likelihood of $Z_i=\log T_i$, whereas model 3 reports a density for $T_i$. The [change-of-variables formula for a probability density](../../../../../../change-of-variables-formula-for-a-probability-density.md) gives

$$
\ell_T=\ell_Z-\sum_{i=1}^{35}\log T_i,
$$

so the transformed model's AIC on the original response scale is

$$
\operatorname{AIC}_{2,T}
=\operatorname{AIC}_{2,Z}+2\sum_i\log T_i.
$$

Because the standardized predictors have zero sample means and the ordinary-least-squares residuals sum to zero,

$$
\sum_i\log T_i=35\widehat\alpha_0=35(4.99902).
$$

Therefore

$$
\operatorname{AIC}_{2,T}
=-12.52943+70(4.99902)=337.402,
$$

which is slightly worse than model 3's $336.381$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
