<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a finite $r\geq0$ and choose $M>r$. By [exponential tightness](../../../../../../exponential-tightness.md), choose a [compact set](../../../../../../compact-space.md) $K_M$ with outside probability having upper exponential rate strictly below $-M$. A [compact set](../../../../../../compact-space.md) in a [Hausdorff space](../../../../../../hausdorff-space.md) is closed, so its complement is an [open set](../../../../../../open-set.md). The lower bound of the [weak large deviation principle](../../../../../../weak-large-deviation-principle.md) gives

$$
-\inf_{x\notin K_M}I(x)
\leq\liminf_L\frac1L\log\mathbb P(X_L\notin K_M)
\leq\limsup_L\frac1L\log\mathbb P(X_L\notin K_M)<-M.
$$

Consequently $\inf_{K_M^c}I>M$, and $\{I\leq r\}\subset K_M$. [Lower semicontinuity](../../../../../../lower-semicontinuity.md) makes this [sublevel set](../../../../../../sublevel-set.md) closed in $E$, hence a closed subset of a [compact set](../../../../../../compact-space.md). Thus it is [compact](../../../../../../compact-space.md). **Every finite sublevel set is compact, so $I$ is a good rate function.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
