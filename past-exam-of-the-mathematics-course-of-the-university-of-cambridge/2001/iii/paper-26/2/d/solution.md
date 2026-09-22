<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the standard [Hausdorff](../../../../../../hausdorff-space.md) state-space convention, so compact sets are closed. Let $F$ be any [closed set](../../../../../../closed-set.md) and choose $K_M$ from [exponential tightness](../../../../../../exponential-tightness.md). The [weak large deviation principle](../../../../../../weak-large-deviation-principle.md) applies to the compact set $F\cap K_M$, while

$$
\mathbb P(X^L\in F)\le\mathbb P(X^L\in F\cap K_M)+\mathbb P(X^L\notin K_M).
$$

The [principle of the largest exponential term](../../../../../../principle-of-the-largest-exponential-term.md) gives

$$
\limsup_La_L^{-1}\log\mathbb P(X^L\in F)
\le\max\{-\inf_{F\cap K_M}I,-M\}
\le\max\{-\inf_FI,-M\}.
$$

Let $M\to\infty$. This is the full closed-set upper bound; the open-set lower bound was already present.

For goodness, fix $r<\infty$ and choose $M>r$. The complement $K_M^c$ is open. Its lower bound and its exponential-tightness upper estimate imply

$$
-\inf_{K_M^c}I
\le\liminf_La_L^{-1}\log\mathbb P(X^L\notin K_M)
\le-M.
$$

Thus $\inf_{K_M^c}I\ge M$ and $\{I\le r\}\subset K_M$. Lower semicontinuity makes this [sublevel set](../../../../../../sublevel-set.md) closed, so it is a closed subset of a compact set and therefore compact. This proves that [exponential tightness upgrades a weak large deviation principle](../../../../../../exponential-tightness-upgrades-a-weak-large-deviation-principle.md) to the full principle with the same [good rate function](../../../../../../good-rate-function.md).

## ↑ Ancestors (11)

1. [D](../d.md)
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
