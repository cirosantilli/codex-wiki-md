<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Orient the plane relative to the eye. For its [affine function](../../../../../../affine-function.md) $F(P)=n\cdot P-d$, assume $F(E)\ne0$ and put $\ell(P)=\operatorname{sign}(F(E))F(P)$. The desired closed [half-space](../../../../../../half-space.md) is $\ell\geq0$. If the eye is on the plane, the notion of its side is undefined and a side convention must be supplied.

Apply [recursive half-space clipping of a subdivision curve](../../../../../../recursive-half-space-clipping-of-a-subdivision-curve.md) to each initial curve piece. Obtain a certified [bounding volume](../../../../../../bounding-volume.md) $K$, and calculate $l=\min_K\ell$, $h=\max_K\ell$. For a control-point [convex hull](../../../../../../convex-hull.md), these extrema occur at its vertices, so this test is inexpensive. If $h<0$, discard the piece. If $l\geq0$, retain the whole piece and draw its chord only when its certified flatness is within the screen-space tolerance; otherwise subdivide and draw the children in parameter order. If $l<0\leq h$, subdivide and repeat the classification.

At a sufficiently flat and sufficiently short terminal piece, clip the approximating chord from $A$ to $B$ against $\ell\geq0$. If both endpoints are nonnegative retain the chord; if both are negative discard the chord; for opposite signs split it at

$$
\boxed{P_*=(1-\lambda)A+\lambda B,\qquad\lambda={\ell(A)\over\ell(A)-\ell(B)}}.
$$

Retain the portion with nonnegative $\ell$. Handle an endpoint exactly on the plane without dividing by zero, and retain a coplanar chord under the closed-half-space convention. The recursion yields an ordered polyline rather than connecting endpoints of disconnected retained pieces.

Crucially, do not reject an unresolved whole curve merely because its endpoints have negative signs: it can cross the plane twice and have a visible interior excursion. The preceding terminal chord rule is a rendering approximation at an explicitly chosen spatial tolerance. A flatness bound and a diameter bound make any missed leaf-sized excursion spatially small; they do not prove exact crossing topology, especially for a near-tangent contact or an unfavorable projection. Use the actual viewing projection to enforce a screen-space tolerance, with special handling near a perspective singularity.

If exact clipping intervals are required for a spline representation, isolate all roots of $\ell(C(t))$, split at them and classify each intervening interval. [Bernstein basis](../../../../../../bernstein-basis.md) coefficient bounds, derivative bounds and recursive subdivision can isolate roots on polynomial spans, including even-multiplicity tangencies. Treat identically coplanar spans separately. For a general [subdivision curve](../../../../../../subdivision-curve.md), keep unresolved straddling pieces flagged or refine to the chosen tolerance instead of claiming that a finite endpoint-sign test is exact. **Certified half-space rejection combined with adaptive subdivision is the recursive drawing algorithm; exact boundary topology needs additional root isolation.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
