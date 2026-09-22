<h1 id="4/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $S=\sigma^2+\tau^2$. For one posterior draw, the Gaussian quadratic-exponential moment is finite precisely when $\tau<\sigma$, and then

$$
\mathbb E_{\theta\mid y}[p(y\mid\theta)^{-2}]
=2\pi\sigma^2\sqrt{\frac{S}{\sigma^2-\tau^2}}
\exp\!\left[
\frac{\sigma^2y^2}{S(\sigma^2-\tau^2)}
\right].
$$

Because the $m$ posterior draws are independent,

$$
\operatorname{Var}_{\theta\mid y}(\widehat I)
=\frac{2\pi}{m}\left[
\sigma^2\sqrt{\frac{S}{\sigma^2-\tau^2}}
\exp\!\left\{\frac{\sigma^2y^2}{S(\sigma^2-\tau^2)}\right\}
-S\exp\!\left\{\frac{y^2}{S}\right\}
\right].
$$

For $\tau\geq\sigma$ the second moment, and hence the variance, is infinite. The [Harmonic mean estimator of Bayesian model evidence](../../../../../../../harmonic-mean-estimator-of-bayesian-model-evidence.md) is therefore unstable in the usual diffuse-prior regime: posterior sampling does not adequately control the reciprocal likelihood in the posterior tails.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 219](../../../../paper-219-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
