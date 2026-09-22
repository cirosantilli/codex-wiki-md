<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the PDF's notation: $P$ is the fixed point light, $C(t)$ is the casting curve, and $S(u,v)$ is the receiver. A shadow point solves

$$
F(u,v,\alpha;t):=S(u,v)-P-\alpha(C(t)-P)=0,\qquad\alpha>1.
$$

The separating-plane assumption puts the caster between light and receiver, so the relevant intersections are beyond the caster, not on the backward ray. The facing assumption supplies transverse regular intersections on the lit side. Carry out [shadow tracing for a parametric curve](../../../../../../shadow-tracing-for-a-parametric-curve.md) as follows.

First subdivide the curve domain and receiving patches. Reject combinations whose certified [bounding volumes](../../../../../../bounding-volume.md) cannot intersect the corresponding forward ray cone. For the remaining combinations, subdivide and isolate a hit, then correct its parameters using a three-variable [Newton method](../../../../../../newton-s-method-in-optimization.md) with Jacobian

$$
J=\big[S_u,\ S_v,\ -(C(t)-P)\big].
$$

Check that the corrected parameters lie in the patch domain and $\alpha>1$. Seed every connected component; one arbitrary initial hit does not establish that other components are absent. If a ray has several receiving hits, compare their $\alpha$ values and retain the visible first hit, rather than jumping between sheets.

At a transverse branch the Jacobian is nonsingular because $(C-P)\cdot(S_u\times S_v)\ne0$. Differentiate the equation to predict the next hit:

$$
J\begin{pmatrix}u'\\v'\\\alpha'\end{pmatrix}=\alpha C'(t).
$$

Use this predictor for a proposed parameter step, then apply Newton correction. To control the polygonal approximation, the shadow path is $X(t)=S(u(t),v(t))$. A second differentiation gives

$$
J\begin{pmatrix}u''\\v''\\\alpha''\end{pmatrix}=\alpha C''+2\alpha'C'-S_{uu}(u')^2-2S_{uv}u'v'-S_{vv}(v')^2.
$$

Together with the surface derivatives this supplies a bound on $X''$. If $\|X''\|\leq M$ over an interval of width $h$, the maximum error from its chord is at most $Mh^2/8$. Subdivide until this bound, plus the numerical intersection error, is below the graphics tolerance. Corrected endpoints then give the requested point sequence on $S$. If second-derivative bounds are unavailable, refine until a certified enclosure of the entire branch segment lies within tolerance of its chord; a sufficiently small enclosure diameter is a conservative fallback.

Continue through adjacent patches, split at a trim or surface boundary, and stop a component when its admissible intersection ceases. Record closed components without duplicating their starting point. **Use adaptive chord-error control and component isolation; a fixed fine sampling or an unverified sequence of local Newton solves can miss part of the shadow.** If only estimated midpoint errors are available, those support a practical rendering heuristic rather than a certified tolerance.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
