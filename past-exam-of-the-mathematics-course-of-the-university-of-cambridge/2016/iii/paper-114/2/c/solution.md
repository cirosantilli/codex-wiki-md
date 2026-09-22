<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $A=\Sigma_h^\partial$. This [surface with boundary](../../../../../../surface-with-boundary.md) deformation retracts onto a wedge of $2h$ circles, so $H^1(A;\mathbb R)$ has dimension $2h$ and $H^2(A;\mathbb R)=0$. If $r$ were a [retraction](../../../../../../retraction.md), $\iota^*r^*=\mathrm{id}$ would make $r^*$ injective. Its image $W\subset H^1(\Sigma_g;\mathbb R)$ would have dimension $2h$.

Every pair of classes $u,v$ in $H^1(A;\mathbb R)$ has $u\smile v=0$, since $H^2(A;\mathbb R)=0$. Naturality gives

$$
r^*u\smile r^*v=r^*(u\smile v)=0.
$$

Thus $W$ is an [isotropic subspace of a symplectic vector space](../../../../../../isotropic-subspace-of-a-symplectic-vector-space.md) for the nondegenerate skew [Poincare duality pairing](../../../../../../poincare-duality-pairing.md) on the $2g$-dimensional space $H^1(\Sigma_g;\mathbb R)$. The stated linear-algebra bound gives $2h\leq g$. Hence

$$
\boxed{h>g/2\quad\Longrightarrow\quad\text{no retraction exists}.}
$$

**The bound is sharp.** Double $A$ along its boundary: $D(A)=A\cup_{\partial A}A$ is the closed oriented surface of genus $2h$. Identify each copy with $A$ and fold them onto one copy. The two maps agree on the joining circle, so they give a continuous [retraction](../../../../../../retraction.md) fixing the first copy pointwise. This includes $h=0$, where the double of a disc is a sphere.

More generally, for $g\geq2h$, add $g-2h$ handles in the interior of the second copy. Pinch those extra handles onto their connecting point, keeping the boundary fixed, and then fold onto $A$. This is still a [retraction](../../../../../../retraction.md). In fact the construction works for any embedding in the question: the connected complement has one boundary component and genus $g-h$ by Euler-characteristic additivity, and the [classification theorem for surfaces](../../../../../../classification-theorem-for-surfaces.md) identifies it, relative to that boundary, with a copy of $A$ having $g-2h$ additional handles. Thus the exact existence criterion is $2h\leq g$, as expressed by [retraction onto a punctured oriented surface](../../../../../../retraction-onto-a-punctured-oriented-surface.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
