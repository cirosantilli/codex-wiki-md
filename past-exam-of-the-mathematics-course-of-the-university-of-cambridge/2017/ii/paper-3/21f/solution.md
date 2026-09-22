<h1 id="21f/solution">Solution</h1>

↑ **Parent:** [21F](../21f.md)

Set $F(z,w)=w^2-z^n+1$. Its complex [gradient](../../../../../gradient.md) is $(-nz^{n-1},2w)$, never zero on $F=0$: simultaneous zero would give $z=w=0$, which is not on the [curve](../../../../../curve.md). The complex [implicit function theorem](../../../../../implicit-function-theorem.md) therefore gives a one-dimensional complex [manifold](../../../../../topological-manifold.md), hence a [Riemann surface](../../../../../riemann-surfaces.md). Where $w\ne0$ use $z$ as coordinate, and where $z\ne0$ use $w$; the transition maps and both projections are [holomorphic](../../../../../complex-differentiability-at-a-point.md).

For $\pi$, a [ramification point of a holomorphic map](../../../../../ramification-point-of-a-holomorphic-map.md) has $w=0$ and $z=\zeta$ with $\zeta^n=1$. In the coordinate $w$, $z-\zeta=w^2/(n\zeta^{n-1})+O(w^4)$, giving [ramification index](../../../../../ramification-index.md) $2$. Thus there are $n$ such points, and their [branch points](../../../../../branch-point.md) are the $n$th [roots of unity](../../../../../root-of-unity.md).

For $\tau$, a [ramification point of a holomorphic map](../../../../../ramification-point-of-a-holomorphic-map.md) has $z=0,w=\pm i$. In the coordinate $z$, $w-w_0=z^n/(2w_0)+O(z^{2n})$, giving [ramification index](../../../../../ramification-index.md) $n$ at both points and [branch points](../../../../../branch-point.md) $\pm i$.

Write $n=2m$. At infinity set $u=1/z$, $v=w u^m$; then $v^2=1-u^n$. At $u=0$ there are two smooth points, $v=\pm1$, and $u$ is a local coordinate. The extended $\pi$ has a simple pole at each, so neither is ramified. The degree-two [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) for the map to the [Riemann sphere](../../../../../riemann-sphere.md) gives $2g-2=2(-2)+n$, hence

$$
\boxed{g=\frac{n-2}{2}.}
$$

The list for $\tau$ above concerns the original affine [Riemann surface](../../../../../riemann-surfaces.md); on the compactification its poles at the two added points have order $m$ and are additionally ramified if $m>1$.

## ↑ Ancestors (10)

1. [21F](../21f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
