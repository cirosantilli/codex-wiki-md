<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume spherical fragments of the common [mass density](../../../../../../density.md) $\rho$, and let $n(D)=KD^{-\alpha}$ count fragments per unit diameter. [Mass normalization of a power-law size distribution](../../../../../../mass-normalization-of-a-power-law-size-distribution.md) gives

$$
m=\frac{\pi\rho K}{6}\frac{D_{\max}^{4-\alpha}-D_{\min}^{4-\alpha}}{4-\alpha}.
$$

Their [geometric cross-sections](../../../../../../geometric-collision-cross-section.md) are $\pi D^2/4$, hence the [cross-section of a power-law fragment population](../../../../../../cross-section-of-a-power-law-fragment-population.md) is exactly

$$
\sigma_{\rm tot}=\frac{3m}{2\rho}\frac{4-\alpha}{\alpha-3}
\frac{D_{\min}^{3-\alpha}-D_{\max}^{3-\alpha}}{D_{\max}^{4-\alpha}-D_{\min}^{4-\alpha}}.
$$

For $3<\alpha<4$, large fragments dominate the [mass](../../../../../../mass.md) integral and small fragments dominate the [geometric cross-section](../../../../../../geometric-collision-cross-section.md) integral. Neglecting the subdominant endpoints gives

$$
\boxed{\sigma_{\rm tot}\simeq\frac{3(4-\alpha)m}{2(\alpha-3)\rho}
D_{\min}^{3-\alpha}D_{\max}^{\alpha-4}}.
$$

The two actual error parameters are $(D_{\min}/D_{\max})^{\alpha-3}$ and $(D_{\min}/D_{\max})^{4-\alpha}$. They must both be small; the approximation is not uniform as $\alpha$ approaches either endpoint. At $\alpha=3$ or $4$ the corresponding integral is logarithmic, so the endpoint-dominated formula must be replaced by that integral.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
