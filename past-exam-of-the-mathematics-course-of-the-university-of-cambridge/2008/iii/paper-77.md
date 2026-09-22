# Paper 77

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper77.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper77.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)
  - [v](#5/v)
    - [Solution](#5/v/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let the [triangles](../../../geometry-and-topology.md#triangle) have vertices $A_0,A_1,A_2$ and $B_0,B_1,B_2$. Work initially with nonzero-area [triangles](../../../geometry-and-topology.md#triangle). A [triangle-triangle intersection algorithm](../../../numerical-analysis.md#triangle-triangle-intersection-algorithm) begins with the unnormalized [normal vector](../../../differential-geometry.md#normal-vector) $N_A=(A_1-A_0)\times(A_2-A_0)$ and the three signed plane evaluations $d_j=N_A\cdot(B_j-A_0)$. If all $d_j$ are strictly positive, or all strictly negative, the second [triangle](../../../geometry-and-topology.md#triangle) lies strictly on one side of the first one's plane, so the [triangles](../../../geometry-and-topology.md#triangle) are disjoint. Otherwise compute $N_B$ and $e_i=N_B\cdot(A_i-B_0)$ and apply the symmetric rejection test. Strict inequalities are important: contact on a vertex or edge counts as intersection.

If the planes are not parallel, put $L=N_A\times N_B$. Each [triangle](../../../geometry-and-topology.md#triangle) meets the other one's plane in an empty set, a point or a [line segment](../../../mathematical-optimization.md#line-segment). Its endpoints are obtained from zero-valued vertices and the edges whose endpoint plane evaluations have opposite signs. For example, an edge $B_jB_k$ contributes

$$
X=B_j+\frac{d_j}{d_j-d_k}(B_k-B_j).
$$

All these points lie on the common line of the two planes. Choose a coordinate $r$ for which $L_r\ne0$ and form the coordinate intervals $I_A=[a_-,a_+]$, $I_B=[b_-,b_+]$ of the two slices. This coordinate is one-to-one along the common line, so the exact final test is

$$
\boxed{\max(a_-,b_-)\le\min(a_+,b_+).}
$$

Only that coordinate of each slice endpoint needs to be evaluated; no full three-dimensional line parameterization is necessary.

Parallel planes which have survived the strict plane tests are coplanar. Drop the coordinate corresponding to the largest component of $N_A$ and test the two projected planar [triangles](../../../geometry-and-topology.md#triangle). For each edge of either projected [triangle](../../../geometry-and-topology.md#triangle), project both vertex sets onto the perpendicular direction. A strictly disjoint pair of projection intervals certifies separation. If none of the six edge directions separates them, the planar [convex sets](../../../mathematical-optimization.md#convex-set) overlap: a separating line for two disjoint convex polygons can be chosen parallel to an edge of one of them. This includes containment and boundary contact.

A zero [normal vector](../../../differential-geometry.md#normal-vector) signifies a degenerate [triangle](../../../geometry-and-topology.md#triangle); reduce its [convex hull](../../../mathematical-optimization.md#convex-hull) to a point or its extreme [line segment](../../../mathematical-optimization.md#line-segment) and use point containment or segment intersection instead. For floating-point input, reliable sign predicates and scale-aware error bounds are preferable to treating a tiny signed distance as an arbitrary exact zero. **Plane rejection followed by interval overlap, with a planar test for coplanar input, determines all nondegenerate cases.**

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Count scalar additions, subtractions, multiplications and divisions for the specific [triangle-triangle intersection algorithm](../../../numerical-analysis.md#triangle-triangle-intersection-algorithm) above; comparisons and index selection are separate. Computing one plane [normal vector](../../../differential-geometry.md#normal-vector) uses two vector differences, costing six subtractions, and one [cross product](../../../vector-space.md#cross-product), costing six multiplications and three subtractions. The three vertex-to-plane evaluations use nine further coordinate subtractions and three [dot products](../../../linear-algebra.md#dot-product), each with three multiplications and two additions. The first rejection test therefore costs

$$
\boxed{6+9+9+3(5)=39\text{ arithmetic operations}.}
$$

For randomly located [triangles](../../../geometry-and-topology.md#triangle) of characteristic size $a$ in a box of size $H\gg a$, a second [triangle](../../../geometry-and-topology.md#triangle) straddles the first triangle's plane only when its position is in a slab of relative thickness $O(a/H)$. Consequently the first plane test rejects almost every pair: the expected arithmetic count for this implementation is $39+O(a/H)$, with the constant in the remainder determined by the subsequent branches. This is an average count, rather than the assertion that every input needs 39 operations.

For a generic surviving noncoplanar pair, the symmetric plane test costs another 39 operations, the [cross product](../../../vector-space.md#cross-product) $N_A\times N_B$ costs nine, and each of the four slice endpoints needs five scalar operations in the selected coordinate: one subtraction and division for the interpolation fraction, then one subtraction, multiplication and addition for the coordinate. Thus this branch uses

$$
\boxed{39+39+9+4(5)=107\text{ operations}.}
$$

A fully executed coplanar test can use six planar edge directions. Each needs two subtractions to form its perpendicular and six two-dimensional [dot products](../../../linear-algebra.md#dot-product), costing $2+6(3)=20$ operations. Including both plane tests and the parallelism [cross product](../../../vector-space.md#cross-product) gives an upper count $78+9+120=207$ before any early exit. Contact and degeneracy can shorten or change these counts. Precomputed [normal vectors](../../../differential-geometry.md#normal-vector) or a preliminary [axis-aligned bounding box](../../../numerical-analysis.md#axis-aligned-bounding-box) test also change the answer: the latter uses only comparisons after its coordinate extrema are available. **The relevant small-triangle average is 39 operations for the specified plane-first implementation; a generic complete test uses 107.**

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Store a [bounding volume hierarchy](../../../numerical-analysis.md#bounding-volume-hierarchy) for each object, using [axis-aligned bounding boxes](../../../numerical-analysis.md#axis-aligned-bounding-box) or tighter enclosing volumes. A leaf contains one [triangle](../../../geometry-and-topology.md#triangle) or a small group; every internal node encloses all its descendants. Start with the two roots. If their [bounding volumes](../../../numerical-analysis.md#bounding-volume) are disjoint, discard that pair. Otherwise descend into children of one or both nodes, usually splitting the larger node, until overlapping leaf pairs are reached. Apply the exact [triangle-triangle intersection algorithm](../../../numerical-analysis.md#triangle-triangle-intersection-algorithm) only at these leaves, and stop at the first hit if only a yes/no answer is required. The pruning is sound because disjoint enclosing volumes imply disjoint enclosed [triangles](../../../geometry-and-topology.md#triangle).

A balanced [bounding volume hierarchy](../../../numerical-analysis.md#bounding-volume-hierarchy) typically takes $O(n\log n)$ work to construct and $O(n)$ storage. It can be reused for repeated queries and refitted when vertex positions move; a rigid transformation can also be handled in a common coordinate frame. Spatial grids or octrees provide another broad-phase strategy: place [triangles](../../../geometry-and-topology.md#triangle) in every cell they meet and test only pairs from common cells, suppressing duplicates. A box test is especially valuable because the small randomly distributed [triangles](../../../geometry-and-topology.md#triangle) almost always fail it.

For $n,m$ of order $10^5$, the naive method has about $10^{10}$ candidate pairs. Hierarchical pruning replaces this by the number of overlapping node pairs and actual candidate leaf pairs. No universal subquadratic worst-case bound follows: interpenetrating or very poorly separated meshes can still generate $nm$ candidates. If “intersection of objects” means overlap of solid volumes rather than intersection of their boundaries, add a point-in-solid containment test when no surface intersections are found; one closed object can lie wholly inside the other. **Use spatial enclosure to prune pairs before exact triangle tests.**

## 2

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

At $X=P(u,v)$, orient the unit [normal vector](../../../differential-geometry.md#normal-vector) $n=(P_u\times P_v)/\lVert P_u\times P_v\rVert$ towards the eye. Define the unit directions from the reflecting point to the source and eye by

$$
a=\frac{Q(t)-P(u,v)}{\lVert Q(t)-P(u,v)\rVert},\qquad b=\frac{E-P(u,v)}{\lVert E-P(u,v)\rVert}.
$$

The incident propagation direction is $-a$. The law of [specular reflection](../../../optics.md#specular-reflection) is $b=-a+2(a\cdot n)n$, so $a+b$ is normal to the surface. Conversely, if the tangential components of $a+b$ vanish and $a\cdot n,b\cdot n>0$, its unit-length summands have equal positive normal components and obey the reflection law. Therefore solve the two scalar equations

$$
\boxed{F(u,v,t)=\begin{pmatrix}(a+b)\cdot P_u\\(a+b)\cdot P_v\end{pmatrix}=0,\qquad (u,v,t)\in[0,1]^3,\quad a\cdot n>0.}
$$

The stated orientation condition gives $b\cdot n>0$. It removes the back-facing ambiguity, but not multiple images or caustics. Exclude $Q(t)=P(u,v)$ and $E=P(u,v)$, where these directions are undefined.

At a root where the $2\times3$ [Jacobian matrix](../../../calculus.md#jacobian-matrix) $DF$ has rank two, the [implicit function theorem](../../../calculus.md#implicit-function-theorem) makes the solution set a local curve in parameter space. Compute a unit tangent $w$ in its nullspace; equivalently take the normalized [cross product](../../../vector-space.md#cross-product) of the two rows of $DF$. A [continuation method](../../../numerical-analysis.md#continuation-method) predicts $x_p=x+h w$, where $x=(u,v,t)$, then corrects with the [Newton method](../../../mathematical-optimization.md#newton-s-method-in-optimization) applied to the three equations

$$
F(x_{\rm new})=0,\qquad w\cdot(x_{\rm new}-x_p)=0.
$$

The last equation fixes a transverse section and allows tracing through a turning point of $t$, where solving only for $(u,v)$ at successive fixed source parameters would fail. The corresponding space point is $R=P(u,v)$, with derivative $R'=P_u u'+P_v v'$ along the traced parameter-space curve.

Find initial roots by subdividing the parameter cube, using [interval arithmetic](../../../numerical-analysis.md#interval-arithmetic) bounds on $F$ to discard impossible boxes and validated local solves in the remaining boxes. Trace in both directions, stop at the boundary or a recognized closed loop, and retain a record of traced boxes to avoid duplicates. Search the remaining boxes as well: starting from just one seed would miss disconnected closed reflection curves. Where $DF$ loses rank, reduce the step and subdivide locally to find the outgoing branches instead of continuing a single guessed tangent. If physical visibility is required, discard roots for which either open segment $XE$ or $XQ(t)$ is occluded; test these segments against the surface or any supplied scene geometry.

Control the geometric approximation rather than just the parameter step. For any regular traced arc $R(s)$ with a bound $\lVert R''(s)\rVert\le M$, the [chord error bound](../../../numerical-analysis.md#chord-error-bound) gives an arc-to-chord [Hausdorff distance](../../../topological-analysis.md#hausdorff-distance) at most $M(\Delta s)^2/8$. Budget, for example, half of $\epsilon$ for corrected-vertex error and half for chord error; accept a segment only when

$$
\boxed{\delta_{\rm vertex}\le\epsilon/2,\qquad M(\Delta s)^2/8\le\epsilon/2.}
$$

Bound the vertex error through the inverse transverse [Jacobian matrix](../../../calculus.md#jacobian-matrix) and a bound on $DP$, or use validated root enclosures. If analytic second-derivative bounds are unavailable, recursively subdivide and enclose each arc in a geometric tube of radius at most the remaining tolerance around its chord. A midpoint test alone is a useful heuristic but cannot certify the requested error for an arbitrary oscillatory curve.

The returned vertices $P(u_k,v_k)$ and their ordered connecting segments give the reflection curve to the prescribed tolerance on every resolved branch. Finite certified termination requires regular evaluable patches, derivative or enclosure bounds, and finitely resolvable branches; eye-facing normals alone do not guarantee these properties. Singular components or an identically vanishing reflection constraint must be handled as such rather than silently reported as an ordinary curve.

## 3

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Write a degree-$p$ [B-spline](../../../uniform-approximation.md#b-spline) as $C(t)=\sum_iP_iN_{i,p}(t)$ and locate its [spline knot](../../../uniform-approximation.md#spline-knot) span. There are several equivalent exact evaluation methods.

Evaluate the at most $p+1$ nonzero basis functions by the [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula), then form their weighted sum of control points. Alternatively apply [De Boor's algorithm](../../../uniform-approximation.md#de-boor-s-algorithm) directly to the $p+1$ active control points. In a span $[t_k,t_{k+1})$, initialize $d_j^{(0)}=P_{k-p+j}$ and repeatedly interpolate:

$$
d_j^{(r)}=(1-\alpha_{j,r})d_{j-1}^{(r-1)}+\alpha_{j,r}d_j^{(r-1)},\qquad \alpha_{j,r}=\frac{t-t_{k-p+j}}{t_{k+1+j-r}-t_{k-p+j}},
$$

for $r=1,\ldots,p$ and $j=p,p-1,\ldots,r$. The last point $d_p^{(p)}$ is $C(t)$; zero knot intervals are handled by the standard limiting convention or an appropriate neighboring nonempty span.

A third method precomputes the local polynomial coefficients on each span and evaluates them by [Horner's method](../../../polynomial.md#horner-s-method). For a uniform cubic [B-spline](../../../uniform-approximation.md#b-spline), a fixed four-by-four basis matrix gives these coefficients. A fourth method uses [knot insertion](../../../uniform-approximation.md#knot-insertion) to express the relevant span as a [Bézier curve](../../../numerical-analysis.md#bezier-curve), followed by [De Casteljau's algorithm](../../../numerical-analysis.md#de-casteljau-s-algorithm). Both interpolation algorithms also split the curve at the requested parameter. Repeated subdivision supplies arbitrarily accurate polygonal evaluation, although a finite subdivision mesh is generally an approximation rather than the exact requested point. **Basis summation, de Boor interpolation, local polynomial evaluation and Bézier extraction are equivalent exact representations.**

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula) and [De Boor's algorithm](../../../uniform-approximation.md#de-boor-s-algorithm) handle nonuniform knots and repeated knots without converting the whole curve. With a tabulated recurrence they require $O(p^2)$ arithmetic after locating the span and use only local control points; a naive recursive basis evaluation wastes work by recomputing the same terms. [De Boor's algorithm](../../../uniform-approximation.md#de-boor-s-algorithm) evaluates the vector directly using affine combinations. Inside the span these are convex combinations, which makes the geometric construction transparent and avoids the cancellation that can occur in a power-basis representation. Basis evaluation is especially useful when the same knots and parameter are shared by many coordinate functions or many curves, since the weights can be reused.

Precomputed power coefficients followed by [Horner's method](../../../polynomial.md#horner-s-method) need only $O(p)$ arithmetic per coordinate and are attractive for many evaluations within an unchanged span, particularly for fixed-degree uniform [B-splines](../../../uniform-approximation.md#b-spline). Coefficient construction has an initial cost, control-point edits require updates to affected spans, and poor scaling of high-degree power coefficients can damage accuracy. Rescaling each span to $[0,1]$ helps. [Bézier curve](../../../numerical-analysis.md#bezier-curve) extraction has a similar initial conversion cost; [De Casteljau's algorithm](../../../numerical-analysis.md#de-casteljau-s-algorithm) then gives stable local evaluation, subdivision, a [convex hull](../../../mathematical-optimization.md#convex-hull) bound and geometric flatness tests useful for rendering and intersection.

Subdivision is convenient when an entire polygonal approximation is wanted: refine only where needed and reuse the hierarchy. It is less economical for a single prescribed parameter and requires a geometric error bound before its approximate point can replace exact evaluation. Span lookup itself costs $O(\log n)$ for sorted arbitrary knots, constant work for a uniform interior span, or amortized constant work for an ordered sequence of sample parameters. **Use de Boor for robust general knots, shared basis weights for batches, and precomputed local polynomials or Bézier pieces for repeated interrogation.**

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Use unit knot spacing and the centered [Cardinal cubic B-spline](../../../uniform-approximation.md#cardinal-cubic-b-spline) convention $C(t)=\sum_iP_iM_3(t-i)$, where $M_3$ is supported on $[-2,2]$. On the span $[i,i+1]$, with $s=t-i$, the active control points are $P_{i-1},P_i,P_{i+1},P_{i+2}$, and their [B-spline](../../../uniform-approximation.md#b-spline) weights are

$$
(b_0,b_1,b_2,b_3)=\frac16\big((1-s)^3,\;3s^3-6s^2+4,\;-3s^3+3s^2+3s+1,\;s^3\big).
$$

For $t=11/4$, take $i=2$, $s=3/4$. The weights and their [derivatives](../../../calculus.md#derivative) are

$$
(b_0,b_1,b_2,b_3)=\frac1{384}(1,121,235,27),\qquad (b'_0,b'_1,b'_2,b'_3)=\frac1{32}(-1,-21,13,9).
$$

The PDF has $P_3=(0,0,0)$ and $P_4=(0,1,0)$, so the point and [tangent vector](../../../differential-geometry.md#tangent-vector) are

$$
C(11/4)=\frac{P_1+121P_2+235P_3+27P_4}{384},\qquad C'(11/4)=\frac{-P_1-21P_2+13P_3+9P_4}{32}.
$$

Thus, under this centered convention,

$$
\boxed{C(11/4)=\left(\frac{61}{192},\frac7{96},\frac{61}{192}\right),\qquad C'(11/4)=\left(-\frac{11}{16},\frac14,-\frac{11}{16}\right).}
$$

The original PDF specifies neither the knot origin nor its indexing relative to $P_i$. If instead the convention associates span $[i,i+1]$ with $P_i,P_{i+1},P_{i+2},P_{i+3}$, the identical local weights multiply $P_2,P_3,P_4,P_5$ at the requested parameter, giving

$$
\boxed{C(11/4)=\left(-\frac{13}{192},\frac{131}{192},\frac7{96}\right),\qquad C'(11/4)=\left(-\frac5{16},\frac{11}{16},\frac14\right).}
$$

These are parameter translations of the same uniform construction, rather than contradictory evaluations with the same knots. A specified knot convention is necessary to select the numerical pair uniquely; changing the knot spacing would also rescale the [derivative](../../../calculus.md#derivative).

## 4

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

A [parallel surface](../../../differential-geometry.md#parallel-surface) at signed distance $d$ from a design surface describes a constant-thickness skin, shell, coating or clearance envelope. A particularly important application is machining with a spherical cutter of radius $r$: when the cutter touches $P$ without penetration, its center lies at $P+r n$, where $n$ is the outward unit [normal vector](../../../differential-geometry.md#normal-vector). Thus a tool-center path can be computed on the [surface offset](../../../differential-geometry.md#parallel-surface) rather than on the desired contact surface. Positive and negative [surface offsets](../../../differential-geometry.md#parallel-surface) also model material addition and removal, and pairs of offsets describe the two faces of a thin manufactured wall. **Offsets convert contact, thickness and clearance specifications into geometric surfaces which can be interrogated.**

The construction is initially local. Where the offset develops self-intersections or reaches a curvature radius, not every point of the raw [parallel surface](../../../differential-geometry.md#parallel-surface) is a usable physical boundary. Tool paths and solid envelopes may require trimming those pieces and checking global collisions.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For a regular [parametric surface](../../../differential-geometry.md#parametric-surface) $P(u,v)$, form $N=P_u\times P_v$, $n=N/\lVert N\rVert$ and define the offset evaluator

$$
\boxed{P_d(u,v)=P(u,v)+d\,n(u,v).}
$$

It is already a [parametric surface](../../../differential-geometry.md#parametric-surface) with the same parameter domain, even if its coordinates no longer belong to the original polynomial or rational patch family. Point interrogation requires evaluations of $P,P_u,P_v$ and one normalization. For tangent or [normal vector](../../../differential-geometry.md#normal-vector) interrogation, differentiate the evaluator. For example,

$$
N_u=P_{uu}\times P_v+P_u\times P_{uv},\qquad n_u=\frac{(I-nn^T)N_u}{\lVert N\rVert},\qquad (P_d)_u=P_u+d n_u,
$$

and similarly for $v$. The offset [normal vector](../../../differential-geometry.md#normal-vector) is the normalized [cross product](../../../vector-space.md#cross-product) $(P_d)_u\times(P_d)_v$ wherever it is nonzero. These derivatives also support intersection, projection and curvature calculations by the usual methods for [parametric surfaces](../../../differential-geometry.md#parametric-surface). For a [variable normal offset](../../../differential-geometry.md#variable-normal-offset), add $d_u n$ and $d_v n$ to the corresponding tangent derivatives.

With [shape operator](../../../second-fundamental-form.md#shape-operator) $W=-Dn$, the constant-distance offset differential is $DP_d=(I-dW)DP$. Along a principal direction its factor is $1-d\kappa_i$, where $\kappa_i$ is a [principal curvature](../../../second-fundamental-form.md#principal-curvature). Consequently regular interrogation fails at $d\kappa_i=1$; on regular pieces the offset principal curvatures are $\kappa_i/(1-d\kappa_i)$ with the continued normal orientation. Global self-intersections can occur even when both local factors are nonzero. **Evaluate and differentiate the base surface and its normalized normal; an exact conversion back to the original patch type is unnecessary.**

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Treat the [subdivision surface](../../../numerical-analysis.md#subdivision-surface) as an evaluable limit together with its refinement hierarchy. At a requested location $\xi$, evaluate the limit position $S(\xi)$ and two independent limit [tangent vectors](../../../differential-geometry.md#tangent-vector), then set

$$
\boxed{S_d(\xi)=S(\xi)+d\,\frac{S_1(\xi)\times S_2(\xi)}{\lVert S_1(\xi)\times S_2(\xi)\rVert}.}
$$

On regular regions, local spline patches supply position and derivative evaluations. Near extraordinary vertices, use the actual subdivision rule and its limit-position and tangent evaluation machinery, or a convergent local refinement with controlled position and [normal vector](../../../differential-geometry.md#normal-vector) errors. If a tangent pair degenerates, the regular offset evaluator is not defined there; a crease requires separate one-sided offsets and an explicitly chosen join.

For polygonal interrogation, subdivide the base mesh adaptively. At every new sample, evaluate the base limit and its limit [normal vector](../../../differential-geometry.md#normal-vector), and displace that sample by $d n$. Connect these samples with the inherited connectivity, refining until flatness and normal-variation bounds meet the desired tolerance. If the position error is $\delta$ and unit-normal error is $\eta$, the offset-position error is at most $\delta+|d|\eta$, in addition to the interpolation error between samples. A [variable normal offset](../../../differential-geometry.md#variable-normal-offset) can be sampled at the same locations, with its approximation error included as well. The result retains the base subdivision hierarchy for locating points and refining patches.

Displacing the original control vertices along estimated vertex normals and applying the original [subdivision mask](../../../numerical-analysis.md#subdivision-mask) just once does not, in general, give the exact [surface offset](../../../differential-geometry.md#parallel-surface). If $A$ is one linear refinement step, then $A(P+d n(P))=AP+d A n(P)$, while displacing the refined base gives $AP+d n(AP)$; normalization and the normal calculation are nonlinear, so $A n(P)\ne n(AP)$ in general. Thus the exact offset is an interrogation wrapper around the base limit, and a conventional subdivision control mesh for it is a fitted approximation requiring refinement or error control. **Refine and interrogate the base limit, then offset its evaluated points; do not assume offsetting commutes with subdivision.**

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

A practical family consists of constant-distance [parallel surfaces](../../../differential-geometry.md#parallel-surface) and smooth [variable normal offsets](../../../differential-geometry.md#variable-normal-offset)

$$
\boxed{P_d(u,v)=P(u,v)+d(u,v)n(u,v),\qquad d(u,v)\text{ represented by a low-degree scalar spline}.}
$$

Constants cover wall thickness, cutter radius and clearance. A scalar [B-spline](../../../uniform-approximation.md#b-spline) or piecewise [polynomial](../../../polynomial.md) displacement field permits thickness variation, local bumps and smooth blending; compact support makes local edits economical. Use the base parameterization or compatible data on its subdivision hierarchy so that evaluating the displacement and its [derivatives](../../../calculus.md#derivative) requires only a small local stencil. Choose displacement size and gradients to avoid unintended folds, and trim global self-intersections where the physical application requires an envelope. A constant displacement smaller than the local curvature radii prevents the corresponding local focal singularities, although global clearance still needs a separate check.

When remaining within a polynomial or rational representation is more useful than prescribing an exact distance, a related practical form is $P+\lambda(u,v)(P_u\times P_v)$ with a low-degree scalar field $\lambda$. Its displacement is normal but has magnitude $|\lambda|\lVert P_u\times P_v\rVert$, so it is not a constant-distance [parallel surface](../../../differential-geometry.md#parallel-surface). For polynomial $P$ and $\lambda$, it stays polynomial; for rational input it stays rational. More general low-degree vector displacement fields similarly preserve efficient evaluation, while relinquishing the normal-offset condition. These forms make explicit the tradeoff between an exact metric offset, which involves normalization, and an easily represented deformation. **Simple scalar normal-displacement fields are useful and directly evaluable; algebraic displacement fields are useful when representation closure is required.**

## 5

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

The supplied [subdivision mask](../../../numerical-analysis.md#subdivision-mask) describes the regular, valence-six triangular grid. Its coefficients split into four parity classes after binary refinement: one class for old vertices and three classes for the three edge directions. For an old vertex $V$ with cyclic neighbors $V_1,\ldots,V_6$, the even stencil is

$$
\boxed{V'=\frac{10V+V_1+\cdots+V_6}{16}=\frac58V+\frac1{16}\sum_{r=1}^6V_r.}
$$

For an edge with endpoints $A,B$ and opposite vertices $C,D$ in its two incident [triangles](../../../geometry-and-topology.md#triangle), the new odd vertex is

$$
\boxed{M'=\frac{6A+6B+2C+2D}{16}=\frac38(A+B)+\frac18(C+D).}
$$

Rotating this edge stencil supplies the other two odd parity classes. All stencil weights sum to one, giving affine invariance; their first moments place an affine regular grid at the old positions and edge midpoints. Apply the same weights separately to $x,y,z$. Boundary edges and extraordinary vertices need additional rules, which are not specified by this uniform mask. The subsequent arguments concern the regular interior grid and compatible extruded boundary treatment.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Choose one grid-edge vector $a$ as the extrusion direction and an independent edge vector $b$. Label grid points $r_{i,j}=ia+jb$, so extruded height data have $z_{i,j}=g_j$, independent of $i$. The [Loop subdivision](../../../numerical-analysis.md#loop-subdivision-surface) stencils are affine-exact in the $x,y$ coordinates, so the refined horizontal grid has spacing one-half and the same row structure.

At an old vertex, two neighbors lie in its own row, two in the row above and two in the row below. Its refined height is therefore

$$
g'_{2j}=\frac{10g_j+2g_j+2g_{j-1}+2g_{j+1}}{16}=\frac{g_{j-1}+6g_j+g_{j+1}}8.
$$

A new vertex on an edge parallel to $a$ has both endpoints in row $j$ and its opposite vertices in rows $j-1,j+1$, giving exactly the same value $g'_{2j}$. A new vertex on either of the other edge directions has endpoints in rows $j,j+1$; its two opposite vertices are also one in each of these rows. Its height is

$$
g'_{2j+1}=\frac{3(g_j+g_{j+1})+(g_j+g_{j+1})}{8}=\frac{g_j+g_{j+1}}2.
$$

Every refined vertex in a given row consequently has the same height. Induction proves this at every refinement level. The piecewise planar interpolating mesh is also constant along $a$ between rows, since adjacent rows have constant heights and form parallel straight lines. Taking its convergent limit preserves this invariance. Thus

$$
\boxed{z_\infty(r+\lambda a)=z_\infty(r)}
$$

where the points lie in the domain. The limit [subdivision surface](../../../numerical-analysis.md#subdivision-surface) is an extrusion of the univariate limit curve. This is a statement about functional data on the regular grid, not about an arbitrary spatial mesh with extraordinary vertices or independently imposed boundary stencils.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

The transverse row sequence in the [extrusion invariance of Loop subdivision](../../../numerical-analysis.md#extrusion-invariance-of-loop-subdivision) obeys

$$
\boxed{g'_{2j}=\frac{g_{j-1}+6g_j+g_{j+1}}8,\qquad g'_{2j+1}=\frac{g_j+g_{j+1}}2.}
$$

In the convention $g'_k=\sum_j a_{k-2j}g_j$, the centered univariate [subdivision mask](../../../numerical-analysis.md#subdivision-mask) is

$$
\boxed{(a_{-2},a_{-1},a_0,a_1,a_2)=\frac18(1,4,6,4,1).}
$$

The even coefficients sum to one and the odd coefficients sum to one; the whole binary mask sums to two. Its generating expression is $a(z)=z^{-2}(1+z)^4/8$, identifying the [Cardinal cubic B-spline](../../../uniform-approximation.md#cardinal-cubic-b-spline) refinement rule. Its limit is $G(y)=\sum_jg_jM_3(y-j)$ for the centered unit-grid cubic basis $M_3$. The curve across rows is this cubic [B-spline](../../../uniform-approximation.md#b-spline); extrusion generates the whole limit surface. The along-extrusion direction itself has constant height, so its profile is a straight line rather than an additional nonconstant cubic curve.

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

Interpret polynomial reproduction as a guarantee for every [polynomial](../../../polynomial.md) of degree at most $d$, with the planar grid coordinates fixed by the affine-exact refinement. Constants are unchanged because every stencil sums to one. Linear height functions are unchanged because each stencil's weighted position is its refined grid location. Therefore the [Loop subdivision](../../../numerical-analysis.md#loop-subdivision-surface) limit reproduces all affine polynomials exactly.

Quadratic data already disprove the next degree. Use extruded data $g_j=j^2$ on a unit-spaced transverse row coordinate $y$. At spacing $h$, both even and odd rules from the induced [subdivision mask](../../../numerical-analysis.md#subdivision-mask) give the value of $y^2$ at the refined location plus $h^2/4$. For the even stencil this follows from

$$
\frac{(y-h)^2+6y^2+(y+h)^2}{8}=y^2+\frac{h^2}4,
$$

and for the odd stencil from the average of the values at $y-h/2$ and $y+h/2$. Constants are reproduced, so the accumulated vertical displacement over all refinement levels is

$$
\sum_{\ell=0}^\infty\frac{4^{-\ell}}4=\frac13.
$$

The limit is $y^2+1/3$, not the original quadratic graph. Hence

$$
\boxed{d_{\rm exact}=1.}
$$

The word “every” matters: some special higher-degree bivariate polynomials have cancelling second moments and can be reproduced. The conclusion concerns the entire polynomial space, which already fails at degree two.

<h3 id="5/v">v</h3>

↑ **Parent:** [5](#5)

<h4 id="5/v/solution">Solution</h4>

↑ **Parent:** [V](#5/v)

Let the three grid-edge vectors be $v_1=a$, $v_2=b$, $v_3=b-a$, and define the constant-coefficient differential operator $D=\sum_{r=1}^3(v_r\cdot\nabla)^2$. For a stencil at grid spacing $h$, its displacement vectors $\delta$ about the new vertex have vanishing first and third moments by central symmetry. All four stencil types have the same second moment

$$
\sum_{\delta}\omega_\delta\,\delta\delta^T=\frac{h^2}{8}\sum_{r=1}^3v_rv_r^T.
$$

For the old-vertex stencil, each pair $\pm hv_r$ contributes $h^2v_rv_r^T/8$. For an edge parallel to $a$, the endpoint displacements are $\pm ha/2$ with weights $3/8$, and the opposite displacements are $\pm h(b-a/2)$ with weights $1/8$. Their moment is $h^2[aa^T/4+bb^T/4-(ab^T+ba^T)/8]$, precisely the same expression; the other edge orientations follow by symmetry.

If $f$ is a [multivariate polynomial](../../../polynomial.md#multivariate-polynomial) of total degree at most three, its [Taylor expansion](../../../calculus.md#taylor-expansion) is exact through the third-order term. Thus every refined vertex samples the single polynomial

$$
T_h f=f+\frac{h^2}{16}Df.
$$

The [polynomial](../../../polynomial.md) $Df$ has degree at most one, so subsequent refinement reproduces it exactly. Starting at unit spacing and successively halving $h$, the limit therefore is

$$
\boxed{f_\infty=f+\frac1{16}\sum_{\ell=0}^\infty4^{-\ell}Df=f+\frac1{12}Df.}
$$

The correction lowers degree by two, leaving the leading homogeneous term unchanged. Hence every sampled polynomial of degree at most three generates a polynomial of that same degree, even though quadratics and cubics need not be reproduced identically. For the extruded cases this gives $y^2\mapsto y^2+1/3$ and $y^3\mapsto y^3+y$.

Degree four is not guaranteed. Extruded data $g_j=j^4$ reduce to the [Cardinal cubic B-spline](../../../uniform-approximation.md#cardinal-cubic-b-spline) $G(y)=\sum_jj^4M_3(y-j)$, which is piecewise cubic and hence cannot be a single polynomial of degree four. It is not a lower-degree polynomial either: at integer rows, $G(k)=[(k-1)^4+4k^4+(k+1)^4]/6=k^4+2k^2+1/3$, which cannot agree with a cubic at all integers. This counterexample excludes every guaranteed degree $d\ge4$. Consequently

$$
\boxed{d_{\rm same\ degree}=3.}
$$

This distinguishes polynomial generation from exact reproduction and again refers to all polynomials through the stated degree.

## 6

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Use the limit [subdivision surface](../../../numerical-analysis.md#subdivision-surface) and limit [subdivision curve](../../../numerical-analysis.md#subdivision-curve), rather than treating their initial control meshes as the reflecting geometry. Build adaptive refinement hierarchies for both. Each surface cell supplies a limit-position evaluator, local [tangent vectors](../../../differential-geometry.md#tangent-vector) and a [normal vector](../../../differential-geometry.md#normal-vector); each curve interval supplies a limit-position evaluator and tangent. Regular regions may be evaluated as local [splines](../../../uniform-approximation.md#spline-mathematics), while extraordinary neighborhoods require the evaluation machinery of the specified subdivision rules. A piecewise smooth surface is handled patch by patch, with explicit boundary or crease joins.

A useful initial polygonal construction refines the surface to small [triangles](../../../geometry-and-topology.md#triangle) and the source curve to small [line segments](../../../mathematical-optimization.md#line-segment). For a candidate mirror [triangle](../../../geometry-and-topology.md#triangle) in a plane $n\cdot(X-X_0)=0$, reflect the eye across that plane:

$$
E^*=E-2\big(n\cdot(E-X_0)\big)n.
$$

For a source edge $Y(t)=(1-t)Y_0+tY_1$, a physical reflection point is the plane intersection of the line $E^*Y(t)$:

$$
X(t)=E^*+\lambda(t)(Y(t)-E^*),\qquad \lambda(t)=\frac{n\cdot(X_0-E^*)}{n\cdot(Y(t)-E^*)}.
$$

Keep only $0\le t\le1$, $0<\lambda<1$, points inside the mirror [triangle](../../../geometry-and-topology.md#triangle), and eye/source points on the appropriate reflecting side. Unfolding the reflected path across the mirror proves the [specular reflection](../../../optics.md#specular-reflection) condition. As $Y$ moves along a straight edge, $X$ lies on the intersection of the mirror plane with the plane through $E^*,Y_0,Y_1$, so the retained locus is a straight segment, a point or the empty set. Plane and triangle clipping computes its endpoints. If these defining points are collinear, or a denominator vanishes, use the corresponding limiting geometric case rather than a generic plane formula. A [bounding volume hierarchy](../../../numerical-analysis.md#bounding-volume-hierarchy) accelerates candidate search where geometric bounds exclude pairs; refined facet segments provide seeds and approximate connectivity.

To obtain the reflection curve of the actual limits, correct these seeds. In a local surface chart write $S(u,v)$, and on a source interval write $C(t)$. Set

$$
a=\frac{C(t)-S(u,v)}{\lVert C(t)-S(u,v)\rVert},\qquad b=\frac{E-S(u,v)}{\lVert E-S(u,v)\rVert},\qquad F=\begin{pmatrix}(a+b)\cdot S_u\\(a+b)\cdot S_v\end{pmatrix}.
$$

The exact limit reflection locus is $F=0$ together with the front-side conditions. For a two-sided mirror, orient $n$ locally so that $b\cdot n>0$ and require $a\cdot n>0$; for a one-sided mirror use its prescribed orientation and discard the wrong side. At grazing incidence this orientation condition ceases to be strict and the case needs separate handling. Unlike the eye-facing assumption in the parametric question, no global orientation condition is supplied here.

Apply a [continuation method](../../../numerical-analysis.md#continuation-method): at a rank-two root of $DF$, predict in a nullspace tangent direction and correct by the [Newton method](../../../mathematical-optimization.md#newton-s-method-in-optimization) on a transverse section. Map corrected parameters to $S(u,v)$, crossing patch and curve-interval boundaries through their hierarchy adjacency. Trace all branches, recognizing closed components and endpoints. Supplement facet seeds by recursive searches of the surface-cell/source-interval product, with [interval arithmetic](../../../numerical-analysis.md#interval-arithmetic) or other certified enclosures of $F$; otherwise a small loop absent from the initial polygonal approximation could be missed. Split singular neighborhoods where the [Jacobian matrix](../../../calculus.md#jacobian-matrix) loses rank, and test the open source-to-mirror and mirror-to-eye segments for occlusion when selecting actually visible components.

Allocate a geometric error budget to limit evaluation, root correction and polygonal chords. For example, require combined position-evaluation and corrected-root error at most $\epsilon/2$ and, on every regular arc, require the [chord error bound](../../../numerical-analysis.md#chord-error-bound) $M(\Delta s)^2/8\le\epsilon/2$. Use subdivision position and normal bounds for evaluations: a tiny position error alone is insufficient, since a wrong [normal vector](../../../differential-geometry.md#normal-vector) changes the reflected ray. Away from singularities an inverse transverse [Jacobian matrix](../../../calculus.md#jacobian-matrix) bound converts reflection residual into parameter error and a bound on $DS$ converts this to space error. Refine until these bounds hold, or use validated enclosures of entire arcs and their distances to the chords.

Near a caustic the inverse bound can become large, so the hierarchy must refine more strongly or isolate the singular branch geometry. Mesh flatness alone does not certify a reflection tolerance. With regular convergent evaluators and finite resolvable components, the resulting ordered vertices and chords satisfy

$$
\boxed{d_H\big(\text{visible limit reflection locus},\text{returned polygonal locus}\big)\le\epsilon.}
$$

The problem supplies no particular subdivision rules or smoothness guarantees, so this construction specifies what their evaluators and bounds must provide; an arbitrary nonsmooth or degenerate limit need not have an ordinary finite reflection curve. **Refine for seeds, enforce reflection on the actual limit geometry, then refine the traced arcs to the required spatial tolerance.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
