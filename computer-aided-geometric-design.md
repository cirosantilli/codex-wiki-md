# Computer aided geometric design

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[Computer aided geometric design](computer-aided-geometric-design.md) studies computational representations, evaluation and manipulation of [curves](topology.md#curve) and [regular surfaces](differential-geometry.md#smooth-surface), especially using [splines](uniform-approximation.md#spline-mathematics) and [subdivision surfaces](#subdivision-surface).

// Target: geometry-and-topology.bigb

**Table of contents**

- [Affine equivariance of a geometric basis](#affine-equivariance-of-a-geometric-basis)
- [Translational penetration depth](#translational-penetration-depth)
- [Linear precision of a geometric basis](#linear-precision-of-a-geometric-basis)
- [Control point](#control-point)
  - [Control-point influence on a curve](#control-point-influence-on-a-curve)
  - [Control net](#control-net)
  - [Control polygon](#control-polygon)
- [Apparent-gravity camera frame](#apparent-gravity-camera-frame)
- [Subdivision curve](#subdivision-curve)
  - [Binary linear interpolatory subdivision](#binary-linear-interpolatory-subdivision)
  - [Functional precision set of a subdivision scheme](#functional-precision-set-of-a-subdivision-scheme)
  - [Chaikin subdivision](#chaikin-subdivision)
    - [Chaikin basis function](#chaikin-basis-function)
    - [Polynomial degree preservation under Chaikin subdivision](#polynomial-degree-preservation-under-chaikin-subdivision)
  - [Support of a stationary subdivision scheme](#support-of-a-stationary-subdivision-scheme)
  - [Subdivision curve interrogation](#subdivision-curve-interrogation)
    - [Closest-point search on a subdivision curve](#closest-point-search-on-a-subdivision-curve)
    - [Shadow tracing for a subdivision curve](#shadow-tracing-for-a-subdivision-curve)
    - [Recursive half-space clipping of a subdivision curve](#recursive-half-space-clipping-of-a-subdivision-curve)
- [Subdivision surface](#subdivision-surface)
  - [Lateral artifacts of a subdivision surface](#lateral-artifacts-of-a-subdivision-surface)
    - [Extrusion invariance of a ternary triangular scheme](#extrusion-invariance-of-a-ternary-triangular-scheme)
  - [Mid-edge subdivision](#mid-edge-subdivision)
    - [Mid-edge facet centroid invariance](#mid-edge-facet-centroid-invariance)
  - [Subdivision surface interrogation](#subdivision-surface-interrogation)
    - [Intersection of subdivision limit surfaces](#intersection-of-subdivision-limit-surfaces)
    - [Plane section of a subdivision surface](#plane-section-of-a-subdivision-surface)
    - [Minimum distance between subdivision bodies](#minimum-distance-between-subdivision-bodies)
  - [Extraordinary subdivision vertex](#extraordinary-subdivision-vertex)
    - [Characteristic map of a subdivision surface](#characteristic-map-of-a-subdivision-surface)
  - [Quincunx subdivision](#quincunx-subdivision)
  - [Loop subdivision surface](#loop-subdivision-surface)
    - [Polynomial generation by regular Loop subdivision](#polynomial-generation-by-regular-loop-subdivision)
    - [Extrusion invariance of Loop subdivision](#extrusion-invariance-of-loop-subdivision)
  - [Subdivision mask](#subdivision-mask)
    - [Subdivision mask width](#subdivision-mask-width)
    - [Subdivision arity](#subdivision-arity)
    - [Subdivision difference scheme](#subdivision-difference-scheme)
      - [Norm and spectral bounds for subdivision regularity](#norm-and-spectral-bounds-for-subdivision-regularity)
    - [Subdivision matrix](#subdivision-matrix)
- [Bézier curve](#bezier-curve)
  - [Bézier derivative control polygon](#bezier-derivative-control-polygon)
    - [Parametric first-derivative join of Bézier curves](#parametric-first-derivative-join-of-bezier-curves)
  - [De Casteljau's algorithm](#de-casteljau-s-algorithm)
- [Bounding volume](#bounding-volume)
  - [Conservative enclosure test](#conservative-enclosure-test)
  - [Collision detection](#collision-detection)
    - [Broad phase](#broad-phase)
    - [Narrow phase](#narrow-phase)
  - [Bounding volume hierarchy](#bounding-volume-hierarchy)
    - [Bounding volume hierarchy traversal](#bounding-volume-hierarchy-traversal)
  - [Axis-aligned bounding box](#axis-aligned-bounding-box)
- [Triangle-triangle intersection algorithm](#triangle-triangle-intersection-algorithm)

## Affine equivariance of a geometric basis

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)

A geometry representation with scalar [partition of unity](smooth-manifold.md#partition-of-unity) basis functions commutes with every [affine map](geometry-and-topology.md#affine-map) of its [control points](#control-point). For $T(x)=Ax+b$, linearity moves $A$ through the sum and the sum-to-one identity supplies the translation $b$. Positivity is needed for a [convex hull](convex-set.md#convex-hull) property, but not for this equivariance. The same argument applies to linear [subdivision matrices](#subdivision-matrix) whose rows sum to one. General [projective transformations](projective-space.md#projective-linear-transformation) require homogeneous [control points](#control-point) and rational dehomogenization rather than transforming Euclidean controls with unchanged weights.

## Translational penetration depth

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)

For overlapping solid bodies, the penetration depth is the smallest translation needed to remove interior overlap, with orientation fixed. It is distance from the origin to the complement of the translational collision region. Define signed separation as positive ordinary separation for disjoint bodies, zero for contact, and $-\delta$ for interior overlap. Translation-space [branch and bound](mathematical-optimization.md#branch-and-bound) can bracket it using certified intersection/containment queries. This convention handles crossing and complete containment; merely negating unsigned boundary distance does not.

## Linear precision of a geometric basis

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)

A basis with the displayed identities reproduces [affine functions](vector-space.md#affine-function) from their values at the precision sites $\xi_j$. For two such bases, the tensor-product precision sites are $(\xi_j,\eta_k)$: summation independently recovers $u$ and $v$. Affine images of this site grid therefore produce exact planar parameterizations, independent of the chosen control-grid representation.

## Control point

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)

A [control point](#control-point) is an editable geometric handle used to specify a [curve](topology.md#curve) or [surface](topological-surface.md) through a [basis](vector-space.md#basis) or refinement rule. The handle is part of the representation; it need not be a [point](geometry-and-topology.md#point-geometry) on the resulting [curve](topology.md#curve). In a [Bézier curve](#bezier-curve), the [control points](#control-point) are the geometric [coefficients](vector-space.md#coefficient) of the [Bernstein basis](functional-analysis.md#bernstein-basis). Joining them in order gives a [control polygon](#control-polygon), which makes the handles easy to manipulate without drawing the [curve](topology.md#curve) as a chain of [line segments](convex-set.md#line-segment).[§4.3, pp. 132–133: control points and Bernstein representation; §5.1, p. 148: control polygon](mathematics-bibliography.md#curves-and-surfaces-in-geometric-modeling-theory-and-algorithms-by-jean-gallier)

For example, use the cubic [Bézier curve](#bezier-curve) with [control points](#control-point)

$$
P_0=(0,0),\qquad P_1=(1,2),\qquad P_2=(3,2),\qquad P_3=(4,0).
$$

Its [Bernstein basis](functional-analysis.md#bernstein-basis) representation gives

$$
C(t)=\bigl(3t+3t^2-2t^3,\;6t(1-t)\bigr),\qquad 0\leq t\leq1,\qquad C(1/2)=(2,1.5).
$$

The greatest height is $1.5$, so neither interior [control point](#control-point), both at height $2$, lies on this [curve](topology.md#curve). The endpoint [control points](#control-point) do lie on it: $C(0)=P_0$ and $C(1)=P_3$. This separates [interpolation](interpolation.md), which requires passage through prescribed data, from an approximating representation, which uses handles to shape a [curve](topology.md#curve) without requiring passage through every handle. If measured [points](geometry-and-topology.md#point-geometry) must be interpolated, choose [control points](#control-point) to satisfy those constraints; simply using the measured [points](geometry-and-topology.md#point-geometry) as the handles of a [Bézier curve](#bezier-curve) does not enforce [interpolation](interpolation.md).

<a id="image-original-cubic-and-the-curve-after-moving-only-the-interior-control-point-p1-upward-by-one-unit-with-fixed-endpoints-and-a-smaller-displacement-at-the-same-parameter"></a>
![](control-point-cubic-curve-edit.png)

**[Figure 1](#image-original-cubic-and-the-curve-after-moving-only-the-interior-control-point-p1-upward-by-one-unit-with-fixed-endpoints-and-a-smaller-displacement-at-the-same-parameter). Original cubic and the curve after moving only the interior control point P1 upward by one unit, with fixed endpoints and a smaller displacement at the same parameter**.

Now move only $P_1$ by the [vector](vector-space.md#vector) $h=(0,1)$, giving $\widetilde P_1=(1,3)$. With the [Bernstein basis](functional-analysis.md#bernstein-basis) and parameter $t$ unchanged, the new [curve](topology.md#curve) is

$$
\widetilde C(t)=C(t)+3t(1-t)^2h.
$$

At $t=1/2$ this gives $\widetilde C(1/2)=(2,15/8)$, a displacement $(0,3/8)$ despite moving the handle by a full unit. Both endpoints stay fixed because the [coefficient](vector-space.md#coefficient) $3t(1-t)^2$ vanishes there. Thus dragging a [control point](#control-point) shapes a whole range of the [curve](topology.md#curve); it does not generally drag an arbitrary selected [point](geometry-and-topology.md#point-geometry) on the [curve](topology.md#curve) by the same [vector](vector-space.md#vector). The [control-point influence on a curve](#control-point-influence-on-a-curve) tells us exactly how much each parameter value moves.

### Control-point influence on a curve

↑ **Parent:** [Control point](#control-point)

For a [parametric curve](topology.md#parametric-curve) represented by fixed scalar [functions](function.md) $b_j$ and [control points](#control-point) $P_j$ in [Euclidean space](normed-vector-space.md#euclidean-norm), write

$$
C(t)=\sum_j b_j(t)P_j,\qquad \widetilde P_i=P_i+h,\qquad \widetilde P_j=P_j\quad(j\ne i).
$$

The influence function of this handle is $b_i$: the resulting displacement [vector](vector-space.md#vector) is $\Delta C(t)=\widetilde C(t)-C(t)=b_i(t)h$, and its [norm](normed-vector-space.md#norm) is $|b_i(t)|\,\|h\|$. These are exact finite changes, not only a first-order estimate. Where $b_i$ is negative the displacement points opposite to $h$. Where $b_i(t)=0$, the [curve](topology.md#curve) is unchanged at that parameter.

<a id="image-the-influence-coefficient-3t-1-t-2-equals-the-vertical-displacement-for-a-unit-upward-move-of-p1-reaches-4-9-at-t-1-3-and-vanishes-at-both-endpoints"></a>
![](control-point-cubic-basis-influence.png)

**[Figure 2](#image-the-influence-coefficient-3t-1-t-2-equals-the-vertical-displacement-for-a-unit-upward-move-of-p1-reaches-4-9-at-t-1-3-and-vanishes-at-both-endpoints). The influence coefficient 3t(1-t)^2 equals the vertical displacement for a unit upward move of P1, reaches 4/9 at t=1/3, and vanishes at both endpoints**.

For the cubic [Bézier curve](#bezier-curve) above, the [Bernstein basis](functional-analysis.md#bernstein-basis) influence function is $b_{1,3}(t)=3t(1-t)^2$. Its [derivative](calculus.md#derivative) is

$$
b_{1,3}'(t)=3(1-t)(1-3t).
$$

It increases up to $t=1/3$ and decreases thereafter on $[0,1]$. Consequently the largest displacement at corresponding parameters is

$$
\max_{0\leq t\leq1}\|\widetilde C(t)-C(t)\|=\frac49\|h\|,\qquad C(1/3)=\left(\frac{34}{27},\frac43\right),\qquad \widetilde C(1/3)=\left(\frac{34}{27},\frac{16}{9}\right).
$$

For $h=(0,1)$ it is $4/9$. This is a comparison at the same parameter. A geometric closest-distance comparison, as in a [closest-point search on a subdivision curve](#closest-point-search-on-a-subdivision-curve), instead minimizes over another parameter:

$$
d\bigl(C(t),\widetilde C([0,1])\bigr)=\min_{0\leq s\leq1}\|\widetilde C(s)-C(t)\|\leq\|\widetilde C(t)-C(t)\|.
$$

The closest parameter $s$ can differ from $t$, so $4/9$ is not automatically a maximum closest-distance separation of the two [curves](topology.md#curve). Neither parameter is assumed to be [arc length](riemannian-geometry.md#arc-length).

The [support of a function](function.md#support) $b_i$ is the closure of the parameter values where $b_i\ne0$. It bounds where a nonzero handle move can act, but may include boundary [points](geometry-and-topology.md#point-geometry) where the actual displacement is zero. Here the [support of a function](function.md#support) $b_{1,3}$ is all of $[0,1]$ relative to the parameter domain, while the endpoints are unaffected. In contrast, a [B-spline](uniform-approximation.md#b-spline) of order $k$ has [support](function.md#support) within $[t_i,t_{i+k}]$ in its [spline knot](uniform-approximation.md#spline-knot) sequence, so its handle affects only that parameter range; the [support and Gram bandwidth of B-splines](uniform-approximation.md#support-and-gram-bandwidth-of-b-splines) describes the same locality in another application. Changing the [spline knots](uniform-approximation.md#spline-knot) or the [basis](vector-space.md#basis) along with the handle requires a different comparison.

When the [basis](vector-space.md#basis) functions form a [partition of unity](smooth-manifold.md#partition-of-unity), $\sum_j b_j(t)=1$, each evaluation is an [affine combination](geometry-and-topology.md#affine-combination) of the [control points](#control-point). Applying an [affine map](geometry-and-topology.md#affine-map) $T(x)=Ax+a$ to all handles gives

$$
\sum_j b_j(t)T(P_j)=A C(t)+a=T(C(t)).
$$

This is [affine equivariance of a geometric basis](#affine-equivariance-of-a-geometric-basis), also called affine covariance: [affine maps preserve affine combinations](geometry-and-topology.md#affine-maps-preserve-affine-combinations). In particular, translating every handle by $h$ translates the whole [curve](topology.md#curve) by $h$, whereas moving just one handle produces $b_i(t)h$. The [Bernstein basis](functional-analysis.md#bernstein-basis) has this [partition of unity](smooth-manifold.md#partition-of-unity) property.[§4.3, pp. 132–133: Bernstein weights sum to one](mathematics-bibliography.md#curves-and-surfaces-in-geometric-modeling-theory-and-algorithms-by-jean-gallier) Nonnegative weights further make evaluations [convex combinations](convex-set.md#convex-combination), giving the [convex hull](convex-set.md#convex-hull) bound illustrated by the [control polygon](#control-polygon); nonnegativity is not needed for affine covariance.

For a proof outline of the influence formula, subtract the two [basis](vector-space.md#basis) representations: every unchanged [coefficient](vector-space.md#coefficient) cancels, leaving $b_i(t)(P_i+h)-b_i(t)P_i=b_i(t)h$. The same subtraction with several moved handles gives $\Delta C(t)=\sum_i b_i(t)h_i$. No claim about [interpolation](interpolation.md), [closest-point search on a subdivision curve](#closest-point-search-on-a-subdivision-curve) or endpoint motion follows until the actual [basis](vector-space.md#basis) values are examined.

### Control net

↑ **Parent:** [Control point](#control-point)

A mesh connecting a surface's [control points](#control-point) according to the representation's indexing topology. A [tensor-product surface basis](differential-geometry.md#tensor-product-surface-basis) gives a rectangular index grid and quadrilateral cells, even when its points in space are neither planar nor rectangular. The drawn mesh is a geometric skeleton, not generally the exact limit surface or an enclosing solid. Positive [partition of unity](smooth-manifold.md#partition-of-unity) coefficients give a [convex hull](convex-set.md#convex-hull) bound on the relevant controls.

### Control polygon

↑ **Parent:** [Control point](#control-point)

A [control polygon](#control-polygon) joins successive [control points](#control-point) by [line segments](convex-set.md#line-segment). It gives an editable geometric skeleton, not usually the exact [curve](topology.md#curve). An open [control polygon](#control-polygon) has two ends; a closed [control polygon](#control-polygon) also joins the last [control point](#control-point) to the first. Store the first [control point](#control-point) only once when using cyclic indices, so the closing edge is counted exactly once. Positive [partition of unity](smooth-manifold.md#partition-of-unity) basis functions place the [curve](topology.md#curve) inside the [convex hull](convex-set.md#convex-hull) of its active [control points](#control-point); a convergent [subdivision curve](#subdivision-curve) rule refines the [control polygon](#control-polygon) toward its limit, with a certified error when an appropriate bound is available.

## Apparent-gravity camera frame

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)

If $g$ is gravitational [acceleration](classical-mechanics.md#acceleration) and $a$ is the camera's [acceleration](classical-mechanics.md#acceleration), the locally felt upward vector is $U=a-g$. Choose the travel [unit vector](vector-space.md#unit-vector) $X$, set $W=U-(U\cdot X)X$, and, when $W\ne0$, take $Z=W/\|W\|$ and $Y=Z\times X$. These form an [orthonormal basis](inner-product.md#orthonormal-basis) with $U$ in the $XZ$ plane. If $U$ is parallel to $X$, the condition leaves the roll angle free even when $U\ne0$; transport a previous transverse axis or choose a well-conditioned coordinate axis and project it into $X^\perp$.

## Subdivision curve

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)

A [subdivision curve](#subdivision-curve) is the limit of repeated refinement of a [control polygon](#control-polygon), when that limit exists. Each finite stage still consists of [line segments](convex-set.md#line-segment); the limiting [curve](topology.md#curve) can have a [continuous](calculus.md#continuous-function) [derivative](calculus.md#derivative). Linear stationary rules, which use the same fixed weighted averages at every stage, can be studied through their [subdivision masks](#subdivision-mask) and often represent [splines](uniform-approximation.md#spline-mathematics). An [interpolation](interpolation.md) rule retains the old [control points](#control-point), as in [binary linear interpolatory subdivision](#binary-linear-interpolatory-subdivision); an approximating rule such as [Chaikin subdivision](#chaikin-subdivision) generally moves away from them. Increasing the number of [control points](#control-point) alone does not prove convergence or smoothness.

// Target: analysis.bigb

### Binary linear interpolatory subdivision

↑ **Parent:** [Subdivision curve](#subdivision-curve)

The centered [subdivision mask](#subdivision-mask) $[1,2,1]/2$ retains old [control points](#control-point) and inserts edge midpoints. Its [control polygon](#control-polygon) is unchanged as a geometric curve by refinement. Its basic limit is the hat $\phi(t)=\max(1-|t|,0)$, with support $[-1,1]$. This [linear spline](uniform-approximation.md#linear-spline) representation reproduces constants and linear functions, and is $C^0$ but generally not $C^1$ at its [spline knots](uniform-approximation.md#spline-knot).

### Functional precision set of a subdivision scheme

↑ **Parent:** [Subdivision curve](#subdivision-curve)

The [functional precision set of a subdivision scheme](#functional-precision-set-of-a-subdivision-scheme) consists of functions exactly reproduced by refining their uniform samples with the scheme's consistent parameter placement. Polynomial precision usually specifies the reproduced polynomial space. If exactness is required for every grid spacing and shift, the binary midpoint-interpolation scheme has precision exactly the [affine functions](vector-space.md#affine-function). At one fixed grid, its entire reconstruction range is the space of continuous [piecewise linear functions](function.md#piecewise-linear-function) on that grid; this larger range should not be confused with polynomial precision or arbitrary-grid reproduction.

### Chaikin subdivision

↑ **Parent:** [Subdivision curve](#subdivision-curve)

[Chaikin subdivision](#chaikin-subdivision) generates a rounded [subdivision curve](#subdivision-curve) by repeatedly cutting the corners off a [control polygon](#control-polygon). Each edge contributes two new [control points](#control-point), one a quarter of the way along the edge and the other three quarters of the way along it. Connecting these new [control points](#control-point) in edge order replaces the old corners by shorter [line segments](convex-set.md#line-segment). This makes [Chaikin subdivision](#chaikin-subdivision) a useful way to draw a smooth outline from a small, editable set of [control points](#control-point), without evaluating [B-spline](uniform-approximation.md#b-spline) basis functions at each drawing step. Joy presents both the corner-cutting rule and its closed version.[Kenneth I. Joy, Chaikin's Algorithms for Curves, §§Chaikin's Method and Example — A Closed Curve, UC Davis authored notes](https://www.cs.unc.edu/~dm/UNC/COMP258/LECTURES/Chaikins-Algorithm.pdf)

For a closed [control polygon](#control-polygon) with $n\geq3$ [control points](#control-point) $P_0,\ldots,P_{n-1}$, set $P_n=P_0$ and interpret indices cyclically. One refinement $S$ gives

$$
Q_i=\frac34P_i+\frac14P_{i+1},\qquad R_i=\frac14P_i+\frac34P_{i+1},\qquad 0\leq i<n,
$$

and the new [control polygon](#control-polygon) is the ordered sequence

$$
S(P)=(Q_0,R_0,Q_1,R_1,\ldots,Q_{n-1},R_{n-1}).
$$

Close it by joining $R_{n-1}$ back to $Q_0$. Use the old [control points](#control-point) for every average in the same refinement; updating them in place would define a different [algorithm](algorithm.md). One refinement produces $2n$ stored [control points](#control-point), and $k$ refinements produce $2^kn$, counting entries even if some coordinates coincide. Open [control polygons](#control-polygon) need an explicit endpoint convention: applying only the interior edge rule discards the original endpoints, whereas retaining endpoints changes the boundary rule. The closed analysis below uses cyclic indices throughout.

For a worked example, start with the rectangular [control polygon](#control-polygon)

$$
P_0=(0,0),\quad P_1=(4,0),\quad P_2=(4,2),\quad P_3=(0,2).
$$

The first edge gives $Q_0=\tfrac34(0,0)+\tfrac14(4,0)=(1,0)$ and $R_0=\tfrac14(0,0)+\tfrac34(4,0)=(3,0)$. Applying [Chaikin subdivision](#chaikin-subdivision) to all four edges, including the closing edge, gives exactly eight [control points](#control-point) in this order:

$$
(1,0),\ (3,0),\ (4,\tfrac12),\ (4,\tfrac32),\ (3,2),\ (1,2),\ (0,\tfrac32),\ (0,\tfrac12).
$$

Thus the rectangle becomes an octagonal [control polygon](#control-polygon). Two refinements have $16$ [control points](#control-point), and five have $128$. The illustration shows finite [control polygons](#control-polygon) at stages $0,1,2,5$; the last is already visually rounded but still consists of [line segments](convex-set.md#line-segment).

<a id="image-chaikin-corner-cutting-on-a-rectangle-at-iterations-zero-one-two-and-five"></a>
![](chaikin-corner-cutting-iterations.png)

**[Figure 3](#image-chaikin-corner-cutting-on-a-rectangle-at-iterations-zero-one-two-and-five). Chaikin corner cutting on a rectangle at iterations zero, one, two and five**. The dashed rectangle is the original [control polygon](#control-polygon) and its [convex hull](convex-set.md#convex-hull). Blue [line segments](convex-set.md#line-segment) and dots show the current [control polygon](#control-polygon) and [control points](#control-point); no panel claims to be the exact limiting [curve](topology.md#curve).

The [convex hull](convex-set.md#convex-hull) property follows directly from the weights. Each new [control point](#control-point) is a [convex combination](convex-set.md#convex-combination) of the endpoints of one old edge, because the weights are nonnegative and sum to one. Consequently, if $H_k$ is the [convex hull](convex-set.md#convex-hull) of the stage-$k$ [control points](#control-point), then $H_{k+1}\subseteq H_k$. Every later [line segment](convex-set.md#line-segment), and every limit point, stays in the original [convex hull](convex-set.md#convex-hull). This gives a useful geometric enclosure. It also explains why [Chaikin subdivision](#chaikin-subdivision) is approximating rather than an [interpolation](interpolation.md) rule: the rectangle's four original corners are outside the first octagon's [convex hull](convex-set.md#convex-hull), so the limiting [curve](topology.md#curve) cannot pass through them. A refinement [control polygon](#control-polygon) generally lies off the limiting [curve](topology.md#curve) as well.

For the cyclic uniform rule, the closed limit is the periodic quadratic uniform [B-spline](uniform-approximation.md#b-spline) [curve](topology.md#curve) determined by the original [control points](#control-point). Uniform refers to equal spacing in the [spline knot sequence](uniform-approximation.md#spline-knot-sequence), not equal physical lengths of edges of the [control polygon](#control-polygon). An infinite uniform control sequence has the corresponding local description; arbitrary open endpoint conventions need separate treatment. Joy derives the quarter-point refinement by splitting quadratic uniform [B-spline](uniform-approximation.md#b-spline) spans.[Kenneth I. Joy, Quadratic Uniform B-Spline Curve Refinement, §§Splitting and Refinement and The General Refinement Procedure, UC Davis authored notes](https://www.cs.unc.edu/~dm/UNC/COMP258/LECTURES/Quadratic-B-Spline-Curve-Refinement.pdf)

Here is an explicit description of that closed limit, with cyclic indices and a unit parameter span for each original [control point](#control-point):

$$
C_i(u)=\frac{(1-u)^2}{2}P_{i-1}+\left(\frac12+u-u^2\right)P_i+\frac{u^2}{2}P_{i+1},\qquad 0\leq u\leq1.
$$

Each coordinate is a [quadratic polynomial](polynomial.md#quadratic-polynomial), and the three coefficients form a nonnegative [partition of unity](smooth-manifold.md#partition-of-unity). The span runs from $(P_{i-1}+P_i)/2$ to $(P_i+P_{i+1})/2$. Differentiating gives $C_i'(0)=P_i-P_{i-1}$ and $C_i'(1)=P_{i+1}-P_i$, so adjacent spans have matching values and matching first [derivatives](calculus.md#derivative). Their second [derivatives](calculus.md#derivative) generally differ. Thus the parameterized [curve](topology.md#curve) is $C^1$, generally not $C^2$; degenerate [control points](#control-point) can still make its [tangent vector](tangent-vector.md) vanish. For the rectangle, the span around $P_1=(4,0)$ is

$$
C_1(u)=(2+4u-2u^2,\ u^2),\qquad C_1(\tfrac12)=(\tfrac72,\tfrac14),
$$

which rounds the original corner between edge midpoints $(2,0)$ and $(4,1)$. For equally spaced abscissae, the centered [Chaikin basis function](#chaikin-basis-function) gives the scalar graph version of this quadratic [B-spline](uniform-approximation.md#b-spline) representation and has support of width three original grid intervals.

Another useful property is [affine equivariance of a geometric basis](#affine-equivariance-of-a-geometric-basis): refining and applying an [affine map](geometry-and-topology.md#affine-map) commute. For $T(x)=Ax+b$,

$$
T(Q_i)=A\left(\frac34P_i+\frac14P_{i+1}\right)+b=\frac34T(P_i)+\frac14T(P_{i+1}),
$$

and the same calculation holds for $R_i$. The sum-to-one weights account for the [translation](geometry-and-topology.md#translation-geometry). Therefore $T(S(P))=S(T(P))$ at every refinement, and also for the limit. A designer can apply a [shear mapping](vector-space.md#shear-mapping), [translation](geometry-and-topology.md#translation-geometry), or other [affine map](geometry-and-topology.md#affine-map) to the original [control polygon](#control-polygon) and obtain exactly the transformed outline.

For example, compose the [shear mapping](vector-space.md#shear-mapping) $(x,y)\mapsto(x+y/2,y)$ with the [translation](geometry-and-topology.md#translation-geometry) $(1,-1)$ to obtain $T(x,y)=(x+y/2+1,y-1)$. The rectangle's [control points](#control-point) become $(1,-1),(5,-1),(6,1),(2,1)$. On its right edge, cutting first gives $Q_1=(4,1/2)$ and then $T(Q_1)=(21/4,-1/2)$. Transforming first and cutting instead gives $\tfrac34(5,-1)+\tfrac14(6,1)=(21/4,-1/2)$, the same [control point](#control-point).

<a id="image-shearing-and-translating-a-control-polygon-commutes-with-one-chaikin-refinement"></a>
![](chaikin-affine-equivariance.png)

**[Figure 4](#image-shearing-and-translating-a-control-polygon-commutes-with-one-chaikin-refinement). Shearing and translating a control polygon commutes with one Chaikin refinement**. Left: the rectangle and its first refinement. Right: the transformed [control polygon](#control-polygon), with blue dots from cutting after the [affine map](geometry-and-topology.md#affine-map) and orange rings from applying the [affine map](geometry-and-topology.md#affine-map) after cutting. All eight pairs coincide.

Historically, George M. Chaikin published “An algorithm for high-speed curve generation” in Computer Graphics and Image Processing 3(4), December 1974, pages 346–349. Its emphasis was practical curve generation through a recursive [algorithm](algorithm.md) using simple arithmetic, with applications including machine control and three-dimensional curves. The lasting appeal of [Chaikin subdivision](#chaikin-subdivision) is how an elementary local average creates an entire smooth [B-spline](uniform-approximation.md#b-spline) [curve](topology.md#curve).[G. M. Chaikin, An algorithm for high-speed curve generation, Computer Graphics and Image Processing 3(4), 346–349, 1974; publisher metadata and abstract](https://doi.org/10.1016/0146-664X(74)90028-8)

#### Chaikin basis function

↑ **Parent:** [Chaikin subdivision](#chaikin-subdivision)

This centered [quadratic cardinal B-spline](uniform-approximation.md#quadratic-cardinal-b-spline) weights each original control ordinate at its uniformly spaced abscissa. Its translates sum to one. It and its first [derivative](calculus.md#derivative) match at half-integer knots, while the second [derivative](calculus.md#derivative) can jump. The limit graph is $\sum_i y_i\beta((x-x_i)/h)$; one ordinate influences exactly three original intervals. Refinement of a quadratic adds $ah^2/4$ in the limit, yielding this basis by extending each three-point neighborhood quadratically.

#### Polynomial degree preservation under Chaikin subdivision

↑ **Parent:** [Chaikin subdivision](#chaikin-subdivision)

For uniformly spaced abscissae, quarter and three-quarter averages applied to constant or affine samples leave the same polynomial. For $P(x)=ax^2+bx+c$ on spacing $h$, both new subgrids lie on $P(x)+3ah^2/16$. For degree $n\geq3$, their candidate polynomial formulas differ with leading term $(h^3/32)P'''$, which has a nonzero highest-degree coefficient. Thus preservation of polynomial degree for arbitrary sufficiently long data sequences holds exactly for degrees zero, one and two, despite quadratic values changing.

### Support of a stationary subdivision scheme

↑ **Parent:** [Subdivision curve](#subdivision-curve)

Under $P_i^{\ell+1}=\sum_jM_{i-aj}P_j^\ell$, the descendants of control index zero lie at $a^{\ell-1}j_1+\cdots+j_\ell$, where each $j_k$ is in the mask support. Dividing by the refined parameter scale $a^\ell$ gives a limiting influence enclosure with the displayed endpoints. For a mask supported on $[-w,w]$ its width is $2w/(a-1)$ when the endpoints are active and a nonzero compactly supported basic limit exists. To prove exactness, the largest active mask term is the only surviving term near the right endpoint of the refinement equation, forcing $\beta=(\beta+j_{\max})/a$; the analogous left-end argument completes the result. Mask padding should be removed, and a nonconvergent rule has no limit support.

### Subdivision curve interrogation

↑ **Parent:** [Subdivision curve](#subdivision-curve)

A useful [subdivision curve](#subdivision-curve) interface provides parameter ranges, endpoint and limit evaluation, derivatives, subdivision into equivalent restricted pieces, a certified [bounding volume](#bounding-volume), and a certified error relative to a chord. Positive [subdivision masks](#subdivision-mask) often give a [convex hull](convex-set.md#convex-hull) bound. Masks with negative coefficients need a separate enclosing bound; their control-point hull need not enclose the limit curve.

#### Closest-point search on a subdivision curve

↑ **Parent:** [Subdivision curve interrogation](#subdivision-curve-interrogation)

At a regular differentiable interior nearest point of a [parametric curve](topology.md#parametric-curve), the displacement from the query point is perpendicular to the [tangent vector](tangent-vector.md). A [branch and bound](mathematical-optimization.md#branch-and-bound) search uses distances to certified enclosing [bounding volumes](#bounding-volume) as lower bounds, and evaluated limit points as upper bounds. Refine the most promising restricted pieces until the upper bound differs from the global lower bound by the chosen distance tolerance. Safeguarded [Newton root-finding iteration](numerical-analysis.md#newton-root-finding-iteration) accelerates local candidates, but endpoints, nonregular points, ties and other stationary branches must not be omitted.

#### Shadow tracing for a subdivision curve

↑ **Parent:** [Subdivision curve interrogation](#subdivision-curve-interrogation)

For a point light at $L$, the shadow of a curve point is the first surface intersection on its ray beyond that point. Certified patch bounds and subdivision isolate intersections; regular hits are corrected with a three-variable [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) solve. Differentiating the displayed equation gives $[S_u,S_v,-(C-L)](u',v',\lambda')^T=\lambda C'$, a predictor for continuation along the shadow. Surface boundaries and grazing rays require clipping and reseeding; every visible component must be isolated, rather than assumed detectable from a fixed sample of the casting curve.

#### Recursive half-space clipping of a subdivision curve

↑ **Parent:** [Subdivision curve interrogation](#subdivision-curve-interrogation)

For an oriented plane function $\ell$, certified extrema over a [bounding volume](#bounding-volume) allow a [subdivision curve](#subdivision-curve) piece to be rejected when $\max\ell<0$, or wholly retained when $\min\ell\geq0$. Otherwise subdivide. At an explicitly chosen rendering tolerance, a sufficiently flat, sufficiently short piece can be replaced by its clipped chord. This is an approximation, not a proof of exact crossing topology. Exact treatment of tangent contacts and small excursions requires root isolation of $\ell(C(t))$ and splitting into sign-constant intervals, when the curve representation supports such isolation.

## Subdivision surface

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subdivision_surface)

A [subdivision surface](#subdivision-surface) is the limit of repeated mesh refinement and vertex averaging. Exact interrogation evaluates this limit and, where defined, its [tangent vectors](tangent-vector.md) and [normal vectors](differential-geometry.md#normal-vector); a finite refined control mesh is generally only an approximation to the limit.

// Target: analysis.bigb

### Lateral artifacts of a subdivision surface

↑ **Parent:** [Subdivision surface](#subdivision-surface)

[Lateral artifacts of a subdivision surface](#lateral-artifacts-of-a-subdivision-surface) are unwanted variations along an intended straight extrusion: input cross-sections identical along a lattice direction acquire ripples in that direction under refinement. For a stationary arity-$m$ lattice rule $a_{i,j}$, extrusion along the first lattice coordinate is preserved exactly when $\sum_{i\equiv r\ (\mathrm{mod}\ m)}a_{i,j}$ is independent of the residue $r$ for every transverse offset $j$. Then summing along each row gives a single associated univariate [subdivision mask](#subdivision-mask). This direction-specific criterion does not promise invariance under every possible oblique extrusion.

#### Extrusion invariance of a ternary triangular scheme

↑ **Parent:** [Lateral artifacts of a subdivision surface](#lateral-artifacts-of-a-subdivision-surface)

If a triangular-lattice [subdivision mask](#subdivision-mask) has the displayed residue-sum equality, refining data $p_{i,j}=q_j$ gives $p'_{I,J}=\sum_k b_{J-3k}q_k$, independent of $I$. If affine coordinates reproduce their parameter positions, a geometrically straight extrusion is preserved. Rotationally symmetric masks give the corresponding property in all three lattice-edge directions. A boundary curve compatible with this extrusion uses the collapsed mask $b$, not just the central row of the two-dimensional mask.

### Mid-edge subdivision

↑ **Parent:** [Subdivision surface](#subdivision-surface)

Mid-edge subdivision replaces each mesh edge by its midpoint, joins successive midpoints around every old face, and joins successive midpoints around every old vertex. For an interior [manifold](topological-manifold.md) mesh, each new vertex has valence four. Each geometric update is a [convex combination](convex-set.md#convex-combination), so every refined control point remains in the [convex hull](convex-set.md#convex-hull) of the original control mesh. The regular limit is associated with the [quadratic four-direction box spline](uniform-approximation.md#quadratic-four-direction-box-spline).

#### Mid-edge facet centroid invariance

↑ **Parent:** [Mid-edge subdivision](#mid-edge-subdivision)

The descendant of a face with cyclic vertices $p_0,\ldots,p_{n-1}$ has vertices $p_i'=(p_i+p_{i+1})/2$. Their arithmetic mean is unchanged. On the cyclic [Fourier basis](fourier-series.md#fourier-basis), a mode of frequency $j$ is multiplied by $(1+e^{2\pi ij/n})/2$. Every nonconstant mode has modulus less than one, so the descendant face shrinks to the original vertex [centroid](euclidean-geometry.md#centroid). This puts that [centroid](euclidean-geometry.md#centroid) on the subdivision limit, without requiring the original face to be planar.

### Subdivision surface interrogation

↑ **Parent:** [Subdivision surface](#subdivision-surface)

Interrogation of a subdivision limit needs patch/topology navigation, refinement, limit evaluation and [derivatives](calculus.md#derivative) where they exist, with certified bounds and geometric error estimates. On regular patches one may use the corresponding spline representation. At [extraordinary subdivision vertices](#extraordinary-subdivision-vertex), local [subdivision matrices](#subdivision-matrix) determine limit positions and tangents under the scheme's smoothness conditions. A [normal vector](differential-geometry.md#normal-vector) may exist even when [second derivatives](calculus.md#second-derivative) and [Gaussian curvature](second-fundamental-form.md#gaussian-curvature) do not; finite refined polygons are approximations rather than exact limit queries.

#### Intersection of subdivision limit surfaces

↑ **Parent:** [Subdivision surface interrogation](#subdivision-surface-interrogation)

A robust intersection search applies [branch and bound](mathematical-optimization.md#branch-and-bound) to pairs of [subdivision surface](#subdivision-surface) patches. Certified [bounding volumes](#bounding-volume) reject disjoint pairs, and refinement reduces unresolved pairs. Limit evaluation, tangent data and controlled approximation bounds produce and correct local intersection arcs, then patch adjacency joins them. Bounds must enclose the limit, not merely the current mesh. Flat polygon intersections are approximations and can miss tiny components or tangencies unless the associated geometric and transversality conditions are verified.

#### Plane section of a subdivision surface

↑ **Parent:** [Subdivision surface interrogation](#subdivision-surface-interrogation)

A [plane section of a subdivision surface](#plane-section-of-a-subdivision-surface) is a zero set of the plane functional evaluated on the limit [parametric surface](differential-geometry.md#parametric-surface). Certified patch [bounding volumes](#bounding-volume) reject sign-definite patches. On a regular transverse section, $\nabla g\ne0$ and the parameter tangent is $(-g_v,g_u)$; predictor-corrector [continuation method](numerical-analysis.md#continuation-method) traces a branch after every component has been isolated. Closed loops, tangencies, coplanar patches and extraordinary-vertex neighborhoods require more than corner-sign tests. Degenerate sections can contain isolated points or two-dimensional portions rather than only regular curves.

#### Minimum distance between subdivision bodies

↑ **Parent:** [Subdivision surface interrogation](#subdivision-surface-interrogation)

For disjoint compact bodies, the minimum occurs on their boundaries. Patch [bounding volumes](#bounding-volume) give certified lower bounds and evaluated limit-point pairs give upper bounds. A [branch and bound](mathematical-optimization.md#branch-and-bound) search refines promising patch pairs until the global bounds differ by the tolerance. Boundary distance alone cannot detect containment; touching, crossing or nested solid bodies have ordinary set distance zero. Negative overlap values require an additional convention such as [translational penetration depth](#translational-penetration-depth).

### Extraordinary subdivision vertex

↑ **Parent:** [Subdivision surface](#subdivision-surface)

An [extraordinary subdivision vertex](#extraordinary-subdivision-vertex) has a valence different from that of the regular refinement lattice. Regular [box spline](uniform-approximation.md#box-spline) calculations do not alone establish smoothness at this vertex. The finite local [subdivision matrix](#subdivision-matrix), its [eigenvalues](linear-operator-theory.md#eigenvalue), and the associated [characteristic map of a subdivision surface](#characteristic-map-of-a-subdivision-surface) determine convergence and tangent behavior.

#### Characteristic map of a subdivision surface

↑ **Parent:** [Extraordinary subdivision vertex](#extraordinary-subdivision-vertex)

The [characteristic map of a subdivision surface](#characteristic-map-of-a-subdivision-surface) is the planar limit map obtained from the two independent tangent [eigenvectors](linear-operator-theory.md#eigenvector) of its local [subdivision matrix](#subdivision-matrix). In the usual stationary setting, a simple constant eigenvalue one, a semisimple double subdominant eigenvalue $0<\lambda<1$, strictly smaller other eigenvalues, and a regular injective characteristic map establish the standard $C^1$ tangent-plane behavior for nondegenerate data. The eigenvalue inequalities alone do not exclude a folded or singular characteristic map. For an alternating scheme these tests must use a full period of refinement.

### Quincunx subdivision

↑ **Parent:** [Subdivision surface](#subdivision-surface)

A regular [quincunx subdivision](#quincunx-subdivision) step replaces a square lattice by the union of its old vertices and face centres. In lattice indices one may use

$$
D=\begin{pmatrix}1&1\\1&-1\end{pmatrix},\qquad D^2=2I.
$$

Thus two steps give ordinary binary refinement. If $A(z,w)$ is the one-step [subdivision mask](#subdivision-mask) symbol, the two-step symbol is $A(z,w)A(zw,z/w)$. The two lattice parity classes separately determine the old-vertex and face-vertex stencils; their coefficient sums must each be one to reproduce constants.

### Loop subdivision surface

↑ **Parent:** [Subdivision surface](#subdivision-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_subdivision_surface)

On a regular triangular grid, [Loop subdivision](#loop-subdivision-surface) retains an old vertex with weight $10/16$ and adds its six neighbors with weight $1/16$ each. A new edge vertex has weights $3/8$ on the endpoints and $1/8$ on the two opposite vertices. Extraordinary vertices require valence-dependent rules.

// Target: analysis.bigb

#### Polynomial generation by regular Loop subdivision

↑ **Parent:** [Loop subdivision surface](#loop-subdivision-surface)

For the three unit-grid edge vectors $v_1,v_2,v_3$ and a [multivariate polynomial](polynomial.md#multivariate-polynomial) $f$ of total degree at most three, sampled regular-grid [Loop subdivision](#loop-subdivision-surface) generates the graph of $f+\frac1{12}\sum_{r=1}^3(v_r\cdot\nabla)^2f$. Thus affine polynomials are reproduced exactly and all polynomials through degree three retain their degree. Fourth-degree data constant along one edge direction reduce to a [Cardinal cubic B-spline](uniform-approximation.md#cardinal-cubic-b-spline), whose limit need not be a polynomial.

#### Extrusion invariance of Loop subdivision

↑ **Parent:** [Loop subdivision surface](#loop-subdivision-surface)

On an infinite regular triangular grid, height data constant along one edge direction remain constant along that direction under [Loop subdivision](#loop-subdivision-surface). Across rows the induced rule is $g'_{2j}=(g_{j-1}+6g_j+g_{j+1})/8$, $g'_{2j+1}=(g_j+g_{j+1})/2$, the centered [Cardinal cubic B-spline](uniform-approximation.md#cardinal-cubic-b-spline) rule.

// Target: analysis.bigb

### Subdivision mask

↑ **Parent:** [Subdivision surface](#subdivision-surface)

A stationary binary [subdivision mask](#subdivision-mask) $a$ specifies a refinement operator $q_j=\sum_i a_{j-2i}p_i$. Indices may be vectors for a surface. Coefficients restricted to a parity class give the stencil for one type of refined vertex.

// Target: analysis.bigb

#### Subdivision mask width

↑ **Parent:** [Subdivision mask](#subdivision-mask)

For a stationary univariate refinement $S_{ij}=a_{i-mj}$, the [subdivision mask width](#subdivision-mask-width) counts fine-grid positions from the first to the last active entry in a column, including any internal zeros. Consecutive columns are translates by $m$ rows, the [subdivision arity](#subdivision-arity). The number of old [control points](#control-point) used by a particular new point is instead the size of its row stencil; it need not equal the mask width. A span convention counts $w-1$ fine intervals, so numerical width claims should specify the convention.

#### Subdivision arity

↑ **Parent:** [Subdivision mask](#subdivision-mask)

The subdivision arity is the integer factor $a>1$ by which a stationary refinement shrinks parameter-grid intervals: control index $i$ has coordinate $i/a^\ell$ after $\ell$ levels. It is distinct from the mask width and from the number of neighbors in a stencil.

#### Subdivision difference scheme

↑ **Parent:** [Subdivision mask](#subdivision-mask)

For backward differences $\Delta P_i=P_i-P_{i-1}$, a [scalar](vector-space.md#scalar) stationary arity-$a$ [subdivision mask](#subdivision-mask) has symbol $M(z)=\sum_iM_i z^i$. The identity $(1-z)M(z)=B(z)(1-z^a)$ gives the displayed intertwining whenever the quotient is a finite [Laurent polynomial](polynomial.md#laurent-polynomial). Iterating supplies higher-difference masks. The coefficients $a^{r\ell}\Delta^rP_i^\ell$ are candidate $r$th-derivative controls. A convergent [derivative](calculus.md#derivative) scheme, proved by contraction of its first differences, establishes corresponding smoothness of the original limit under the standard consistent parameterization.

##### Norm and spectral bounds for subdivision regularity

↑ **Parent:** [Subdivision difference scheme](#subdivision-difference-scheme)

Finite local [subdivision matrices](#subdivision-matrix) for the scaled difference scheme track [derivative](calculus.md#derivative) variations in nested parameter intervals. A product-norm bound below one proves uniform contraction for every interval and therefore gives a [lower bound](set.md#lower-bound-in-a-partially-ordered-set) on [derivative](calculus.md#derivative) [continuity](calculus.md#continuous-function). A product [eigenvalue](linear-operator-theory.md#eigenvalue) of modulus at least one is an obstruction when its mode is reachable from the data and visible in the limit: generic data excite it, so the corresponding [derivative](calculus.md#derivative) differences fail to vanish. Harmless [polynomial](polynomial.md) or unobservable modes must be removed before applying such an [upper bound](set.md#upper-bound-in-a-partially-ordered-set). Borderline smoothness needs direct analysis, not rounding a numerical exponent. Stability and convergence of the underlying scheme must be checked rather than inferred from mask width.

#### Subdivision matrix

↑ **Parent:** [Subdivision mask](#subdivision-mask)

A local [subdivision matrix](#subdivision-matrix) maps the [control points](#control-point) in a refinement-invariant neighborhood to the refined neighborhood. Row sums one express constant reproduction. Its constant [eigenvector](linear-operator-theory.md#eigenvector) has [eigenvalue](linear-operator-theory.md#eigenvalue) one; remaining [eigenvalues](linear-operator-theory.md#eigenvalue) govern decay of shape modes. Near an [extraordinary subdivision vertex](#extraordinary-subdivision-vertex), tangent modes and a [characteristic map of a subdivision surface](#characteristic-map-of-a-subdivision-surface) are needed to test geometric smoothness, beyond simple convergence.

<h2 id="bezier-curve">Bézier curve</h2>

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bézier_curve)

A [Bézier curve](#bezier-curve) is a [parametric curve](topology.md#parametric-curve) specified by [control points](#control-point) $P_0,\ldots,P_n$ in a [Euclidean space](normed-vector-space.md#euclidean-norm) and the [Bernstein basis](functional-analysis.md#bernstein-basis):

$$
C(t)=\sum_{i=0}^n b_{i,n}(t)P_i,\qquad b_{i,n}(t)=\binom ni(1-t)^{n-i}t^i,\qquad 0\leq t\leq1.
$$

Here $\binom ni$ is a [binomial coefficient](binomial-coefficient.md). Each coordinate is a [polynomial](polynomial.md) of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $n$; special choices of [control points](#control-point) can lower the [polynomial degree](polynomial.md#degree-of-a-polynomial). The ordered [control points](#control-point) form the [control polygon](#control-polygon). A cubic [Bézier curve](#bezier-curve) uses four [control points](#control-point) and has the explicit form

$$
C(t)=(1-t)^3P_0+3(1-t)^2tP_1+3(1-t)t^2P_2+t^3P_3.
$$

The curve passes through $P_0$ and $P_3$; the interior [control points](#control-point) steer its shape and need not lie on it.[MIT 6.837, Bézier Curves and Splines, slides 23–31 and 45–47, 2012](https://ocw.mit.edu/courses/6-837-computer-graphics-fall-2012/aba8735cf2cf7c71ca5d29b46873309a_MIT6_837F12_Lec01.pdf)

For a worked example, choose

$$
P_0=(0,0),\qquad P_1=(1,2),\qquad P_2=(3,2),\qquad P_3=(4,0).
$$

Substituting these [control points](#control-point) gives

$$
C(t)=\bigl(3t+3t^2-2t^3,\;6t(1-t)\bigr),\qquad C(1/2)=\tfrac18P_0+\tfrac38P_1+\tfrac38P_2+\tfrac18P_3=(2,1.5).
$$

Here $y(t)=1.5-6(t-1/2)^2\leq1.5$, so neither interior [control point](#control-point), both at height $2$, lies on the curve. [De Casteljau's algorithm](#de-casteljau-s-algorithm) computes the same point using only successive [linear interpolations](function.md#linear-interpolation).

The endpoint [tangent vectors](tangent-vector.md) follow from the [Bézier derivative control polygon](#bezier-derivative-control-polygon):

$$
C'(0)=3(P_1-P_0)=(3,6),\qquad C'(1)=3(P_3-P_2)=(3,-6).
$$

Thus the curve leaves $P_0$ toward $P_1$ and arrives at $P_3$ from $P_2$. These nonzero [derivatives](calculus.md#derivative) determine the endpoint [tangent lines](calculus.md#tangent-line); if an endpoint [derivative](calculus.md#derivative) vanishes, that formula alone does not determine its tangent direction. Endpoint handles are useful when arranging a [parametric first-derivative join of Bézier curves](#parametric-first-derivative-join-of-bezier-curves).

The parameter $t$ is usually not [arc length](riemannian-geometry.md#arc-length). For this example,

$$
C'(t)=\bigl(3+6t-6t^2,\;6-12t\bigr),\qquad \|C'(0)\|=\sqrt{45},\qquad \|C'(1/2)\|=4.5.
$$

Equal steps in $t$ therefore do not generally travel equal distances. Distance along the curve is instead the [arc length](riemannian-geometry.md#arc-length), given by the [integral](integral.md) $s(t)=\int_0^t\|C'(u)\|\,du$; its [derivative](calculus.md#derivative) is the [norm](normed-vector-space.md#norm) of the [tangent vector](tangent-vector.md) and measures the rate of travel.

Two geometric facts make [Bézier curves](#bezier-curve) especially convenient for design. First, the [Bernstein basis](functional-analysis.md#bernstein-basis) weights are nonnegative and form a [partition of unity](smooth-manifold.md#partition-of-unity), since the [binomial theorem](binomial-coefficient.md#binomial-theorem) gives $\sum_i b_{i,n}(t)=((1-t)+t)^n=1$. Hence $C(t)$ is a [convex combination](convex-set.md#convex-combination) of the [control points](#control-point) and lies in their [convex hull](convex-set.md#convex-hull).[MIT 6.838, Bézier Curve and B-Spline Curve, §1.4.1, 1998](https://groups.csail.mit.edu/graphics/classes/6.838/S98/meetings/m15/) The [convex hull](convex-set.md#convex-hull) is the smallest [convex set](convex-set.md) containing the [control points](#control-point), not their [axis-aligned bounding box](#axis-aligned-bounding-box). Here it is a trapezoid, strictly smaller than $[0,4]\times[0,2]$: the box corner $(0,2)$ is outside the [convex hull](convex-set.md#convex-hull). The curve need not fill or touch every edge of either enclosure. The [convex hull](convex-set.md#convex-hull) guarantee concerns $0\leq t\leq1$; outside that interval weights can be negative.

Second, applying an [affine map](geometry-and-topology.md#affine-map) to every [control point](#control-point) gives exactly the same result as applying it to the entire curve. For $T(x)=Ax+b$,

$$
\sum_i b_{i,n}(t)T(P_i)=A\sum_i b_{i,n}(t)P_i+b\sum_i b_{i,n}(t)=T(C(t)).
$$

This is [affine equivariance of a geometric basis](#affine-equivariance-of-a-geometric-basis): a [translation](geometry-and-topology.md#translation-geometry), [rotation](riemannian-geometry.md#rotation-mathematics) or [shear mapping](vector-space.md#shear-mapping) can be performed on a handful of [control points](#control-point). For example, $T(x,y)=(2x+y,\;y+1)$ transforms the four [control points](#control-point) to $(0,1),(4,3),(8,3),(8,1)$ and transforms the midpoint to $(5.5,2.5)$, also obtained from the same weights $(1,3,3,1)/8$.

These editable handles explain the usefulness of [Bézier curves](#bezier-curve) in [computer aided geometric design](computer-aided-geometric-design.md), [vector graphics](computer-graphics.md#vector-graphics) paths and [outline fonts](typography.md#outline-font): a small collection of points controls an entire smooth stroke, and resizing the design preserves its mathematical shape. Cambridge's computer-graphics notes describe their use in graphic design, typography and PostScript outlines. The industrial context includes Pierre Bézier's work at Renault and Paul de Casteljau's work at Citroën.[Neil A. Dodgson and Peter Robinson, Cambridge Computer Graphics and Image Processing, slides 183 and 226–228, 2014](https://www.cl.cam.ac.uk/teaching/1415/CompGraph/cgip.pdf)

// Target: analysis.bigb

<h3 id="bezier-derivative-control-polygon">Bézier derivative control polygon</h3>

↑ **Parent:** [Bézier curve](#bezier-curve)

For a degree-$n$ [Bézier curve](#bezier-curve), the $r$th [derivative](calculus.md#derivative) has degree at most $n-r$ and [control points](#control-point) $n!\Delta^rP_j/(n-r)!$. The first [derivative](calculus.md#derivative) follows by differentiating the [Bernstein basis](functional-analysis.md#bernstein-basis) and shifting one summation index; iteration proves the general formula. A parameter interval of length $h$ multiplies these [derivative](calculus.md#derivative) controls by $h^{-r}$.

<h4 id="parametric-first-derivative-join-of-bezier-curves">Parametric first-derivative join of Bézier curves</h4>

↑ **Parent:** [Bézier derivative control polygon](#bezier-derivative-control-polygon)

Two adjacent [Bézier curves](#bezier-curve) of degrees $n,m$ and interval lengths $h,k$ have a $C^1$ join precisely when their endpoint positions and their [derivatives](calculus.md#derivative) in the common parameter agree. Parallel endpoint polygon edges alone give tangent-direction agreement; their scaled vectors must be equal for parametric first-derivative [continuity](calculus.md#continuous-function).

<h3 id="de-casteljau-s-algorithm">De Casteljau's algorithm</h3>

↑ **Parent:** [Bézier curve](#bezier-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/De_Casteljau's_algorithm)

[De Casteljau's algorithm](#de-casteljau-s-algorithm) evaluates a [Bézier curve](#bezier-curve) by repeated [linear interpolation](function.md#linear-interpolation) between neighboring [control points](#control-point). Fix $t\in[0,1]$, start with $P_i^{(0)}(t)=P_i$, and compute

$$
P_i^{(r)}(t)=(1-t)P_i^{(r-1)}(t)+tP_{i+1}^{(r-1)}(t),\qquad r=1,\ldots,n,\quad i=0,\ldots,n-r.
$$

Each new row has one fewer point. The final point is $P_0^{(n)}(t)=C(t)$. Use the same $t$ at every stage: it describes the fraction of each [line segment](convex-set.md#line-segment) traversed from its first endpoint toward its second. A cubic [Bézier curve](#bezier-curve) needs three levels containing $3$, $2$, and $1$ [linear interpolations](function.md#linear-interpolation), respectively.[Stanford CS348a, Handout 19, §2.3, pp. 10–11](https://graphics.stanford.edu/courses/cs164-10-spring/Handouts/handout19.pdf)

For the [Bézier curve](#bezier-curve) with [control points](#control-point) $P_0=(0,0)$, $P_1=(1,2)$, $P_2=(3,2)$, $P_3=(4,0)$, evaluation at $t=1/2$ takes the [midpoint](convex-set.md#midpoint) of every neighboring pair. The first level gives

$$
Q_0=\tfrac12(P_0+P_1)=(0.5,1),\qquad Q_1=\tfrac12(P_1+P_2)=(2,2),\qquad Q_2=\tfrac12(P_2+P_3)=(3.5,1).
$$

The second level gives

$$
R_0=\tfrac12(Q_0+Q_1)=(1.25,1.5),\qquad R_1=\tfrac12(Q_1+Q_2)=(2.75,1.5),
$$

and the third level gives

$$
S=\tfrac12(R_0+R_1)=(2,1.5)=C(1/2).
$$

The intermediate [control polygons](#control-polygon) shrink toward the evaluated point. Each step is a [convex combination](convex-set.md#convex-combination), giving a geometric explanation of the [convex hull](convex-set.md#convex-hull) property; every step also commutes with an [affine map](geometry-and-topology.md#affine-map).

<a id="image-cubic-bezier-curve-its-convex-hull-and-bounding-box-and-the-three-levels-of-de-casteljau-s-algorithm-at-t-1-2"></a>
![](bezier-de-casteljau-construction.png)

**[Figure 5](#image-cubic-bezier-curve-its-convex-hull-and-bounding-box-and-the-three-levels-of-de-casteljau-s-algorithm-at-t-1-2). Cubic Bézier curve, its convex hull and bounding box, and the three levels of De Casteljau's algorithm at t = 1/2**.

The same construction splits the [Bézier curve](#bezier-curve) exactly, with no approximation. The outer edges of the triangular array give the new [control points](#control-point): for a cubic, $(P_0,Q_0,R_0,S)$ specify the left piece and $(S,R_1,Q_2,P_3)$ specify the right piece.[Stanford CS348a, Handout 19, §2.3, p. 11, subsegment control points](https://graphics.stanford.edu/courses/cs164-10-spring/Handouts/handout19.pdf) At $t=1/2$ these two lists are

$$
L=\bigl((0,0),(0.5,1),(1.25,1.5),(2,1.5)\bigr),\qquad H=\bigl((2,1.5),(2.75,1.5),(3.5,1),(4,0)\bigr).
$$

Write $C_L$ and $C_H$ for the [Bézier curves](#bezier-curve) defined by these lists, each with its own parameter $u\in[0,1]$. Then

$$
C_L(u)=C(u/2),\qquad C_H(u)=C((1+u)/2).
$$

Their images reproduce the original curve, while their [derivatives](calculus.md#derivative) account for the shorter parameter intervals. At the join,

$$
C_L(1)=C_H(0)=S,\qquad C_L'(1)=3(S-R_0)=(2.25,0)=3(R_1-S)=C_H'(0).
$$

The [chain rule](calculus.md#chain-rule) gives $C_L'(1)=C_H'(0)=C'(1/2)/2$; in the original parameter, both pieces have [derivative](calculus.md#derivative) $(4.5,0)$. This is the interval scaling in the [parametric first-derivative join of Bézier curves](#parametric-first-derivative-join-of-bezier-curves).

<a id="image-exact-midpoint-subdivision-with-two-smaller-control-polygons-endpoint-tangent-directions-and-equally-spaced-parameter-samples"></a>
![](bezier-subdivision-and-tangents.png)

**[Figure 6](#image-exact-midpoint-subdivision-with-two-smaller-control-polygons-endpoint-tangent-directions-and-equally-spaced-parameter-samples). Exact midpoint subdivision with two smaller control polygons, endpoint tangent directions, and equally spaced parameter samples**.

Repeated [midpoint](convex-set.md#midpoint) splitting is useful for drawing [vector graphics](computer-graphics.md#vector-graphics) paths: each piece has a smaller [control polygon](#control-polygon) and its own [convex hull](convex-set.md#convex-hull) enclosure. A renderer can refine pieces until they are sufficiently close to [line segments](convex-set.md#line-segment) at the chosen display scale. Evaluating $C(t)$ and splitting it are thus two results of the same short [algorithm](algorithm.md).

For a proof outline, expanding the recursion gives

$$
P_i^{(r)}(t)=\sum_{j=0}^r\binom rj(1-t)^{r-j}t^jP_{i+j}.
$$

[Pascal's identity](binomial-coefficient.md#pascal-s-rule) proves this by [induction](foundations-of-mathematics.md#mathematical-induction); at $r=n$, $i=0$ it is precisely the [Bernstein basis](functional-analysis.md#bernstein-basis) formula for the [Bézier curve](#bezier-curve). The geometric construction remains useful even when expanding the [polynomial](polynomial.md) by hand would be cumbersome.

// Target: analysis.bigb

## Bounding volume

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bounding_volume)

A [bounding volume](#bounding-volume) is a simple enclosing [set](set.md) $B$ for an object $S$: every [point](geometry-and-topology.md#point-geometry) of $S$ belongs to $B$. Its purpose is to make a cheap rejection possible before examining the object itself. For example, an [axis-aligned bounding box](#axis-aligned-bounding-box) can enclose a [triangle](euclidean-geometry.md#triangle) using just its smallest and largest [coordinates](vector-space.md#coordinate-linear-algebra).

The guarantee is one-sided. If $S\subseteq B_S$ and $T\subseteq B_T$, then

$$
S\cap T\ne\varnothing\ \Longrightarrow\ B_S\cap B_T\ne\varnothing.
$$

Thus an empty [set intersection](set.md#set-intersection) of the [bounding volumes](#bounding-volume) certifies an empty [set intersection](set.md#set-intersection) of the objects. An overlap of the [bounding volumes](#bounding-volume) is necessary for actual intersection, but does not prove it. This is a [conservative enclosure test](#conservative-enclosure-test): rejection is conclusive, acceptance means further examination is needed.

Consider the filled [triangles](euclidean-geometry.md#triangle) $A$ with [vertices of a polygon](euclidean-geometry.md#vertex-of-a-polygon) $(0,0),(2,0),(0,2)$ and $B$ with [vertices of a polygon](euclidean-geometry.md#vertex-of-a-polygon) $(3/2,3/2),(7/2,3/2),(7/2,7/2)$. Their [axis-aligned bounding boxes](#axis-aligned-bounding-box) overlap in $[3/2,2]\times[3/2,2]$. Nevertheless, every [point](geometry-and-topology.md#point-geometry) of $A$ satisfies $x+y\leq2$, whereas every [point](geometry-and-topology.md#point-geometry) of $B$ satisfies $x+y\geq3$. The two [triangles](euclidean-geometry.md#triangle) are disjoint. The shaded square in the [bounding volume hierarchy](#bounding-volume-hierarchy) illustration makes this false candidate visible.

For [collision detection](#collision-detection), a [broad phase](#broad-phase) produces possible object pairs from [bounding volume](#bounding-volume) tests; a [narrow phase](#narrow-phase) examines the actual shapes, for example with a [triangle-triangle intersection algorithm](#triangle-triangle-intersection-algorithm). Scott Le Grand's [Chapter 32. Broad-Phase Collision Detection with CUDA](mathematics-bibliography.md#gpu-gems-3/chapter-32-broad-phase-collision-detection-with-cuda) explains this separation in its opening paragraphs. Whether touching counts as a [collision](classical-mechanics.md#collision) must be specified by the application.

An enclosure must cover the entire object being queried. A box fitted to samples of a [parametric curve](topology.md#parametric-curve) only guarantees enclosure of the sampled [points](geometry-and-topology.md#point-geometry), unless a separate bound covers the whole [parametric curve](topology.md#parametric-curve). For a [Bézier curve](#bezier-curve), the [convex hull](convex-set.md#convex-hull) of its [control points](#control-point) provides such a bound on its defining parameter [interval](real-analysis.md#interval-mathematics). In [floating-point arithmetic](floating-point-arithmetic.md), [outward rounding](numerical-analysis.md#outward-rounding) can preserve certified [coordinate](vector-space.md#coordinate-linear-algebra) bounds; an inward [roundoff error](numerical-analysis.md#round-off-error) can invalidate a rejection. Bounds must also be updated when objects move.

### Conservative enclosure test

↑ **Parent:** [Bounding volume](#bounding-volume)

A [conservative enclosure test](#conservative-enclosure-test) may retain disjoint objects as candidates, but must never reject a true [set intersection](set.md#set-intersection). Increasing an enclosure can add candidates while preserving this implication.

### Collision detection

↑ **Parent:** [Bounding volume](#bounding-volume)

[Collision detection](#collision-detection) determines whether geometric objects meet, under a specified convention for touching. A [bounding volume](#bounding-volume) test can reject a pair before a more detailed shape test.

#### Broad phase

↑ **Parent:** [Collision detection](#collision-detection)

The [broad phase](#broad-phase) generates candidate pairs with inexpensive [conservative enclosure tests](#conservative-enclosure-test). An accepted pair still needs the [narrow phase](#narrow-phase).

#### Narrow phase

↑ **Parent:** [Collision detection](#collision-detection)

The [narrow phase](#narrow-phase) checks the actual objects for candidates retained by the [broad phase](#broad-phase). Its numerical guarantees depend on the chosen shape test.

// Target: analysis.bigb

### Bounding volume hierarchy

↑ **Parent:** [Bounding volume](#bounding-volume)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bounding_volume_hierarchy)

A [bounding volume hierarchy](#bounding-volume-hierarchy) is a [data structure](data-structure.md) arranged as a [rooted tree](tree-graph-theory.md#rooted-tree): leaves store objects, and each internal node stores a [bounding volume](#bounding-volume) enclosing its [children in a rooted tree](tree-graph-theory.md#child-in-a-rooted-tree). Consequently, every node encloses all objects in its [subtree](data-structure.md#subtree). A common choice is a [binary tree](data-structure.md#binary-tree) of [axis-aligned bounding boxes](#axis-aligned-bounding-box). The objects assigned to sibling [subtrees](data-structure.md#subtree) can be different even when their [bounding volumes](#bounding-volume) overlap.[§7.3, opening paragraphs and Figure 7.3: leaves, descendant bounds and rejection of a subtree](mathematics-bibliography.md#physically-based-rendering-from-theory-to-implementation-4th-edition-by-matt-pharr-and-others/7-3-bounding-volume-hierarchies)

Here is an exact two-dimensional example. Use the [triangles](euclidean-geometry.md#triangle) $A,B$ from [bounding volume](#bounding-volume), together with $C$ having [vertices of a polygon](euclidean-geometry.md#vertex-of-a-polygon) $(6,0),(8,0),(6,2)$ and $D$ having [vertices of a polygon](euclidean-geometry.md#vertex-of-a-polygon) $(6,3),(8,3),(8,5)$. Group $A,B$ under $L$, and $C,D$ under $R$. Their parent [axis-aligned bounding boxes](#axis-aligned-bounding-box) and the box at the [root of a tree](tree-graph-theory.md#root-of-a-tree) are

$$
B_L=[0,7/2]\times[0,7/2],\qquad B_R=[6,8]\times[0,5],\qquad B_{\mathrm{root}}=[0,8]\times[0,5].
$$

The diagram shows all seven nodes. Taking the [coordinate](vector-space.md#coordinate-linear-algebra)-wise [minimum](set.md#minimum-of-a-subset-of-a-total-order) and [maximum](set.md#maximum-of-a-subset-of-a-total-order) of the two child boxes constructs each parent box; the resulting box contains the [set union](set.md#set-union) of the children, and can also contain empty space between them.

<a id="bounding-box-enclosures-and-hierarchy"></a>
![](bounding-box-enclosures-and-hierarchy.png)

**[Figure 7](#bounding-box-enclosures-and-hierarchy). Four exact triangles, their enclosing boxes, and a seven-node bounding volume hierarchy arranged as a binary tree**.

A [bounding volume hierarchy traversal](#bounding-volume-hierarchy-traversal) starts at the [root of a tree](tree-graph-theory.md#root-of-a-tree) and discards a [subtree](data-structure.md#subtree) when its [bounding volume](#bounding-volume) misses the query. Accepted internal nodes expose their children; accepted leaves supply candidates for actual shape tests. Box2D's official [Collision: Dynamic Tree](mathematics-bibliography.md#collision-dynamic-tree) describes [axis-aligned bounding box](#axis-aligned-bounding-box) region queries that return overlapping leaf boxes. A query box that bounds a different query shape can produce additional false candidates.

For the closed query [rectangle](euclidean-geometry.md#rectangle)

$$
Q=[8/5,9/5]\times[8/5,9/5],
$$

left-first [depth-first search](algorithm.md#depth-first-search) tests the node boxes in order: root, $L$, $A$, $B$, $R$. The first four overlap $Q$; $R$ does not, because its smallest $x$-[coordinate](vector-space.md#coordinate-linear-algebra) is $6>9/5$. Pruning $R$ skips both $C$ and $D$. Five box tests leave two [broad phase](#broad-phase) candidates. The [narrow phase](#narrow-phase) rejects $A$, since $x+y\geq16/5>2$ throughout $Q$, and accepts $B$: the [point](geometry-and-topology.md#point-geometry) $(7/4,13/8)$ belongs to both $Q$ and $B$. There are two detailed shape tests and one true hit.

<a id="bounding-volume-hierarchy-query-pruning"></a>
![](bounding-volume-hierarchy-query-pruning.png)

**[Figure 8](#bounding-volume-hierarchy-query-pruning). An exact rectangle query prunes the right subtree and leaves two box candidates but only one triangle hit**.

For a query asking for all intersections, [time complexity](theoretical-computer-science.md#time-complexity) depends on the number $v$ of visited nodes and the cost $T_j$ of each candidate shape test. With fixed dimension and constant bookkeeping cost per node, the work is

$$
O\!\left(v+\sum_{j=1}^{c}T_j\right),
$$

where $c$ counts candidate objects and $O$ is [Big O notation](real-analysis.md#big-o-notation). A balanced [binary tree](data-structure.md#binary-tree) has small [height of a binary tree](data-structure.md#height-of-a-binary-tree), but a query can enter both children at every level. In this example a query containing $[0,8]\times[0,5]$ visits all seven nodes and tests all four [triangles](euclidean-geometry.md#triangle). More generally, a [full binary tree](data-structure.md#full-binary-tree) with $n$ single-object leaves has $2n-1$ nodes, so such a query takes $O(n)$ work for constant-cost shape tests even when its [height of a binary tree](data-structure.md#height-of-a-binary-tree) is $O(\log n)$. Listing $n$ hits itself requires $n$ outputs. Small height alone gives no unconditional logarithmic query bound.

For [collision detection](#collision-detection) between two [bounding volume hierarchies](#bounding-volume-hierarchy), traverse pairs of nodes: reject disjoint pairs of [bounding volumes](#bounding-volume), expand a nonleaf member of an accepted pair, and apply the [narrow phase](#narrow-phase) at accepted leaf pairs. A single collection's self-query must exclude pairing an object with itself and avoid duplicate unordered pairs. If every object overlaps every other object, reporting all pairs already requires $n(n-1)/2$ results. Construction quality, empty space in boxes and the queries determine how much pruning is useful.[§32.1: the n(n−1)/2 pair baseline and worst-case quadratic broad-phase work](mathematics-bibliography.md#gpu-gems-3/chapter-32-broad-phase-collision-detection-with-cuda)

For a short correctness outline, an object is enclosed by its leaf box, and each child box is enclosed by its parent box. Repeated [subset](set.md#subset) relations carry this property to every ancestor. A true query intersection therefore prevents rejection at every ancestor of the object's leaf. Updating leaf boxes after motion also requires restoring all affected ancestor bounds before querying.

#### Bounding volume hierarchy traversal

↑ **Parent:** [Bounding volume hierarchy](#bounding-volume-hierarchy)

A [bounding volume hierarchy traversal](#bounding-volume-hierarchy-traversal) visits only nodes whose ancestors passed a [conservative enclosure test](#conservative-enclosure-test). It can use [depth-first search](algorithm.md#depth-first-search); its [time complexity](theoretical-computer-science.md#time-complexity) depends on how many nodes pass, not just the [height of a binary tree](data-structure.md#height-of-a-binary-tree).

// Target: optics.bigb

### Axis-aligned bounding box

↑ **Parent:** [Bounding volume](#bounding-volume)

An [axis-aligned bounding box](#axis-aligned-bounding-box) is a [Cartesian product](set-theory.md#cartesian-product) of [closed intervals](real-analysis.md#closed-real-interval) aligned with a chosen [Cartesian coordinate system](linear-algebra.md#cartesian-coordinate-system):

$$
B=\prod_{i=1}^{d}[m_i,M_i],\qquad m_i\leq M_i.
$$

Only the two opposite corners $(m_1,\ldots,m_d)$ and $(M_1,\ldots,M_d)$ need to be stored. In two dimensions it is a [rectangle](euclidean-geometry.md#rectangle). Changing the [Cartesian coordinate system](linear-algebra.md#cartesian-coordinate-system) can change how tightly the [axis-aligned bounding box](#axis-aligned-bounding-box) fits the same object.[§3.7, two-point representation and Figure 3.9](mathematics-bibliography.md#physically-based-rendering-from-theory-to-implementation-4th-edition-by-matt-pharr-and-others/3-7-bounding-boxes)

For a nonempty [finite set](set.md#finite-set) of [points](geometry-and-topology.md#point-geometry) $P$, the smallest such [axis-aligned bounding box](#axis-aligned-bounding-box) has

$$
m_i=\min_{p\in P}p_i,\qquad M_i=\max_{p\in P}p_i.
$$

These [minimum](set.md#minimum-of-a-subset-of-a-total-order) and [maximum](set.md#maximum-of-a-subset-of-a-total-order) values also enclose the [convex hull](convex-set.md#convex-hull) of $P$: each [coordinate](vector-space.md#coordinate-linear-algebra) of a [convex combination](convex-set.md#convex-combination) lies between the smallest and largest input [coordinates](vector-space.md#coordinate-linear-algebra). In particular, three [vertices of a polygon](euclidean-geometry.md#vertex-of-a-polygon) determine the [axis-aligned bounding box](#axis-aligned-bounding-box) of a filled [triangle](euclidean-geometry.md#triangle). For a general nonempty [compact set](topology.md#compact-space), the same formulas use all its [points](geometry-and-topology.md#point-geometry); inspecting only an arbitrary finite sample is insufficient.

Given nonempty boxes $B=\prod_i[m_i,M_i]$ and $C=\prod_i[n_i,N_i]$, the [closed interval](real-analysis.md#closed-real-interval) convention gives

$$
B\cap C\ne\varnothing\quad\Longleftrightarrow\quad
\max(m_i,n_i)\leq\min(M_i,N_i)\quad\text{for every }i.
$$

Equivalently, reject as soon as $M_i<n_i$ or $N_i<m_i$ in any [coordinate](vector-space.md#coordinate-linear-algebra). The surviving [set intersection](set.md#set-intersection) has endpoints $\max(m_i,n_i)$ and $\min(M_i,N_i)$. This is an exact box test, while its conclusion about enclosed objects remains a [conservative enclosure test](#conservative-enclosure-test).[§3.7, Intersect() and Overlaps(): coordinate-wise intersection and inclusive comparisons](mathematics-bibliography.md#physically-based-rendering-from-theory-to-implementation-4th-edition-by-matt-pharr-and-others/3-7-bounding-boxes)

Equality counts as touching: $[0,1]\times[0,1]$ and $[1,2]\times[0,1]$ share an edge, so their [set intersection](set.md#set-intersection) is nonempty. Replacing every $\leq$ in the overlap formula by $<$ tests intersection of the [interiors](topology.md#interior-topology) of full-dimensional boxes and excludes this contact. A zero-width [closed interval](real-analysis.md#closed-real-interval) can represent a [point](geometry-and-topology.md#point-geometry) or a lower-dimensional enclosure, and must not automatically be discarded when touching counts. A box with some $m_i>M_i$ is empty; test emptiness before applying rules intended for nonempty boxes. The [broad phase](#broad-phase) must retain touching candidates whenever the [narrow phase](#narrow-phase) counts touching as a hit.

For nonempty boxes, the smallest enclosing [axis-aligned bounding box](#axis-aligned-bounding-box) of their [set union](set.md#set-union) is

$$
\prod_{i=1}^{d}\bigl[\min(m_i,n_i),\max(M_i,N_i)\bigr].
$$

This operation supplies the parent boxes in a [bounding volume hierarchy](#bounding-volume-hierarchy). It is an enclosure of the [set union](set.md#set-union), rather than generally the [set union](set.md#set-union) itself. In [floating-point arithmetic](floating-point-arithmetic.md), comparisons are conclusive only for endpoints that still enclose the intended exact objects; use certified bounds such as [interval arithmetic](numerical-analysis.md#interval-arithmetic) with [outward rounding](numerical-analysis.md#outward-rounding) when that guarantee is required.

// Target: analysis.bigb

## Triangle-triangle intersection algorithm

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)

For two noncoplanar [triangles](euclidean-geometry.md#triangle), first reject vertices strictly on one side of the other triangle's plane. Otherwise intersect each triangle with the other plane and compare the resulting intervals along the common line. Coplanar triangles require a planar overlap test; zero-area triangles require separate [line segment](convex-set.md#line-segment) or point tests.

// Target: analysis.bigb

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Bézier curve](#bezier-curve)
- [Computer aided geometric design](computer-aided-geometric-design.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70.md#2/i/solution)
