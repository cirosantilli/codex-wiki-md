<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The degree-$n$ [Bernstein basis](../../../../../../bernstein-basis.md) on $[0,1]$ is

$$
\boxed{B_i^n(t)=\binom ni t^i(1-t)^{n-i},\qquad i=0,\ldots,n.}
$$

The associated [Bézier curve](../../../../../../bezier-curve.md) is $C(t)=\sum_iP_iB_i^n(t)$. The basis is nonnegative and has [partition of unity](../../../../../../partition-of-unity.md), since $\sum_iB_i^n(t)=(t+1-t)^n=1$. Thus the curve is a [convex combination](../../../../../../convex-combination.md) of its [control points](../../../../../../control-point.md), giving the [convex hull](../../../../../../convex-hull.md) enclosure useful for geometric bounds. The same identity makes the construction invariant under application of [affine functions](../../../../../../affine-function.md).

It interpolates its endpoint controls, $C(0)=P_0$, $C(1)=P_n$, and its endpoint [tangent vectors](../../../../../../tangent-vector.md) are $n(P_1-P_0)$ and $n(P_n-P_{n-1})$. These follow from

$$
C'(t)=n\sum_{i=0}^{n-1}(P_{i+1}-P_i)B_i^{n-1}(t).
$$

The [control polygon](../../../../../../control-polygon.md) therefore gives direct geometric editing and tangent control. Repeated interpolation by the [De Casteljau algorithm](../../../../../../de-casteljau-s-algorithm.md) evaluates and subdivides the curve without converting to a monomial representation. Together, positive geometric weights, simple endpoint behavior and stable subdivision make this basis useful in [computer aided geometric design](../../../../../../computer-aided-geometric-design.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
