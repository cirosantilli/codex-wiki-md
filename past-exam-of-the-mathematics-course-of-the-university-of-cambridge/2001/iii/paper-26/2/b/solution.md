<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) says that if $X^L$ has a [large deviation principle](../../../../../../large-deviation-principle.md) in $E$ with [good rate function](../../../../../../good-rate-function.md) $I$, and $f:E\to H$ is a [continuous map](../../../../../../continuous-map.md) between [Hausdorff spaces](../../../../../../hausdorff-space.md), then $f(X^L)$ has the same [large-deviation speed](../../../../../../large-deviation-speed.md) and [good rate function](../../../../../../good-rate-function.md)

$$
J(y)=\inf_{f(x)=y}I(x).
$$

For an [open set](../../../../../../open-set.md) $G\subset H$, its inverse image is open, so the input lower bound gives

$$
\liminf_L a_L^{-1}\log\mathbb P(f(X^L)\in G)
\ge-\inf_{f^{-1}(G)}I=-\inf_GJ.
$$

For a [closed set](../../../../../../closed-set.md) $F\subset H$, its inverse image is closed, giving the corresponding upper bound with $-\inf_FJ$.

It remains to prove goodness, including the endpoint issue in the infimum. Each fibre $f^{-1}(\{y\})$ is closed. If $J(y)<\infty$, compact [sublevel sets](../../../../../../sublevel-set.md) and [lower semicontinuity](../../../../../../lower-semicontinuity.md) make $I$ attain its infimum on that fibre: intersect it with the compact set $\{I\le J(y)+1\}$ and use the closed nested sublevels tending down to $J(y)$. Hence for each finite $r$,

$$
\{y:J(y)\le r\}=f(\{x:I(x)\le r\}).
$$

The right-hand side is compact, being a continuous image of a [compact set](../../../../../../compact-space.md), and is closed because the target is [Hausdorff](../../../../../../hausdorff-space.md). Thus $J$ is lower semicontinuous and good, completing the proof.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
