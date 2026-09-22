<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the limit [subdivision surface](../../../../../subdivision-surface.md) and limit [subdivision curve](../../../../../subdivision-curve.md), rather than treating their initial control meshes as the reflecting geometry. Build adaptive refinement hierarchies for both. Each surface cell supplies a limit-position evaluator, local [tangent vectors](../../../../../tangent-vector.md) and a [normal vector](../../../../../normal-vector.md); each curve interval supplies a limit-position evaluator and tangent. Regular regions may be evaluated as local [splines](../../../../../spline-mathematics.md), while extraordinary neighborhoods require the evaluation machinery of the specified subdivision rules. A piecewise smooth surface is handled patch by patch, with explicit boundary or crease joins.

A useful initial polygonal construction refines the surface to small [triangles](../../../../../triangle.md) and the source curve to small [line segments](../../../../../line-segment.md). For a candidate mirror [triangle](../../../../../triangle.md) in a plane $n\cdot(X-X_0)=0$, reflect the eye across that plane:

$$
E^*=E-2\big(n\cdot(E-X_0)\big)n.
$$

For a source edge $Y(t)=(1-t)Y_0+tY_1$, a physical reflection point is the plane intersection of the line $E^*Y(t)$:

$$
X(t)=E^*+\lambda(t)(Y(t)-E^*),\qquad \lambda(t)=\frac{n\cdot(X_0-E^*)}{n\cdot(Y(t)-E^*)}.
$$

Keep only $0\le t\le1$, $0<\lambda<1$, points inside the mirror [triangle](../../../../../triangle.md), and eye/source points on the appropriate reflecting side. Unfolding the reflected path across the mirror proves the [specular reflection](../../../../../specular-reflection.md) condition. As $Y$ moves along a straight edge, $X$ lies on the intersection of the mirror plane with the plane through $E^*,Y_0,Y_1$, so the retained locus is a straight segment, a point or the empty set. Plane and triangle clipping computes its endpoints. If these defining points are collinear, or a denominator vanishes, use the corresponding limiting geometric case rather than a generic plane formula. A [bounding volume hierarchy](../../../../../bounding-volume-hierarchy.md) accelerates candidate search where geometric bounds exclude pairs; refined facet segments provide seeds and approximate connectivity.

To obtain the reflection curve of the actual limits, correct these seeds. In a local surface chart write $S(u,v)$, and on a source interval write $C(t)$. Set

$$
a=\frac{C(t)-S(u,v)}{\lVert C(t)-S(u,v)\rVert},\qquad b=\frac{E-S(u,v)}{\lVert E-S(u,v)\rVert},\qquad F=\begin{pmatrix}(a+b)\cdot S_u\\(a+b)\cdot S_v\end{pmatrix}.
$$

The exact limit reflection locus is $F=0$ together with the front-side conditions. For a two-sided mirror, orient $n$ locally so that $b\cdot n>0$ and require $a\cdot n>0$; for a one-sided mirror use its prescribed orientation and discard the wrong side. At grazing incidence this orientation condition ceases to be strict and the case needs separate handling. Unlike the eye-facing assumption in the parametric question, no global orientation condition is supplied here.

Apply a [continuation method](../../../../../continuation-method.md): at a rank-two root of $DF$, predict in a nullspace tangent direction and correct by the [Newton method](../../../../../newton-s-method-in-optimization.md) on a transverse section. Map corrected parameters to $S(u,v)$, crossing patch and curve-interval boundaries through their hierarchy adjacency. Trace all branches, recognizing closed components and endpoints. Supplement facet seeds by recursive searches of the surface-cell/source-interval product, with [interval arithmetic](../../../../../interval-arithmetic.md) or other certified enclosures of $F$; otherwise a small loop absent from the initial polygonal approximation could be missed. Split singular neighborhoods where the [Jacobian matrix](../../../../../jacobian-matrix.md) loses rank, and test the open source-to-mirror and mirror-to-eye segments for occlusion when selecting actually visible components.

Allocate a geometric error budget to limit evaluation, root correction and polygonal chords. For example, require combined position-evaluation and corrected-root error at most $\epsilon/2$ and, on every regular arc, require the [chord error bound](../../../../../chord-error-bound.md) $M(\Delta s)^2/8\le\epsilon/2$. Use subdivision position and normal bounds for evaluations: a tiny position error alone is insufficient, since a wrong [normal vector](../../../../../normal-vector.md) changes the reflected ray. Away from singularities an inverse transverse [Jacobian matrix](../../../../../jacobian-matrix.md) bound converts reflection residual into parameter error and a bound on $DS$ converts this to space error. Refine until these bounds hold, or use validated enclosures of entire arcs and their distances to the chords.

Near a caustic the inverse bound can become large, so the hierarchy must refine more strongly or isolate the singular branch geometry. Mesh flatness alone does not certify a reflection tolerance. With regular convergent evaluators and finite resolvable components, the resulting ordered vertices and chords satisfy

$$
\boxed{d_H\big(\text{visible limit reflection locus},\text{returned polygonal locus}\big)\le\epsilon.}
$$

The problem supplies no particular subdivision rules or smoothness guarantees, so this construction specifies what their evaluators and bounds must provide; an arbitrary nonsmooth or degenerate limit need not have an ordinary finite reflection curve. **Refine for seeds, enforce reflection on the actual limit geometry, then refine the traced arcs to the required spatial tolerance.**

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
