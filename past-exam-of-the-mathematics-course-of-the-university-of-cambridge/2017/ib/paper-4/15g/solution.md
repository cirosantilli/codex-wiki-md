<h1 id="15g/solution">Solution</h1>

↑ **Parent:** [15G](../15g.md)

Use curvature $-1$. In the [Poincare disc model](../../../../../poincare-disk-model.md), [hyperbolic lines](../../../../../hyperbolic-line.md) are Euclidean diameters and arcs of [circles](../../../../../circle.md) orthogonal to the unit [circle](../../../../../circle.md), with [hyperbolic length](../../../../../hyperbolic-length-in-the-poincare-disc.md) element $ds=2|dz|/(1-|z|^2)$. In the [upper half-plane model](../../../../../poincare-half-plane-model.md), they are vertical lines and semicircles with centres on the real axis, with $ds=|dz|/\operatorname{Im}z$. Both displayed [hyperbolic metrics](../../../../../hyperbolic-metric.md) are positive scalar multiples of the Euclidean metric, so their [angles](../../../../../angle.md) agree with Euclidean [angles](../../../../../angle.md). The [hyperbolic distance](../../../../../hyperbolic-distance.md) is the length of the joining [hyperbolic line](../../../../../hyperbolic-line.md) segment; explicitly, in the [upper half-plane model](../../../../../poincare-half-plane-model.md),

$$
\boxed{d(P,Q)=\operatorname{arcosh}\left(1+\frac{|P-Q|^2}{2\operatorname{Im}P\operatorname{Im}Q}\right)}.
$$

In the [Poincare disc model](../../../../../poincare-disk-model.md) it is $2\operatorname{artanh}|(P-Q)/(1-\overline P Q)|$.

For distinct $P,Q$, a [isometry](../../../../../isometry.md) sends their joining [hyperbolic line](../../../../../hyperbolic-line.md) to the imaginary axis, so their images are $ip,iq$ with $p,q>0$. For any [continuously differentiable](../../../../../continuously-differentiable-function.md) curve $x(t)+iy(t)$ joining them,

$$
\ell(\gamma)=\int\frac{\sqrt{x'(t)^2+y'(t)^2}}{y(t)}\,dt
\geq\int\frac{|y'(t)|}{y(t)}\,dt
\geq|\log q-\log p|=d(P,Q).
$$

Equality in the first inequality requires $x'=0$ everywhere, because the nonnegative difference is [continuous](../../../../../continuous-function.md). Equality in the second requires $y'$ to have one sign, allowing zero intervals. Thus **equality holds precisely for a monotone reparametrisation of the joining hyperbolic segment**. Conversely every such reparametrisation gives equality. For $P=Q$, equality means length zero and the constant curve; monotonicity is understood non-strictly.

Two distinct [hyperbolic lines](../../../../../hyperbolic-line.md) are [parallel hyperbolic lines](../../../../../parallel-hyperbolic-lines.md) if they are disjoint in the plane and have exactly one common [ideal endpoint](../../../../../ideal-endpoint.md); they are [ultraparallel hyperbolic lines](../../../../../ultraparallel-hyperbolic-lines.md) if they are disjoint and have no common [ideal endpoint](../../../../../ideal-endpoint.md). To prove the [common perpendicular of ultraparallel hyperbolic lines](../../../../../common-perpendicular-of-ultraparallel-hyperbolic-lines.md) theorem, send one line to the imaginary axis. An [ultraparallel hyperbolic lines](../../../../../ultraparallel-hyperbolic-lines.md) second line can, after reflection if necessary, be written as a semicircle with centre $c>0$ and radius $r$ satisfying $c>r$. A [hyperbolic line](../../../../../hyperbolic-line.md) perpendicular to the imaginary axis must be a semicircle centred at zero, of some radius $R>0$. The Euclidean condition for its orthogonality to the second [circle](../../../../../circle.md) is

$$
\boxed{R^2=c^2-r^2}.
$$

This has exactly one positive solution, proving existence and uniqueness. Conversely, if such a common perpendicular exists, the second line cannot be another vertical line, and the same condition forces $|c|>r$, so its endpoints lie strictly on one side of zero and it is [ultraparallel hyperbolic lines](../../../../../ultraparallel-hyperbolic-lines.md). This includes exclusion of intersecting lines ($|c|<r$) and [parallel hyperbolic lines](../../../../../parallel-hyperbolic-lines.md) ($|c|=r$ or another vertical line). The statement concerns distinct lines: a line coincident with itself would have many perpendiculars.

A [horocycle](../../../../../horocycle.md) in the [upper half-plane model](../../../../../poincare-half-plane-model.md) is either a Euclidean [circle](../../../../../circle.md) tangent to the real axis from above, with the tangent point as its [ideal centre of a horocycle](../../../../../ideal-centre-of-a-horocycle.md), or a horizontal line $y=h>0$, whose [ideal centre of a horocycle](../../../../../ideal-centre-of-a-horocycle.md) is infinity. A [isometry](../../../../../isometry.md) sending this centre to infinity sends the [horocycle](../../../../../horocycle.md) to a horizontal line. The [hyperbolic lines](../../../../../hyperbolic-line.md) meeting that horizontal line orthogonally are exactly the vertical lines; therefore the [hyperbolic lines](../../../../../hyperbolic-line.md) orthogonal to a [horocycle](../../../../../horocycle.md) are exactly those with its ideal centre as an endpoint.

If two [horocycles](../../../../../horocycle.md) have distinct [horocycle centres](../../../../../ideal-centre-of-a-horocycle.md), the unique [hyperbolic line](../../../../../hyperbolic-line.md) with those two [ideal endpoints](../../../../../ideal-endpoint.md) meets both orthogonally. If they have the same [horocycle centre](../../../../../ideal-centre-of-a-horocycle.md), send it to infinity: both become horizontal lines and every vertical [hyperbolic line](../../../../../hyperbolic-line.md) meets both orthogonally. Hence

$$
\boxed{\text{The common orthogonal line is unique exactly when the ideal centres differ.}}
$$

In the other case there are infinitely many; intersection or tangency of the two [horocycles](../../../../../horocycle.md) does not change this classification.

## ↑ Ancestors (10)

1. [15G](../15g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
