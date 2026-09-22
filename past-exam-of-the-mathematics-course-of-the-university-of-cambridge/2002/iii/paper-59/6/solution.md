<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

An efficient [subdivision surface interrogation](../../../../../subdivision-surface-interrogation.md) interface needs the mesh topology and patch adjacency, boundary and trimming information, patch-local parameter charts and their transition maps, and local restriction/refinement with the complete influencing [control net](../../../../../control-net.md). Numerical enquiries should supply limit positions $S$, first [derivatives](../../../../../derivative.md) $S_u,S_v$, and second [derivatives](../../../../../derivative.md) where defined; these determine [normal vectors](../../../../../normal-vector.md) and [curvatures](../../../../../curvature.md) at regular points. It must also return certified patch [bounding volumes](../../../../../bounding-volume.md) and convergent geometric/derivative error bounds. Near an [extraordinary subdivision vertex](../../../../../extraordinary-subdivision-vertex.md), use the local [subdivision matrix](../../../../../subdivision-matrix.md) and limit/tangent evaluation appropriate to that scheme; second [derivatives](../../../../../derivative.md) need not exist merely because a tangent plane does. Finite refined mesh vertices are not exact limit positions.

Represent the cutting [plane](../../../../../plane.md) as $n\cdot x=d$, with $n$ normalized. On each chart set

$$
g(u,v)=n\cdot S(u,v)-d,
\qquad g_u=n\cdot S_u,\quad g_v=n\cdot S_v.
$$

The desired [plane section of a subdivision surface](../../../../../plane-section-of-a-subdivision-surface.md) is the image of the zero set $g=0$. For a [bounding volume](../../../../../bounding-volume.md) $B$, compute a certified interval $[g_{\min},g_{\max}]$ for the plane functional over $B$. If that interval is strictly positive or strictly negative, reject the patch. With positive partition-of-unity weights, the minimum and maximum of $n\cdot p_i-d$ over all influencing [control points](../../../../../control-point.md) already bound its limit patch. For masks without this [convex hull](../../../../../convex-hull.md) property, the interface must provide a different valid enclosure.

An adaptive algorithm that isolates components before tracing is:

- Build or reuse a [bounding volume hierarchy](../../../../../bounding-volume-hierarchy.md) over limit patches. Traverse only patches whose plane-functional interval contains zero; entirely rejected subtrees need no limit evaluation.
- Recursively restrict every retained patch. At regular spline patches, use their exact polynomial/rational basis to refine range and derivative bounds. Split at representation breaks, boundaries and extraordinary neighborhoods rather than differentiating across them blindly.
- In a sufficiently small transverse patch, certify that at least one of $g_u,g_v$ stays away from zero. Then the zero set is locally a graph by the [implicit function theorem](../../../../../implicit-function-theorem.md), with no interior closed component in that chart. Isolate all zeros on its patch edges, using certified scalar ranges, derivative bounds and safeguarded [Newton root-finding iteration](../../../../../newton-root-finding-iteration.md). Pair edge intersections according to the monotone graph structure, subdividing further if the connectivity is not certified. A certified transverse graph with no boundary zero can be rejected.
- For every isolated branch, trace a predictor-corrector [continuation method](../../../../../continuation-method.md). The parameter [tangent vector](../../../../../tangent-vector.md) is $t=(-g_v,g_u)$. Normalize by $\|DS\,t\|$ when physical [arc length](../../../../../arc-length.md) steps are desired, predict $z_p=z+h\,t$, then correct with the two scalar equations $g(z_c)=0$ and $t_p\cdot(z_c-z_p)=0$. The Newton correction solves the explicit $2\times2$ system with rows $(g_u,g_v)$ and $t_p^T$. Reduce the step if this system is ill-conditioned or the correction leaves its chart.
- Transfer branches consistently across patch edges and assemble the resulting segments into connected curves, including boundary endpoints and closed loops. Edge intersection records must be shared between neighboring patches to avoid cracks or duplicate branches.
- Keep unresolved patches containing possible tangent contacts, singular vertices, or coplanar pieces for a separate degeneracy treatment. Do not discard them solely because no sampled edge changes sign. Refine, use local polynomial/interval tests if available, or return an explicitly flagged unresolved contact region at the selected tolerance.

This is exhaustive to a chosen tolerance when certified subdivision isolates finitely many regular transverse branches and enclosures converge. If $\|\nabla g\|\ge\gamma>0$ locally and $\|DS\|\le M$, a residual tolerance $|g|\le\delta$ corresponds locally to a geometric correction bounded by $M\delta/\gamma$, using the gradient flow toward the level set. Bounds on second [derivatives](../../../../../derivative.md) similarly control curve-segment [chord error bound](../../../../../chord-error-bound.md). As $\gamma$ approaches zero, a fixed residual tolerance no longer gives a fixed geometric error, so the step and stopping rules must reflect conditioning.

Seeding must not rely just on corner signs. For example $S(u,v)=(u,v,u^2+v^2-r^2)$ cut by $z=0$ has a closed circle wholly inside a patch whose corner values are all positive. Certified range tests plus subdivision retain it; a corner-only marching rule can miss it. Tangencies also change the nature of the output: $S=(u,v,u^2+v^2)$ meets $z=0$ in one isolated point, while a coplanar patch contributes an area rather than a curve. Thus **a general plane section is not necessarily a union of regular curves**; the algorithm should classify these cases instead of silently fabricating or deleting a branch.

For efficiency, cache subdivision stencils, patch extraction, limit-evaluation coefficients and bounds; reuse child data instead of reconstructing the entire refined mesh. Use local influencing neighborhoods, with the halo dictated by mask support, and keep adjacency/boundary topology separate from changing geometric coordinates. Plane-functional bounds can be computed by refining scalar signed-distance controls, which is cheaper than refining all three coordinates. Combine coarse inexpensive boxes with tighter local [convex hull](../../../../../convex-hull.md) or [interval arithmetic](../../../../../interval-arithmetic.md) tests only where needed. Adapt steps to curvature and transversality, reuse branch seeds, and use regular spline evaluation away from extraordinary points. Stable edge ownership, outward-rounded bounds, scale-aware tolerances, and explicit degeneracy flags are correctness requirements as well as performance issues. The result is a limit-surface intersection computation; merely intersecting a finitely refined [control polyhedron](../../../../../control-net.md) with the plane supplies only an uncontrolled approximation.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
