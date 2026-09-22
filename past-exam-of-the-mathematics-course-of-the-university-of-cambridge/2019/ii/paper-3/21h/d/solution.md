<h1 id="21h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $x,y\in\ell^2$ satisfy $\lVert x\rVert_2=\lVert y\rVert_2=1$. The [parallelogram law](../../../../../../parallelogram-law.md) gives

$$
\left\lVert\frac{x+y}{2}\right\rVert_2^2
+\left\lVert\frac{x-y}{2}\right\rVert_2^2
=\frac{\lVert x\rVert_2^2+\lVert y\rVert_2^2}{2}=1.
$$

If $\lVert x-y\rVert_2\geq\varepsilon$, then

$$
\left\lVert\frac{x+y}{2}\right\rVert_2^2
\leq1-\frac{\varepsilon^2}{4},
$$

and therefore

$$
\left\lVert\frac{x+y}{2}\right\rVert_2
\leq\sqrt{1-\frac{\varepsilon^2}{4}}
=1-\delta,
\qquad
\boxed{\delta=1-\sqrt{1-\varepsilon^2/4}>0.}
$$

This depends only on $\varepsilon$, so the [l2 sequence space](../../../../../../l2-sequence-space.md) is a [uniformly convex Banach space](../../../../../../uniformly-convex-banach-space.md), as asserted by the [uniform convexity of l2](../../../../../../uniform-convexity-of-l2.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
