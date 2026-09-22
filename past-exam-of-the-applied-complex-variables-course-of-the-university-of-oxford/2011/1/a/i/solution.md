<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $\alpha_j=1-\beta_j$, so the interior [angle](../../../../../angle.md) at the $j$th [polygon](../../../../../polygon.md) vertex is $\pi\alpha_j$. A [conformal map](../../../../../conformal-map.md) straightens that corner by a power: locally,

$$
f(z)-f(x_j)\sim A_j(z-x_j)^{\alpha_j},\qquad f'(z)\sim\alpha_jA_j(z-x_j)^{-\beta_j}.
$$

This follows by composing with the power $1/\alpha_j$ that maps the corner to a half-plane and using [Schwarz reflection](../../../../../schwarz-reflection-principle.md) along its straight edges. The reflected map has a nonzero first [derivative](../../../../../derivative.md) in the straightened coordinates.

For an upper-half-plane [branch of the complex logarithm](../../../../../branch-of-the-complex-logarithm.md), define

$$
P(z)=\prod_{j=1}^n\exp\bigl(-\beta_j\operatorname{Log}(z-x_j)\bigr).
$$

Along each open interval of the real axis, $P$ has constant [argument](../../../../../argument-complex-analysis.md). Crossing $x_j$ from left to right decreases $\arg(z-x_j)$ from $\pi$ to zero, so the [argument](../../../../../argument-complex-analysis.md) of $P$ increases by $\beta_j\pi$. This is exactly the exterior turning [angle](../../../../../angle.md) of the polygon [boundary](../../../../../boundary-of-a-set.md). Thus $f'/P$ has one constant [boundary](../../../../../boundary-of-a-set.md) [argument](../../../../../argument-complex-analysis.md) on all the intervals. The corner asymptotics remove its apparent [singularity](../../../../../complex-singularity.md) at each [prevertex](../../../../../prevertex-of-a-schwarz-christoffel-map.md).

For a bounded polygon, the sum of exterior [angles](../../../../../angle.md) gives $\sum_j\beta_j=2$. Since every vertex has a finite [prevertex](../../../../../prevertex-of-a-schwarz-christoffel-map.md), [infinity](../../../../../infinity.md) maps to an ordinary point of an edge. In the local coordinate $1/z$, [Schwarz reflection](../../../../../schwarz-reflection-principle.md) gives $f(z)=f(\infty)+d/z+O(z^{-2})$ with $d\ne0$. Hence $f'/P$ has a finite nonzero limit at [infinity](../../../../../infinity.md). After multiplication by one unit [complex number](../../../../../complex-number.md), its [boundary values](../../../../../boundary-value.md) are real. Reflecting across the real axis extends it to an [entire function](../../../../../entire-function.md), including each removed [prevertex](../../../../../prevertex-of-a-schwarz-christoffel-map.md), and it is bounded at [infinity](../../../../../infinity.md). [Liouville's theorem](../../../../../liouville-theorem.md) makes it constant. Therefore the [Schwarz-Christoffel formula](../../../../../schwarz-christoffel-mapping.md) is

$$
\boxed{f'(z)=c\prod_{j=1}^n(z-x_j)^{-\beta_j},\qquad c\ne0.}
$$

Integration introduces one further additive constant.

The [Möbius transformations](../../../../../mobius-transformation.md) preserving the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) have three real parameters:

$$
z\longmapsto\frac{az+b}{cz+d},\qquad a,b,c,d\in\mathbb R,\quad ad-bc>0,
$$

with common nonzero scaling irrelevant. They can send any cyclically ordered triple of [boundary](../../../../../boundary-of-a-set.md) points to another such triple. Consequently **three prevertices may be fixed independently**; the other $n-3$ are constrained by the polygon's shape, through its side-length ratios. The constants of integration and multiplication account for translation, rotation and scale of the image, rather than further [prevertex](../../../../../prevertex-of-a-schwarz-christoffel-map.md) freedom.

If the last [prevertex](../../../../../prevertex-of-a-schwarz-christoffel-map.md) is [infinity](../../../../../infinity.md), use $1/z$ as its local coordinate. Its factor is absorbed into the overall normalization, leaving

$$
\boxed{f'(z)=c\prod_{j=1}^{n-1}(z-x_j)^{-\beta_j}.}
$$

For a finite image vertex at [infinity](../../../../../infinity.md)'s preimage, this has asymptotic order $z^{\beta_n-2}$, because $f(z)-f(\infty)$ is of order $z^{-(1-\beta_n)}$. Thus the omitted factor is not evaluated by substituting [infinity](../../../../../infinity.md) into the finite product; its [angle](../../../../../angle.md) is encoded by the behavior at [infinity](../../../../../infinity.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the applied complex variables course of the University of Oxford](../../../../split.md)
6. [Applied complex variables course of the University of Oxford](../../../../../applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
