<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Consider the subset

$$
A=\{x\in M:f_1(x)=f_2(x),\ (df_1)_x=(df_2)_x\}.
$$

It is nonempty by the given initial data. A [local isometry](../../../../../../local-isometry.md) preserves the [Levi-Civita connection](../../../../../../levi-civita-connection.md) and therefore affinely parametrized [geodesics](../../../../../../geodesic.md). On a sufficiently small [normal neighborhood](../../../../../../normal-neighbourhood.md) of $x\in A$, this gives

$$
f_i(\exp_xv)=\exp_{f_i(x)}((df_i)_xv).
$$

The right sides agree, so $f_1=f_2$ on that neighborhood and their [differentials](../../../../../../differential-of-a-smooth-map.md) agree there as well. Consequently $A$ is [open](../../../../../../open-set.md).

It is also [closed](../../../../../../closed-set.md). If $x_j\in A$ converges to $x$, continuity first gives $f_1(x)=f_2(x)$. Choose coordinate charts around $x$ and this common image. The coordinate matrices of the two [differentials](../../../../../../differential-of-a-smooth-map.md) depend continuously on the base point; their equalities at $x_j$ therefore pass to $x$. Thus $x\in A$. Since $M$ is [connected](../../../../../../connected-space.md), the nonempty subset $A$ that is both open and closed equals $M$. Hence **$f_1=f_2$ everywhere**. This proves [local isometries are determined by first-order data](../../../../../../local-isometries-are-determined-by-first-order-data.md) without requiring completeness.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
