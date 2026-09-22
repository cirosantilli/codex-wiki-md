<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Use the [Poincaré half-plane model](../../../../../poincare-half-plane-model.md), $\mathbb H=\{x+iy:y>0\}$ with metric $ds^2=(dx^2+dy^2)/y^2$. Its [hyperbolic lines](../../../../../hyperbolic-line.md) are vertical lines and semicircles centred on the real boundary, hence orthogonal to that boundary. Each has two [ideal endpoints](../../../../../ideal-endpoint.md) in $\mathbb R\cup\{\infty\}$. Distinct [parallel hyperbolic lines](../../../../../parallel-hyperbolic-lines.md) are disjoint inside $\mathbb H$ and share one ideal endpoint; distinct [ultraparallel hyperbolic lines](../../../../../ultraparallel-hyperbolic-lines.md) are disjoint and share none. Intersecting lines are neither. Because the metric is conformal to the Euclidean metric, the two notions of angle agree.

Apply a hyperbolic [isometry](../../../../../isometry.md) taking one line $l$ to the imaginary axis, whose ideal endpoints are $0,\infty$. If the other line $l'$ is ultraparallel, its endpoints are two finite nonzero real numbers of the same sign. Reflect if necessary to write them as $0<a<b$. Then $l'$ is the semicircle with centre $c=(a+b)/2$ and radius $r=(b-a)/2$.

Every [hyperbolic line](../../../../../hyperbolic-line.md) perpendicular to the imaginary axis must be a semicircle centred at zero: at the intersection its tangent has to be horizontal, forcing its real centre to coincide with zero. Let its radius be $R$. Orthogonality to the circle representing $l'$ requires $c^2=R^2+r^2$, since the radii to the intersection form a right triangle. Consequently

$$
\boxed{R^2=c^2-r^2=ab.}
$$

This has exactly one positive solution. The circles intersect above the real axis: $c-r=a<\sqrt{ab}<b=c+r$. Hence the required [common perpendicular of ultraparallel hyperbolic lines](../../../../../common-perpendicular-of-ultraparallel-hyperbolic-lines.md) exists and is unique.

Conversely, if $l'$ intersects the imaginary axis, its endpoints straddle zero and the same equation would require $R^2=ab<0$, which is impossible. If $l'$ has endpoint zero, it gives $R^2=0$, not a line. If its shared endpoint is infinity, $l'$ is another vertical line; no circle centred at zero meets a distinct vertical line with horizontal tangent. Thus parallel lines have no common perpendicular either. These cases exhaust distinct lines, proving **a unique common perpendicular exists exactly for ultraparallel lines**.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
