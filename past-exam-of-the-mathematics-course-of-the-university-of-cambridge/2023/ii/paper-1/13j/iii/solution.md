<h1 id="13j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let

$$
\widehat\beta=(X^TX)^{-1}X^TY,
\qquad
\widehat\sigma^2
=\frac{\|Y-X\widehat\beta\|^2}{n-p}.
$$

The pivotal quadratic form has an $F_{p,n-p}$ distribution, so the $(1-\alpha)$ [normal linear-model confidence ellipsoid](../../../../../../normal-linear-model-confidence-ellipsoid.md) is

$$
\boxed{
\left\{b\in\mathbb R^p:
\frac{(b-\widehat\beta)^TX^TX(b-\widehat\beta)}
 {p\widehat\sigma^2}
\leq F_{p,n-p}(1-\alpha)
\right\}
}.
$$

Here $F_{p,n-p}(1-\alpha)$ is the $(1-\alpha)$ quantile of the indicated $F$ distribution.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
