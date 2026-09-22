<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [strictly convex normed space](../../../../../../strictly-convex-normed-space.md) is a [normed vector space](../../../../../../normed-vector-space.md) whose unit sphere contains no nontrivial line segment. Equivalently, for distinct unit vectors $x,y$,

$$
\left\|\frac{x+y}{2}\right\|<1.
$$

Suppose $u,v\in U$ are both elements of [best approximation in a normed space](../../../../../../best-approximation-in-a-normed-space.md) to $f$, and let $d=\inf_{w\in U}\|f-w\|$. If $d=0$ then $u=v=f$. If $d>0$ and $u\ne v$, the vectors $(f-u)/d$ and $(f-v)/d$ are distinct unit vectors. Strict convexity gives

$$
\left\|f-\frac{u+v}{2}\right\|
=d\left\|\frac{(f-u)/d+(f-v)/d}{2}\right\|<d.
$$

But $(u+v)/2\in U$, contradicting the definition of $d$. Thus **there is at most one best approximant**. This proves [uniqueness of best approximation in a strictly convex space](../../../../../../uniqueness-of-best-approximation-in-a-strictly-convex-space.md), and does not assert existence for an arbitrary, possibly nonclosed, [linear subspace](../../../../../../vector-subspace.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
