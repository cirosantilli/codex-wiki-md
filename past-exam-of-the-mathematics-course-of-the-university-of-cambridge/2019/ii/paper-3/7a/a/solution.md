<h1 id="7a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Differentiating under the [contour integration](../../../../../../contour-integration.md) sign gives

$$
zw''+w=\int_\gamma e^{zt}\bigl(zt^2f(t)+f(t)\bigr)\,dt.
$$

Since $\partial_t e^{zt}=ze^{zt}$, [integration by parts](../../../../../../integration-by-parts.md) turns this into

$$
\left[e^{zt}t^2f(t)\right]_{\partial\gamma}
+\int_\gamma e^{zt}\left[f(t)-\frac{d}{dt}\bigl(t^2f(t)\bigr)\right]dt.
$$

The integral vanishes when

$$
(t^2f)'=f,
\qquad
\frac{f'}f=\frac1{t^2}-\frac2t.
$$

Hence, up to an irrelevant multiplicative constant,

$$
\boxed{f(t)=t^{-2}e^{-1/t}.}
$$

The remaining endpoint condition is

$$
\boxed{\left[e^{zt-1/t}\right]_{\partial\gamma}=0.}
$$

**Thus each open end of $\gamma$ must lie where $\operatorname{Re}(zt-1/t)\to-\infty$; a closed contour also makes the boundary term vanish when the integrand is single-valued along it.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7A](../../7a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
