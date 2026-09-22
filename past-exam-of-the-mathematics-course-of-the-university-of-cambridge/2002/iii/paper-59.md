# Paper 59

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper59.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper59.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Fix an explicit stationary-grid convention. For [subdivision arity](../../../numerical-analysis.md#subdivision-arity) $m>1$, write the univariate rule as

$$
p_i^{\ell+1}=\sum_jS_{ij}p_j^\ell,\qquad S_{ij}=a_{i-mj}.
$$

A column of the [subdivision matrix](../../../numerical-analysis.md#subdivision-matrix) is one translated [subdivision mask](../../../numerical-analysis.md#subdivision-mask); the next column is translated by $m$ fine-grid rows. Thus **the column displacement is the arity**. If $a_k$ is active from $k=\alpha$ to $k=\beta$, the [subdivision mask width](../../../numerical-analysis.md#subdivision-mask-width) is $w=\beta-\alpha+1$ fine-grid positions, after removing zero padding. Equivalently the mask span is $\beta-\alpha$ fine intervals. This is different from counting old [control points](../../../numerical-analysis.md#control-point) in a row stencil: that count measures how many controls influence one newly created point. Stating the convention avoids confusing these two widths.

For a convergent [subdivision curve](../../../numerical-analysis.md#subdivision-curve) scheme, its support is the influence region of one original [control point](../../../numerical-analysis.md#control-point), equivalently the [support of a function](../../../function.md#support) of the basic limit $\phi$ obtained from data $p_j=\delta_{j0}$. Translation gives the representation $P(t)=\sum_jp_j\phi(t-j)$. Descendant indices of index zero have parameter positions

$$
\frac{k_1}{m}+\frac{k_2}{m^2}+\cdots+\frac{k_\ell}{m^\ell},\qquad k_r\in[\alpha,\beta].
$$

Thus the limiting support enclosure is $[\alpha/(m-1),\beta/(m-1)]$, as in the [support of a stationary subdivision scheme](../../../numerical-analysis.md#support-of-a-stationary-subdivision-scheme). Endpoint activity gives equality for the ordinary positive convergent masks under discussion.

The [functional precision set of a subdivision scheme](../../../numerical-analysis.md#functional-precision-set-of-a-subdivision-scheme) consists of functions exactly recovered from their uniformly sampled data using the scheme's consistent parameter placement. Polynomial precision records the exactly reproduced [polynomial](../../../polynomial.md) space. Sampling-grid spacing and origin must be specified; the usual arbitrary-grid precision requirement uses every spacing and shift, rather than merely membership in the fixed-grid reconstruction space.

Center the given mask at indices $-1,0,1$. Its [binary linear interpolatory subdivision](../../../numerical-analysis.md#binary-linear-interpolatory-subdivision) rule is

$$
p'_{2j}=p_j,\qquad p'_{2j+1}=\tfrac12(p_j+p_{j+1}).
$$

Each new [control point](../../../numerical-analysis.md#control-point) is either an old point or an edge midpoint. Hence every refined [control polygon](../../../numerical-analysis.md#control-polygon) is the same [curve](../../../topology.md#curve) with extra vertices. Starting from scalar impulse data, the limit is explicitly

$$
\phi(t)=\max(1-|t|,0),\qquad\boxed{\operatorname{supp}\phi=[-1,1].}
$$

The mask width is three positions, its mask span is two, its largest row stencil uses two old [control points](../../../numerical-analysis.md#control-point), and its [subdivision arity](../../../numerical-analysis.md#subdivision-arity) is two. Translating the mask indexing to $0,1,2$ translates the basic support to $[0,2]$; the support width remains two original grid intervals.

On $[j,j+1]$, reconstruction is $(j+1-t)p_j+(t-j)p_{j+1}$. Constant and affine samples are therefore recovered exactly. A non-affine [polynomial](../../../polynomial.md) cannot agree with a linear expression on a whole open interval. Thus its polynomial [functional precision set of a subdivision scheme](../../../numerical-analysis.md#functional-precision-set-of-a-subdivision-scheme) is

$$
\boxed{\mathcal P=\operatorname{span}\{1,t\}.}
$$

For continuous functions reproduced at every translated sampling grid, the same conclusion holds: agreement with all chord interpolants forces the affine interpolation identity, hence affinity. At one fixed grid, the larger exactly representable class is the space of [linear splines](../../../uniform-approximation.md#linear-spline) with those [spline knots](../../../uniform-approximation.md#spline-knot); this is not a higher polynomial precision claim.

For arbitrary data, the one-sided [derivatives](../../../calculus.md#derivative) at $j$ are $p_j-p_{j-1}$ and $p_{j+1}-p_j$. They need not coincide. Therefore **the generic limit is $C^0$, not $C^1$**. Its first [derivative](../../../calculus.md#derivative) is piecewise constant; exceptional affine data, or individual matching neighboring slopes, can be smoother. This conclusion follows directly from the limit formula, not just from a heuristic mask-width test.

## 2

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

An efficient [parametric curve interrogation](../../../topology.md#parametric-curve-interrogation) interface should provide the parameter domain and open/closed status, point evaluation, one-sided endpoint enquiries, first and second [derivatives](../../../calculus.md#derivative) wherever defined, and information about knots or singular parameters. It should also restrict a curve to an interval and subdivide it without changing its limit, return a certified [bounding volume](../../../numerical-analysis.md#bounding-volume) for that restriction, and supply derivative or [chord error bounds](../../../numerical-analysis.md#chord-error-bound) when supported. These enquiries allow cheap geometric rejection before expensive exact evaluation. For a [subdivision curve](../../../numerical-analysis.md#subdivision-curve), limit evaluation is distinct from returning a vertex of a finite refined [control polygon](../../../numerical-analysis.md#control-polygon); the latter is usually an approximation.

For a query point $Q$, minimize $d(t)=\tfrac12\|P(t)-Q\|^2$. At a differentiable interior minimizer,

$$
\boxed{(P(t)-Q)\cdot P'(t)=0.}
$$

At a regular curve point this says that the query displacement is perpendicular to the [tangent vector](../../../differential-geometry.md#tangent-vector). If a second [derivative](../../../calculus.md#derivative) exists, the local second-order test is

$$
d''(t)=\|P'(t)\|^2+(P(t)-Q)\cdot P''(t)\ge0;
$$

a strictly positive value is sufficient for a strict local minimum. The stationarity equation alone also includes local maxima and is automatic at $P'=0$, so it cannot be used as the only global search criterion.

A reliable efficient [closest-point search on a subdivision curve](../../../numerical-analysis.md#closest-point-search-on-a-subdivision-curve) uses [branch and bound](../../../mathematical-optimization.md#branch-and-bound). Cover the compact curve by restricted pieces with certified enclosures $B_I$. For each piece set $L_I=\operatorname{dist}(Q,B_I)$, a lower bound on its true distance. Distances to actually evaluated limit points give upper bounds; keep the best point $P(t_*)$ and distance $U$. For an [axis-aligned bounding box](../../../numerical-analysis.md#axis-aligned-bounding-box) $\prod_k[l_k,h_k]$, the squared lower bound is inexpensive:

$$
L_I^2=\sum_k\bigl(\max\{l_k-Q_k,0,Q_k-h_k\}\bigr)^2.
$$

For positive partition-of-unity refinement, a [convex hull](../../../mathematical-optimization.md#convex-hull) of the active [control points](../../../numerical-analysis.md#control-point) is an enclosure. A negative-weight scheme requires a separate certified enclosure; its control hull need not contain the limit.

The algorithm is:

- Initialize the pieces at representation breaks and evaluate endpoints and one or more interior limit points. Place pieces in a priority queue ordered by their $L_I$.
- Discard any piece with $L_I>U$, since it cannot improve the best known point. If only one nearest point is required, equality may also be discarded; keep equality candidates when all ties matter.
- Remove the smallest-bound piece. Evaluate new limit points to reduce $U$, subdivide the piece, compute tighter child enclosures, and insert children that can still improve $U$.
- Use the best chord projection or current candidate to seed a safeguarded [Newton root-finding iteration](../../../numerical-analysis.md#newton-root-finding-iteration) for $F(t)=(P(t)-Q)\cdot P'(t)$. Its derivative is $F'(t)=\|P'\|^2+(P-Q)\cdot P''$. Keep iterates inside the restricted interval, fall back to [bisection method](../../../numerical-analysis.md#bisection-method) on an isolated sign-changing bracket, and accept an improvement only after evaluating its actual curve distance. This is an accelerator; rejection still depends on certified geometric bounds.
- Terminate when $U-\min_I L_I\le\epsilon$, also regarding the best evaluated point as a retained candidate. If no pieces remain, the evaluated candidate is already optimal relative to the exhausted bounds. Return $t_*$ and $P(t_*)$ with the global distance guarantee.

Because $\min_I L_I\le d_{\min}\le U$, the reported point is at most $\epsilon$ farther from $Q$ than a true nearest point. Include endpoints, nondifferentiable joins, and singular parameters in the candidate bookkeeping, or split them into separate pieces. With enclosures converging in diameter under subdivision on a compact continuous curve, the bounds converge to arbitrary prescribed positive distance tolerance. Interval bounds or outward-rounded arithmetic are needed if the guarantee is intended to be certified in floating-point computation. A single [Newton root-finding iteration](../../../numerical-analysis.md#newton-root-finding-iteration) from a single seed supplies no such global guarantee.

## 3

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [solid body transform](../../../geometry-and-topology.md#rigid-transformation) is a [rigid transformation](../../../geometry-and-topology.md#rigid-transformation): it preserves distances within the object. In three-dimensional coordinates it has the form $T(x)=Rx+b$, with translation $b\in\mathbb R^3$ and an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) $R$. For a proper physical rotation, the coefficient constraints are

$$
\boxed{R^TR=I,\qquad\det R=1.}
$$

Equivalently the columns of $R$ are an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) with positive orientation. A reflection also preserves distance but has $\det R=-1$ and is excluded when “solid-body motion” means a rotation and translation. There are three rotational and three translational degrees of freedom, not twelve independent matrix coefficients.

Computationally use the [homogeneous coordinates](../../../projective-space.md#homogeneous-coordinate) representation

$$
\begin{pmatrix}T(x)\\1\end{pmatrix}
=\begin{pmatrix}R&b\\0&1\end{pmatrix}\begin{pmatrix}x\\1\end{pmatrix}.
$$

The last row is $(0,0,0,1)$; matrix multiplication composes transforms. Alternatively store a unit [quaternion](../../../algebra.md#quaternion) together with $b$, maintaining its unit norm. A transpose gives the rotational inverse: $T^{-1}(y)=R^T(y-b)$.

Write the cubic [Bézier curve](../../../numerical-analysis.md#bezier-curve) as $P(t)=\sum_{i=0}^3B_i^3(t)p_i$, where $B_i^3(t)=\binom3i(1-t)^{3-i}t^i$. The [binomial theorem](../../../combinatorics.md#binomial-theorem) gives $\sum_iB_i^3(t)=1$. Transforming the controls produces

$$
\begin{aligned}
\widetilde P(t)&=\sum_{i=0}^3B_i^3(t)(Rp_i+b)\\
&=R\sum_{i=0}^3B_i^3(t)p_i+b\sum_{i=0}^3B_i^3(t)\\
&=\boxed{RP(t)+b=T(P(t)).}
\end{aligned}
$$

This proves pointwise equivariance, including the original parameter values; it is stronger than a statement that the two curves merely have the same shape.

Orthogonality was not used in the calculation. The identical proof applies to **every [affine map](../../../geometry-and-topology.md#affine-map) $T(x)=Ax+b$**, including scales, shears and even singular affine maps. It applies to every representation $P(u)=\sum_i\phi_i(u)p_i$ with scalar, control-independent [partition of unity](../../../differential-geometry.md#partition-of-unity) basis functions: [Bézier curves](../../../numerical-analysis.md#bezier-curve) of every degree, [B-splines](../../../uniform-approximation.md#b-spline), surfaces built on a [tensor-product surface basis](../../../differential-geometry.md#tensor-product-surface-basis), [triangular Bézier patches](../../../differential-geometry.md#triangular-bezier-patch), and more general linear control-point representations. Positivity is not needed for [affine equivariance of a geometric basis](../../../numerical-analysis.md#affine-equivariance-of-a-geometric-basis). For linear stationary [subdivision matrices](../../../numerical-analysis.md#subdivision-matrix) with row sums one, each refinement step commutes with the affine transformation; taking a convergent limit proves the corresponding assertion for [subdivision curves](../../../numerical-analysis.md#subdivision-curve) and [subdivision surfaces](../../../numerical-analysis.md#subdivision-surface). Rules with geometry-dependent nonlinear weights require separate equivariance tests and are not covered automatically.

The affine class is the largest class that preserves every such Euclidean-control construction with unchanged basis weights, under the usual continuity assumption. In fact the degree-one case would force

$$
T((1-t)x+ty)=(1-t)T(x)+tT(y)
$$

for all $x,y$ and $0\le t\le1$. This segment identity, followed by continuity, forces $T$ to be affine. Nonlinear transforms such as perspective division generally fail it.

There is a further extension when the representation itself is enlarged: apply a [projective transformation](../../../projective-space.md#projective-linear-transformation) linearly to homogeneous controls $(w_ip_i,w_i)$, then dehomogenize the weighted sum. The transformed objects are rational [Bézier curves](../../../numerical-analysis.md#bezier-curve) or [non-uniform rational B-splines](../../../uniform-approximation.md#non-uniform-rational-b-spline), with transformed weights as well as transformed Euclidean controls. This works wherever the new denominator is nonzero. It does not assert projective invariance of ordinary polynomial [Bézier curves](../../../numerical-analysis.md#bezier-curve) with their old weights.

## 4

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

[Lateral artifacts of a subdivision surface](../../../numerical-analysis.md#lateral-artifacts-of-a-subdivision-surface) are spurious changes along an intended straight extrusion. For example, if every row of a [control net](../../../numerical-analysis.md#control-net) is the same profile translated along a straight direction, a refinement rule should not create periodic ripples along that direction. This is distinct from changing or smoothing the transverse profile itself.

Use triangular-lattice coordinates $(i,j)$ with basis vectors $e_1=(1,0)$ and $e_2=(1/2,\sqrt3/2)$. The displayed mask is supported on $|i|,|j|,|i+j|\le3$, with the central entry at $(0,0)$. Write its coefficients as $a_{i,j}$, including their division by12. For data constant along horizontal rows, $p_{i,j}=q_j$, ternary refinement gives

$$
p'_{I,J}=\sum_kq_k\sum_{i\equiv I\ (\mathrm{mod}\ 3)}a_{i,J-3k}.
$$

Thus the three residue sums in every mask row must agree if arbitrary row-constant data are to remain row-constant. Equal whole-stencil sums alone only reproduce constants and do not guarantee straight-extrusion preservation.

For the original row $j=1$, the numerator coefficients at $i=-3,-2,-1,0,1,2$ are $2,4,5,5,4,2$. Their three residue sums are $7,8,7$, which do not agree. For $j=2$ the sums are $5,5,4$. In particular input $q_j=\delta_{j0}$ yields heights $7/12,8/12,7/12$ along the refined row $J=1$. **The original mask has lateral artifacts**, since it introduces a three-phase ripple into a straight extrusion. The residue-sum criterion is also the usual symbol-factor test: the mask polynomial must contain the ternary averaging factor in the extrusion direction. The original does not. This connects the concrete calculation with the directional artifact analysis in [Deriving Box-Spline Subdivision Schemes](https://neildodgson.com/pubs/arrows.pdf), while the coefficients and correction here are computed directly from the exam PDF.

A symmetric correction with the same denominator and support is to **replace the six nearest-center coefficients5 by6, and the six second-ring corner coefficients3 by2**. Leave every other coefficient unchanged, including the central6. The added and subtracted weights balance. For a complete computational specification, the corrected numerator rows are

$$
\begin{array}{c|r|l}
j&\text{first }i&\text{coefficients at successive }i\\\hline
3&-3&(1,2,2,1)\\
2&-3&(2,2,4,2,2)\\
1&-3&(2,4,6,6,4,2)\\
0&-3&(1,2,6,6,6,2,1)\\
-1&-2&(2,4,6,6,4,2)\\
-2&-1&(2,2,4,2,2)\\
-3&0&(1,2,2,1).
\end{array}
$$

Every entry in this new table is divided by12. The corresponding horizontal residue sums, before division, are

$$
\begin{array}{c|ccc}
j& i\equiv0&i\equiv1&i\equiv2\\\hline
-3&2&2&2\\
-2&4&4&4\\
-1&8&8&8\\
0&8&8&8\\
1&8&8&8\\
2&4&4&4\\
3&2&2&2.
\end{array}
$$

Consequently the corrected rule has [extrusion invariance of a ternary triangular scheme](../../../numerical-analysis.md#extrusion-invariance-of-a-ternary-triangular-scheme). Sixfold symmetry gives the same residue-sum property in the other two lattice-edge directions. Every two-dimensional residue class still sums to12 before normalization, so each refinement stencil sums to one. The weights are nonnegative. Symmetry about the stencil's refined parameter location also reproduces affine coordinates: the class first moments vanish, so an initial straight geometric translation direction remains straight.

The associated univariate boundary [subdivision mask](../../../numerical-analysis.md#subdivision-mask) is the common sum in each transverse row, rather than the central row of the bivariate mask. Centering it at indices $-3,\ldots,3$ gives

$$
\boxed{b=\frac16[1,2,4,4,4,2,1].}
$$

Its ternary stencils can be written explicitly as

$$
\boxed{\begin{aligned}
q'_{3k}&=\tfrac16q_{k-1}+\tfrac23q_k+\tfrac16q_{k+1},\\
q'_{3k+1}&=\tfrac23q_k+\tfrac13q_{k+1},\\
q'_{3k+2}&=\tfrac13q_k+\tfrac23q_{k+1}.
\end{aligned}}
$$

Each stencil sums to one and has the correct affine parameter moment. Applying this rule to a boundary profile agrees with the bivariate rule on a straight extrusion. Endpoint or corner rules must still be chosen for a finite open boundary. The artifact-free conclusion established here concerns the three lattice-edge extrusion directions; it does not promise exact extrusion preservation for every arbitrary off-grid direction. The directional limitation is intrinsic to the mask test, not a reason to substitute the central mask row as a boundary rule.

## 5

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [tensor-product surface basis](../../../differential-geometry.md#tensor-product-surface-basis) is formed from two independent univariate basis families $\phi_i(u)$ and $\psi_j(v)$ on separate parameter intervals. Given a rectangular [control net](../../../numerical-analysis.md#control-net) $p_{ij}$, its [parametric surface](../../../differential-geometry.md#parametric-surface) is

$$
\boxed{S(u,v)=\sum_i\sum_jp_{ij}\phi_i(u)\psi_j(v).}
$$

The parameters and indices vary independently over a product domain. The representation can be evaluated first in either parameter, giving a convenient computational advantage. Assume a finite basis, or locally finite [spline](../../../uniform-approximation.md#spline-mathematics) bases, so differentiation and summation below are justified locally.

For positivity, if each factor basis is nonnegative, then $\phi_i(u)\psi_j(v)\ge0$. If both factors are strictly positive at a point, their product is strictly positive there. Nonnegative weights are the usual geometric meaning of positivity; zero boundary weights are allowed. With [partition of unity](../../../differential-geometry.md#partition-of-unity), this gives the local [convex hull](../../../mathematical-optimization.md#convex-hull) enclosure of the active [control points](../../../numerical-analysis.md#control-point).

For continuity, suppose the first family is $C^r$ and the second $C^s$, including matching derivatives across their respective [spline knots](../../../uniform-approximation.md#spline-knot). On every polynomial piece, and by matching at the knot lines,

$$
\partial_u^p\partial_v^qS(u,v)
=\sum_{i,j}p_{ij}\phi_i^{(p)}(u)\psi_j^{(q)}(v),
\qquad 0\le p\le r,\quad0\le q\le s.
$$

Every factor on the right is continuous in its own variable, so its product is jointly continuous. Thus **all these mixed derivatives are continuous**, in particular the surface is jointly $C^{\min(r,s)}$. The separate coordinate smoothness can be better: $r$ orders in $u$ and $s$ in $v$. For piecewise polynomials of degrees $d_u,d_v$, an interior knot of multiplicity $k$ in the first factor normally gives $C^{d_u-k}$ matching in $u$, inherited along that knot line; similarly for $v$. The statement is an inherited lower bound. Special [control points](../../../numerical-analysis.md#control-point) can cancel derivative jumps, so a particular surface may be smoother than a generic member of its basis.

For summation to unity, independent summation factors exactly:

$$
\boxed{\sum_{i,j}\phi_i(u)\psi_j(v)
=\left(\sum_i\phi_i(u)\right)\left(\sum_j\psi_j(v)\right)=1.}
$$

This also explains why translations of all [control points](../../../numerical-analysis.md#control-point) translate the surface by the same vector, as in [affine equivariance of a geometric basis](../../../numerical-analysis.md#affine-equivariance-of-a-geometric-basis). These three arguments establish [tensor-product inheritance of geometric basis properties](../../../differential-geometry.md#tensor-product-inheritance-of-geometric-basis-properties) directly from the factor identities.

A [triangular Bézier patch](../../../differential-geometry.md#triangular-bezier-patch) is a non-tensor-product example. For barycentric parameters $u,v,w\ge0$ with $u+v+w=1$, a quadratic patch is

$$
S=u^2p_{200}+v^2p_{020}+w^2p_{002}
+2uvp_{110}+2uwp_{101}+2vwp_{011}.
$$

The six basis functions have total degree two and sum to $(u+v+w)^2=1$. Their index constraint and triangular parameter domain do not arise from two independently indexed univariate factors on a rectangle. An individual triangular polynomial could be embedded in another larger representation, but this triangular basis and [control net](../../../numerical-analysis.md#control-net) are not a tensor-product surface definition.

## 6

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

An efficient [subdivision surface interrogation](../../../numerical-analysis.md#subdivision-surface-interrogation) interface needs the mesh topology and patch adjacency, boundary and trimming information, patch-local parameter charts and their transition maps, and local restriction/refinement with the complete influencing [control net](../../../numerical-analysis.md#control-net). Numerical enquiries should supply limit positions $S$, first [derivatives](../../../calculus.md#derivative) $S_u,S_v$, and second [derivatives](../../../calculus.md#derivative) where defined; these determine [normal vectors](../../../differential-geometry.md#normal-vector) and [curvatures](../../../differential-geometry.md#curvature) at regular points. It must also return certified patch [bounding volumes](../../../numerical-analysis.md#bounding-volume) and convergent geometric/derivative error bounds. Near an [extraordinary subdivision vertex](../../../numerical-analysis.md#extraordinary-subdivision-vertex), use the local [subdivision matrix](../../../numerical-analysis.md#subdivision-matrix) and limit/tangent evaluation appropriate to that scheme; second [derivatives](../../../calculus.md#derivative) need not exist merely because a tangent plane does. Finite refined mesh vertices are not exact limit positions.

Represent the cutting [plane](../../../geometry-and-topology.md#plane) as $n\cdot x=d$, with $n$ normalized. On each chart set

$$
g(u,v)=n\cdot S(u,v)-d,
\qquad g_u=n\cdot S_u,\quad g_v=n\cdot S_v.
$$

The desired [plane section of a subdivision surface](../../../numerical-analysis.md#plane-section-of-a-subdivision-surface) is the image of the zero set $g=0$. For a [bounding volume](../../../numerical-analysis.md#bounding-volume) $B$, compute a certified interval $[g_{\min},g_{\max}]$ for the plane functional over $B$. If that interval is strictly positive or strictly negative, reject the patch. With positive partition-of-unity weights, the minimum and maximum of $n\cdot p_i-d$ over all influencing [control points](../../../numerical-analysis.md#control-point) already bound its limit patch. For masks without this [convex hull](../../../mathematical-optimization.md#convex-hull) property, the interface must provide a different valid enclosure.

An adaptive algorithm that isolates components before tracing is:

- Build or reuse a [bounding volume hierarchy](../../../numerical-analysis.md#bounding-volume-hierarchy) over limit patches. Traverse only patches whose plane-functional interval contains zero; entirely rejected subtrees need no limit evaluation.
- Recursively restrict every retained patch. At regular spline patches, use their exact polynomial/rational basis to refine range and derivative bounds. Split at representation breaks, boundaries and extraordinary neighborhoods rather than differentiating across them blindly.
- In a sufficiently small transverse patch, certify that at least one of $g_u,g_v$ stays away from zero. Then the zero set is locally a graph by the [implicit function theorem](../../../calculus.md#implicit-function-theorem), with no interior closed component in that chart. Isolate all zeros on its patch edges, using certified scalar ranges, derivative bounds and safeguarded [Newton root-finding iteration](../../../numerical-analysis.md#newton-root-finding-iteration). Pair edge intersections according to the monotone graph structure, subdividing further if the connectivity is not certified. A certified transverse graph with no boundary zero can be rejected.
- For every isolated branch, trace a predictor-corrector [continuation method](../../../numerical-analysis.md#continuation-method). The parameter [tangent vector](../../../differential-geometry.md#tangent-vector) is $t=(-g_v,g_u)$. Normalize by $\|DS\,t\|$ when physical [arc length](../../../riemannian-geometry.md#arc-length) steps are desired, predict $z_p=z+h\,t$, then correct with the two scalar equations $g(z_c)=0$ and $t_p\cdot(z_c-z_p)=0$. The Newton correction solves the explicit $2\times2$ system with rows $(g_u,g_v)$ and $t_p^T$. Reduce the step if this system is ill-conditioned or the correction leaves its chart.
- Transfer branches consistently across patch edges and assemble the resulting segments into connected curves, including boundary endpoints and closed loops. Edge intersection records must be shared between neighboring patches to avoid cracks or duplicate branches.
- Keep unresolved patches containing possible tangent contacts, singular vertices, or coplanar pieces for a separate degeneracy treatment. Do not discard them solely because no sampled edge changes sign. Refine, use local polynomial/interval tests if available, or return an explicitly flagged unresolved contact region at the selected tolerance.

This is exhaustive to a chosen tolerance when certified subdivision isolates finitely many regular transverse branches and enclosures converge. If $\|\nabla g\|\ge\gamma>0$ locally and $\|DS\|\le M$, a residual tolerance $|g|\le\delta$ corresponds locally to a geometric correction bounded by $M\delta/\gamma$, using the gradient flow toward the level set. Bounds on second [derivatives](../../../calculus.md#derivative) similarly control curve-segment [chord error bound](../../../numerical-analysis.md#chord-error-bound). As $\gamma$ approaches zero, a fixed residual tolerance no longer gives a fixed geometric error, so the step and stopping rules must reflect conditioning.

Seeding must not rely just on corner signs. For example $S(u,v)=(u,v,u^2+v^2-r^2)$ cut by $z=0$ has a closed circle wholly inside a patch whose corner values are all positive. Certified range tests plus subdivision retain it; a corner-only marching rule can miss it. Tangencies also change the nature of the output: $S=(u,v,u^2+v^2)$ meets $z=0$ in one isolated point, while a coplanar patch contributes an area rather than a curve. Thus **a general plane section is not necessarily a union of regular curves**; the algorithm should classify these cases instead of silently fabricating or deleting a branch.

For efficiency, cache subdivision stencils, patch extraction, limit-evaluation coefficients and bounds; reuse child data instead of reconstructing the entire refined mesh. Use local influencing neighborhoods, with the halo dictated by mask support, and keep adjacency/boundary topology separate from changing geometric coordinates. Plane-functional bounds can be computed by refining scalar signed-distance controls, which is cheaper than refining all three coordinates. Combine coarse inexpensive boxes with tighter local [convex hull](../../../mathematical-optimization.md#convex-hull) or [interval arithmetic](../../../numerical-analysis.md#interval-arithmetic) tests only where needed. Adapt steps to curvature and transversality, reuse branch seeds, and use regular spline evaluation away from extraordinary points. Stable edge ownership, outward-rounded bounds, scale-aware tolerances, and explicit degeneracy flags are correctness requirements as well as performance issues. The result is a limit-surface intersection computation; merely intersecting a finitely refined [control polyhedron](../../../numerical-analysis.md#control-net) with the plane supplies only an uncontrolled approximation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
