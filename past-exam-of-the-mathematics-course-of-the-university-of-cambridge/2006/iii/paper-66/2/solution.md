<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work first in the parameter rectangle of the [parametric surface](../../../../../parametric-surface.md). Set $g(u,v)=f(F(u,v))$. With $F_u,F_v$ linearly independent, the chain rule gives

$$
g_u=\nabla f(F)\cdot F_u,\qquad g_v=\nabla f(F)\cdot F_v.
$$

The intersection is transversal precisely when the implicit [normal vector](../../../../../normal-vector.md) $\nabla f(F)$ and the parametric [normal vector](../../../../../normal-vector.md) $F_u\times F_v$ are not parallel. Consequently $(g_u,g_v)\ne(0,0)$, and the [implicit function theorem](../../../../../implicit-function-theorem.md) makes $g=0$ a locally regular parameter curve. This is the setting for [transversal surface intersection tracing](../../../../../transversal-surface-intersection-tracing.md) by a predictor-corrector [continuation method](../../../../../continuation-method.md).

Find one seed on the required component. Subdivide parameter patches, enclosing their images by [bounding volumes](../../../../../bounding-volume.md) and testing whether a certified range of $f$ excludes zero. For a positive-weight [NURBS](../../../../../non-uniform-rational-b-spline.md), the active control-point [convex hull](../../../../../convex-hull.md) supplies a convenient enclosure; [interval arithmetic](../../../../../interval-arithmetic.md) can tighten the range of the composed function. Search the surviving patches for a bracketed root or a local corrected seed. Merely checking signs at four corners is inadequate: a small closed intersection can lie wholly inside a patch with the same corner signs. An adaptive or certified patch search, or a supplied seed, avoids this failure. For a [sphere](../../../../../sphere.md) centered at $C$, use $f(P)=\|P-C\|^2-r^2$ and $\nabla f=2(P-C)$; for a [torus](../../../../../torus.md), use its implicit polynomial and its differentiated polynomial in the same algorithm.

At a corrected seed $\eta_k=(u_k,v_k)$, an unnormalized parameter [tangent vector](../../../../../tangent-vector.md) and a unit spatial [tangent vector](../../../../../tangent-vector.md) are

$$
q_0=(-g_v,g_u),\qquad T_k={F_u(q_0)_1+F_v(q_0)_2\over\|F_u(q_0)_1+F_v(q_0)_2\|}.
$$

Choose the sign consistently with the previous [tangent vector](../../../../../tangent-vector.md). Normalize $q=q_0/\|DFq_0\|$ and predict $\eta_p=\eta_k+hq$, so $h$ is approximately a physical [arc length](../../../../../arc-length.md) step. Correct the predictor by [Newton method](../../../../../newton-s-method-in-optimization.md) applied to

$$
g(\eta)=0,\qquad T_k\cdot(F(\eta)-F(\eta_k))-h=0.
$$

The Jacobian has rows $(g_u,g_v)$ and $(T_k\cdot F_u,T_k\cdot F_v)$. At the starting point its first row vanishes along $q$, whereas its second row applied to $q$ is one. The two rows are therefore independent. The transverse-plane condition prevents the corrector from sliding arbitrarily along the intersection. Restrict correction to a neighborhood of the predictor, use damping, and reduce $h$ when correction fails or its displacement becomes excessive; this prevents jumps to another nearby branch.

To obtain a sufficiently dense sequence, impose a physical point-spacing bound, a bound on tangent turning, and a chord-error estimate. For local [curvature](../../../../../curvature.md) $\kappa$, the small-step sagitta is approximately $\kappa h^2/8$; estimate curvature from successive [tangent vectors](../../../../../tangent-vector.md) and reduce $h$ until this and the desired spacing are acceptable. The correction residual should be small relative to the drawing tolerance. Uniform steps in $u$ or $v$ alone do not ensure spatial density because the surface metric can vary considerably.

For an open component, trace in both tangent directions from the seed. On reaching a parameter boundary, locate the endpoint by solving $g=0$ together with that boundary's parameter equation, rather than accepting an overshoot. For a closed component, stop only after nontrivial travel and return to the initial parameter location with compatible tangent orientation; near-coincidence in three-dimensional space alone can mistake a self-intersection or neighboring branch for closure. Cross periodic seams using the appropriate chart identification. **Adaptive physical stepping, local correction, and component-aware termination give the required point sequence.** A vanishing parameter gradient signals a tangency or singularity outside the transversal hypothesis and must be reported rather than passed through by this regular algorithm.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
