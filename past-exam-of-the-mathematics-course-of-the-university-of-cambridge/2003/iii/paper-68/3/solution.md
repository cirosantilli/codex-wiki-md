<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [parametric curve interrogation](../../../../../parametric-curve-interrogation.md) interface first supplies the parameter domain and the point $C(t)$. At regular parameters, it also supplies $C'(t)$ and, when needed, higher [derivatives](../../../../../derivative.md). The unit [tangent vector](../../../../../tangent-vector.md), speed and [curvature](../../../../../curvature.md) are then obtained from

$$
\frac{C'}{\|C'\|},\qquad \|C'\|,\qquad
\kappa=\frac{\|C'\times C''\|}{\|C'\|^3}
$$

in three dimensions. The formulas require $C'\ne0$; a Frenet normal additionally requires nonzero [curvature](../../../../../curvature.md). A practical interface can restrict the curve to a parameter interval, provide endpoints, and give a certified [bounding volume](../../../../../bounding-volume.md) or a derivative-range bound. Arc length, closest-point and intersection queries are higher-level operations built from these elementary enquiries rather than consequences of point evaluation alone.

For a plane $n\cdot x=d$ with $n\ne0$, define

$$
F(t)=n\cdot C(t)-d,\qquad F'(t)=n\cdot C'(t).
$$

This reduces [certified curve-plane intersection](../../../../../certified-curve-plane-intersection.md) to scalar root isolation. A [subdivision curve](../../../../../subdivision-curve.md) can expose the parametric enquiries by evaluating its limit at a parameter address: refine the corresponding piece until its certified positional enclosure reaches the requested accuracy, or use its exact local [spline](../../../../../spline-mathematics.md) representation. [Derivative](../../../../../derivative.md) evaluation similarly needs the [derivative](../../../../../derivative.md) refinement rule and its error bound. A finite control vertex is not automatically a point of the limit curve.

One reliable algorithm is **range-based isolation followed by safeguarded Newton iteration**:

- Split the domain at representation breaks. For each interval $I$, enclose $F(I)$ by projecting its certified curve bound onto $n$. Reject $I$ if this interval excludes zero.
- If the [derivative](../../../../../derivative.md) enclosure excludes zero and the endpoint values have opposite signs, there is exactly one intersection in $I$. Record any endpoint zero separately and avoid counting it twice.
- Within such a bracket, propose $t_{\rm new}=t-F(t)/F'(t)$ using the [Newton root-finding iteration](../../../../../newton-root-finding-iteration.md). Accept only a well-conditioned step inside a suitably smaller portion of the bracket; otherwise use the [bisection method](../../../../../bisection-method.md). Update the sign bracket and stop when its parameter width and the curve's positional error meet the tolerances.
- Subdivide every other undecided interval. Use representation-supported tests for tangent roots and coplanar pieces; do not reject an interval merely because its endpoint signs agree.

For a transverse root, the [derivative](../../../../../derivative.md) is nonzero nearby, so sufficiently fine intervals have monotone $F$ and the sign bracket isolates it. Bisection provides a global error bound; near a simple root Newton iteration gives quadratic convergence. Good enclosures discard most of the curve before expensive limit evaluation, and the method does not require a specific subdivision mask.

The weaknesses are equally important. Near tangency $F'$ is small and Newton steps are ill-conditioned; same-sign endpoints may conceal a tangent root or two crossings. An arc lying in the plane has infinitely many intersections and should be returned as an interval, not a point. Finite-precision evaluations require error enclosures before a sign is certified. For an arbitrary smooth point-evaluation oracle, **no finite sampling scheme can certify all intersections**: a smooth bump between sampled parameters can create extra crossings without changing any sampled values or [derivatives](../../../../../derivative.md). With finitely many isolated transverse intersections and convergent certified enclosures, the algorithm terminates to any prescribed tolerance. For tangencies it either uses stronger representation tests or reports unresolved possible-contact intervals, rather than silently omitting them.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
