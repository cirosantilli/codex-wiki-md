<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $0<\sigma^2<\infty$, the [central limit theorem](../../../../../central-limit-theorem.md) gives

$$
\sqrt n(\overline X-\mu)\xrightarrow dN(0,\sigma^2).
$$

If $g$ is differentiable at $\mu$, the [delta method](../../../../../delta-method.md) applies to the first-order expansion

$$
g(\overline X)-g(\mu)=g'(\mu)(\overline X-\mu)+o_p(n^{-1/2}),
$$

where the remainder notation means that its product with $\sqrt n$ tends to zero in [probability](../../../../../probability.md). Hence

$$
\boxed{\sqrt n\{g(\overline X)-g(\mu)\}\xrightarrow dN\!\left(0,\sigma^2[g'(\mu)]^2\right),\qquad
g(\overline X)\mathrel{\dot\sim}N\!\left(g(\mu),\frac{\sigma^2[g'(\mu)]^2}{n}\right).}
$$

The useful nondegenerate [normal approximation](../../../../../normal-approximation.md) requires $g'(\mu)\ne0$. When $g'(\mu)=0$, the first-order limit is zero and a higher-order expansion may be needed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
