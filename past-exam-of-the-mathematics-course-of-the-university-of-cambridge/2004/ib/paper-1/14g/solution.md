<h1 id="14g/solution">Solution</h1>

↑ **Parent:** [14G](../14g.md)

In the [upper half-plane model](../../../../../poincare-half-plane-model.md), a [hyperbolic line](../../../../../hyperbolic-line.md) is either a vertical line or a Euclidean semicircle perpendicular to the real axis. For the vertical line $x=a$, set $R_L(z)=2a-\bar z$. For the circle $|z-a|=r$ with real $a$, set

$$
\boxed{R_L(z)=a+\frac{r^2}{\bar z-a}.}
$$

The vertical formula preserves $y$ and Euclidean speed. For the circular formula, $\operatorname{Im}R_L(z)=r^2\operatorname{Im}z/|z-a|^2$, while its local Euclidean length multiplier is $r^2/|z-a|^2$. Thus both preserve $|dz|/\operatorname{Im}z$, the [hyperbolic metric](../../../../../hyperbolic-metric.md), and consequently all curve lengths and distances. Each is an involution preserving the half-plane; each fixes its specified line pointwise and moves points off that line. This establishes the required [hyperbolic reflection](../../../../../hyperbolic-reflection.md) explicitly.

To factor an arbitrary [isometry](../../../../../isometry.md) $g$, first recall why a bisector reflection exchanges any distinct points $P,Q$. The [hyperbolic distance](../../../../../hyperbolic-distance.md) formula is

$$
\cosh d(x+iy,a+ib)=\frac{(x-a)^2+y^2+b^2}{2yb}.
$$

Equating the distances to $P$ and $Q$ yields a vertical line or a circle with centre on the real axis, hence a [hyperbolic line](../../../../../hyperbolic-line.md). Substitution in the reflection formulas above shows that its reflection exchanges $P$ and $Q$. Choose a base point $P$. If $gP\ne P$, compose $g$ on the left with their bisector reflection, obtaining $h$ that fixes $P$; otherwise take $h=g$.

Choose $Q\ne P$. The points $hQ,Q$ have the same distance from $P$, so their bisector contains $P$. If they differ, its reflection corrects $hQ$ while retaining $P$. We obtain an [isometry](../../../../../isometry.md) $k$ fixing both $P,Q$ after at most two reflections.

An [isometry](../../../../../isometry.md) fixing two points is either the identity or reflection in their joining line. To see this directly, a point with prescribed distances from $P,Q$ lies at the intersection of two [hyperbolic circles](../../../../../hyperbolic-circle.md); these are Euclidean circles in this model and have at most two intersections. When there are two, reflection in the line $PQ$ interchanges them. Pick a third point off that line. Either $k$ fixes it, or composing $k$ with that line reflection fixes it. An [isometry](../../../../../isometry.md) fixing three noncollinear points is the identity: the first two distances leave only the reflected pair, and the distance to the third point distinguishes that pair. Thus $k$ is the identity or one additional reflection. Reversing the compositions proves **every [isometry](../../../../../isometry.md) is a product of at most three [hyperbolic reflections](../../../../../hyperbolic-reflection.md)**.

## ↑ Ancestors (10)

1. [14G](../14g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
