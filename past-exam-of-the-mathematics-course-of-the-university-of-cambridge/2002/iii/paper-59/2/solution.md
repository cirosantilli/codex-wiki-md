<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An efficient [parametric curve interrogation](../../../../../parametric-curve-interrogation.md) interface should provide the parameter domain and open/closed status, point evaluation, one-sided endpoint enquiries, first and second [derivatives](../../../../../derivative.md) wherever defined, and information about knots or singular parameters. It should also restrict a curve to an interval and subdivide it without changing its limit, return a certified [bounding volume](../../../../../bounding-volume.md) for that restriction, and supply derivative or [chord error bounds](../../../../../chord-error-bound.md) when supported. These enquiries allow cheap geometric rejection before expensive exact evaluation. For a [subdivision curve](../../../../../subdivision-curve.md), limit evaluation is distinct from returning a vertex of a finite refined [control polygon](../../../../../control-polygon.md); the latter is usually an approximation.

For a query point $Q$, minimize $d(t)=\tfrac12\|P(t)-Q\|^2$. At a differentiable interior minimizer,

$$
\boxed{(P(t)-Q)\cdot P'(t)=0.}
$$

At a regular curve point this says that the query displacement is perpendicular to the [tangent vector](../../../../../tangent-vector.md). If a second [derivative](../../../../../derivative.md) exists, the local second-order test is

$$
d''(t)=\|P'(t)\|^2+(P(t)-Q)\cdot P''(t)\ge0;
$$

a strictly positive value is sufficient for a strict local minimum. The stationarity equation alone also includes local maxima and is automatic at $P'=0$, so it cannot be used as the only global search criterion.

A reliable efficient [closest-point search on a subdivision curve](../../../../../closest-point-search-on-a-subdivision-curve.md) uses [branch and bound](../../../../../branch-and-bound.md). Cover the compact curve by restricted pieces with certified enclosures $B_I$. For each piece set $L_I=\operatorname{dist}(Q,B_I)$, a lower bound on its true distance. Distances to actually evaluated limit points give upper bounds; keep the best point $P(t_*)$ and distance $U$. For an [axis-aligned bounding box](../../../../../axis-aligned-bounding-box.md) $\prod_k[l_k,h_k]$, the squared lower bound is inexpensive:

$$
L_I^2=\sum_k\bigl(\max\{l_k-Q_k,0,Q_k-h_k\}\bigr)^2.
$$

For positive partition-of-unity refinement, a [convex hull](../../../../../convex-hull.md) of the active [control points](../../../../../control-point.md) is an enclosure. A negative-weight scheme requires a separate certified enclosure; its control hull need not contain the limit.

The algorithm is:

- Initialize the pieces at representation breaks and evaluate endpoints and one or more interior limit points. Place pieces in a priority queue ordered by their $L_I$.
- Discard any piece with $L_I>U$, since it cannot improve the best known point. If only one nearest point is required, equality may also be discarded; keep equality candidates when all ties matter.
- Remove the smallest-bound piece. Evaluate new limit points to reduce $U$, subdivide the piece, compute tighter child enclosures, and insert children that can still improve $U$.
- Use the best chord projection or current candidate to seed a safeguarded [Newton root-finding iteration](../../../../../newton-root-finding-iteration.md) for $F(t)=(P(t)-Q)\cdot P'(t)$. Its derivative is $F'(t)=\|P'\|^2+(P-Q)\cdot P''$. Keep iterates inside the restricted interval, fall back to [bisection method](../../../../../bisection-method.md) on an isolated sign-changing bracket, and accept an improvement only after evaluating its actual curve distance. This is an accelerator; rejection still depends on certified geometric bounds.
- Terminate when $U-\min_I L_I\le\epsilon$, also regarding the best evaluated point as a retained candidate. If no pieces remain, the evaluated candidate is already optimal relative to the exhausted bounds. Return $t_*$ and $P(t_*)$ with the global distance guarantee.

Because $\min_I L_I\le d_{\min}\le U$, the reported point is at most $\epsilon$ farther from $Q$ than a true nearest point. Include endpoints, nondifferentiable joins, and singular parameters in the candidate bookkeeping, or split them into separate pieces. With enclosures converging in diameter under subdivision on a compact continuous curve, the bounds converge to arbitrary prescribed positive distance tolerance. Interval bounds or outward-rounded arithmetic are needed if the guarantee is intended to be certified in floating-point computation. A single [Newton root-finding iteration](../../../../../newton-root-finding-iteration.md) from a single seed supplies no such global guarantee.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
