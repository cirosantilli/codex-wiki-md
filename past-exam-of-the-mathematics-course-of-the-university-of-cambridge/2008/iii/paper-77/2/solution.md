<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

At $X=P(u,v)$, orient the unit [normal vector](../../../../../normal-vector.md) $n=(P_u\times P_v)/\lVert P_u\times P_v\rVert$ towards the eye. Define the unit directions from the reflecting point to the source and eye by

$$
a=\frac{Q(t)-P(u,v)}{\lVert Q(t)-P(u,v)\rVert},\qquad b=\frac{E-P(u,v)}{\lVert E-P(u,v)\rVert}.
$$

The incident propagation direction is $-a$. The law of [specular reflection](../../../../../specular-reflection.md) is $b=-a+2(a\cdot n)n$, so $a+b$ is normal to the surface. Conversely, if the tangential components of $a+b$ vanish and $a\cdot n,b\cdot n>0$, its unit-length summands have equal positive normal components and obey the reflection law. Therefore solve the two scalar equations

$$
\boxed{F(u,v,t)=\begin{pmatrix}(a+b)\cdot P_u\\(a+b)\cdot P_v\end{pmatrix}=0,\qquad (u,v,t)\in[0,1]^3,\quad a\cdot n>0.}
$$

The stated orientation condition gives $b\cdot n>0$. It removes the back-facing ambiguity, but not multiple images or caustics. Exclude $Q(t)=P(u,v)$ and $E=P(u,v)$, where these directions are undefined.

At a root where the $2\times3$ [Jacobian matrix](../../../../../jacobian-matrix.md) $DF$ has rank two, the [implicit function theorem](../../../../../implicit-function-theorem.md) makes the solution set a local curve in parameter space. Compute a unit tangent $w$ in its nullspace; equivalently take the normalized [cross product](../../../../../cross-product.md) of the two rows of $DF$. A [continuation method](../../../../../continuation-method.md) predicts $x_p=x+h w$, where $x=(u,v,t)$, then corrects with the [Newton method](../../../../../newton-s-method-in-optimization.md) applied to the three equations

$$
F(x_{\rm new})=0,\qquad w\cdot(x_{\rm new}-x_p)=0.
$$

The last equation fixes a transverse section and allows tracing through a turning point of $t$, where solving only for $(u,v)$ at successive fixed source parameters would fail. The corresponding space point is $R=P(u,v)$, with derivative $R'=P_u u'+P_v v'$ along the traced parameter-space curve.

Find initial roots by subdividing the parameter cube, using [interval arithmetic](../../../../../interval-arithmetic.md) bounds on $F$ to discard impossible boxes and validated local solves in the remaining boxes. Trace in both directions, stop at the boundary or a recognized closed loop, and retain a record of traced boxes to avoid duplicates. Search the remaining boxes as well: starting from just one seed would miss disconnected closed reflection curves. Where $DF$ loses rank, reduce the step and subdivide locally to find the outgoing branches instead of continuing a single guessed tangent. If physical visibility is required, discard roots for which either open segment $XE$ or $XQ(t)$ is occluded; test these segments against the surface or any supplied scene geometry.

Control the geometric approximation rather than just the parameter step. For any regular traced arc $R(s)$ with a bound $\lVert R''(s)\rVert\le M$, the [chord error bound](../../../../../chord-error-bound.md) gives an arc-to-chord [Hausdorff distance](../../../../../hausdorff-distance.md) at most $M(\Delta s)^2/8$. Budget, for example, half of $\epsilon$ for corrected-vertex error and half for chord error; accept a segment only when

$$
\boxed{\delta_{\rm vertex}\le\epsilon/2,\qquad M(\Delta s)^2/8\le\epsilon/2.}
$$

Bound the vertex error through the inverse transverse [Jacobian matrix](../../../../../jacobian-matrix.md) and a bound on $DP$, or use validated root enclosures. If analytic second-derivative bounds are unavailable, recursively subdivide and enclose each arc in a geometric tube of radius at most the remaining tolerance around its chord. A midpoint test alone is a useful heuristic but cannot certify the requested error for an arbitrary oscillatory curve.

The returned vertices $P(u_k,v_k)$ and their ordered connecting segments give the reflection curve to the prescribed tolerance on every resolved branch. Finite certified termination requires regular evaluable patches, derivative or enclosure bounds, and finitely resolvable branches; eye-facing normals alone do not guarantee these properties. Singular components or an identically vanishing reflection constraint must be handled as such rather than silently reported as an ordinary curve.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
