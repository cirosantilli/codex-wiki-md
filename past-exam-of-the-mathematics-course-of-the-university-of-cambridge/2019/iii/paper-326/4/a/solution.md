<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a convex functional $J$ and $p\in\partial J(v)$, the [generalized Bregman distance](../../../../../../bregman-divergence.md) is

$$
\boxed{D_J^p(u,v)=J(u)-J(v)-\langle p,u-v\rangle\geq0.}
$$

The inequality is exactly the [subgradient inequality](../../../../../../subgradient-inequality.md).

Suppose $J$ is [strictly convex](../../../../../../strictly-convex-function.md) and $u\ne v$, with both values finite. If the distance vanished, the supporting affine function at $v$ would also meet $J$ at $u$. At $w=(1-t)v+tu$, $0<t<1$, the subgradient inequality would give

$$
J(w)\geq J(v)+t\langle p,u-v\rangle
=(1-t)J(v)+tJ(u),
$$

contradicting strict convexity. Hence zero distance implies $u=v$.

Without strict convexity, take $J(s)=|s|$, $v=1$, and $p=1\in\partial J(1)$. For every $u\geq0$,

$$
D_J^1(u,1)=u-1-(u-1)=0,
$$

including $u=2\ne1$. Thus **zero Bregman distance need not identify a point**. It identifies points on the same supporting face, as explained by [zero Bregman distance and supporting faces](../../../../../../zero-bregman-distance-and-supporting-faces.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
