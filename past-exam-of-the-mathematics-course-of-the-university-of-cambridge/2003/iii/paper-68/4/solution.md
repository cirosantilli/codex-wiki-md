<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [subdivision curve interrogation](../../../../../subdivision-curve-interrogation.md) interface provides its control/topology data, a parameter interval or address, and a refinement operation returning restricted child pieces with their parameter correspondence. It also provides a certified enclosing [bounding volume](../../../../../bounding-volume.md), endpoints or limit-point enclosures, and an error estimate for replacing a sufficiently small piece by its chord. Positional and [derivative](../../../../../derivative.md) limit queries may be implemented by refinement or by conversion to the appropriate [spline](../../../../../spline-mathematics.md). Nonnegative masks often imply a control-point [convex hull](../../../../../convex-hull.md) bound; a generic scheme with negative weights needs a separate bound.

These enquiries can be applied to a [parametric curve](../../../../../parametric-curve.md) by using interval restriction as the subdivision operation and constructing its enclosure from its representation. For example, a [Bézier curve](../../../../../bezier-curve.md) is split by [De Casteljau's algorithm](../../../../../de-casteljau-s-algorithm.md), and each child's control-point [convex hull](../../../../../convex-hull.md) encloses exactly that child arc. More generally, if a restricted curve has a certified bound $\|C'(t)\|\leq L_I$, the midpoint $m$ supplies

$$
\|C(t)-C(m)\|\leq L_I|t-m|\leq L_I|I|/2.
$$

This ball gives a signed plane-range enclosure. Such an upper [derivative](../../../../../derivative.md) bound must be supplied or proved; taking the largest [derivative](../../../../../derivative.md) seen in a few samples is not a certificate.

The recursive intersection algorithm is as follows. Start with the whole domain. For each piece with enclosure $B_I$, compute

$$
\alpha_I=\min_{x\in B_I}(n\cdot x-d),\qquad
\beta_I=\max_{x\in B_I}(n\cdot x-d).
$$

If $\alpha_I>0$ or $\beta_I<0$, discard that piece. Otherwise split it and process the children, unless a root has already been uniquely isolated and can be polished as in Question 3. For a [convex hull](../../../../../convex-hull.md) bound, the extrema of this affine plane function are attained among its [control points](../../../../../control-point.md), so only dot products are required. For an [axis-aligned bounding box](../../../../../axis-aligned-bounding-box.md), choose the low or high coordinate in each term according to the sign of $n_i$.

At a small flat piece, the chord-plane parameter is

$$
t_{\rm chord}=a-\frac{F(a)(b-a)}{F(b)-F(a)}
$$

when the denominator is nonzero. It supplies an initial estimate, which is corrected on the actual curve. A chord of a piece with geometric error $\varepsilon$ gives plane-function error at most $\|n\|\varepsilon$; a transverse root additionally needs a positive [derivative](../../../../../derivative.md) lower bound to convert that into a parameter error. **A chord hit is not by itself a proof of the exact crossing count.** Keep unresolved tangent contacts, merge shared-endpoint hits, and return any certified coplanar parameter intervals separately.

Good speed comes from a [bounding volume hierarchy](../../../../../bounding-volume-hierarchy.md), conservative cheap rejection before accurate evaluation, caching shared subdivision work, local rather than uniform refinement, and fast root polishing only after isolation. Convex-hull or box extrema cost far less than solving every potential intersection. Tight bounds shrink rapidly with subdivision and reduce the active search to neighborhoods of actual crossings. [Derivative](../../../../../derivative.md) information can prove monotonicity, accelerate with the [Newton root-finding iteration](../../../../../newton-root-finding-iteration.md), or tighten range bounds using [interval arithmetic](../../../../../interval-arithmetic.md). There is no universal fixed speed guarantee when the curve is nearly coplanar or has arbitrarily many intersections: those are genuinely difficult inputs. The representation must provide meaningful bounds and restriction operations; point/[derivative](../../../../../derivative.md) enquiries alone do not imply such capabilities.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
