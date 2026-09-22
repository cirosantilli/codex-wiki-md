# Green theorem

↑ **Parent:** [Vector calculus](vector-calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Green_theorem)

Green’s theorem converts circulation around a positively oriented planar boundary into the area integral of scalar curl.

Let $D$ be a bounded region in the [Euclidean plane](euclidean-plane.md) whose [boundary](boundary-of-a-set.md) is a finite union of disjoint, piecewise [smooth](smooth-function.md) [simple closed curves](simple-closed-curve.md). Suppose the [vector field](vector-field.md) $F=(P,Q)$ is [continuously differentiable](continuously-differentiable-function.md) on an [open set](open-set.md) containing the whole closed region. With positive [boundary orientation](boundary-orientation.md),

$$
\oint_{\partial D}F\cdot d\mathbf r
=\oint_{\partial D}(P\,dx+Q\,dy)
=\iint_D\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)\,dA.
$$

The [partial derivatives](partial-derivative.md) $Q_x-P_y$ give the scalar [curl](curl.md): the third component of the [curl](curl.md) of $(P,Q,0)$. For a [parametric curve](parametric-curve.md) $\gamma(t)=(x(t),y(t))$, the boundary [line integral](line-integral.md) has [integrand](integrand.md) $P(\gamma(t))x'(t)+Q(\gamma(t))y'(t)$.[Calculus Volume 3 by Gilbert Strang and others; §6.4, Theorem 6.12, equation (6.13); circulation form and its hypotheses](calculus-volume-3-by-gilbert-strang-and-others/6-4-green-s-theorem.md)

Positive [boundary orientation](boundary-orientation.md) keeps $D$ on the left as one walks along each boundary component: the outer [curve](curve.md) is counterclockwise, and curves around holes are clockwise. Every component belongs in the [line integral](line-integral.md). The [vector field](vector-field.md) must be regular throughout $D$, but need not extend into a hole.[18.02SC Multivariable Calculus, Fall 2010; V5. Simply-Connected Regions, p. 1, §1, Extended Green's Theorem, equation (1) and subdivision proof](18-02sc-multivariable-calculus-fall-2010/v5-simply-connected-regions.md)

The useful tradeoff is between boundary and interior: integrate tangential components along a [curve](curve.md), or integrate a [partial derivative](partial-derivative.md) over a region, whichever is simpler. The [boundary formula for planar area](boundary-formula-for-planar-area.md) uses this freedom in the opposite direction, recovering [area](surface-area.md) from a [line integral](line-integral.md). As a planar case of [Stokes theorem](stokes-theorem.md), [Green theorem](green-theorem.md) also explains why a local [curl](curl.md) can determine a complete boundary measurement while leaving room for the global obstruction in [Green theorem with holes](green-theorem-with-holes.md).

A short proof starts with a [rectangle](rectangle.md) $D=[a,b]\times[c,d]$. Add its four positively oriented edge [line integrals](line-integral.md):

$$
\oint_{\partial D}(P\,dx+Q\,dy)
=\int_a^b\bigl(P(x,c)-P(x,d)\bigr)\,dx
+\int_c^d\bigl(Q(b,y)-Q(a,y)\bigr)\,dy.
$$

The [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) turns the differences into [integrals](integral-split.md) of $-P_y$ and $Q_x$; [Fubini's theorem](fubini-s-theorem.md) then gives the required [double integral](double-integral.md). On subdividing a region, adjacent edge [line integrals](line-integral.md) cancel because their directions oppose. For curved boundaries, the proof uses pieces bounded by graphs and [double integrals](double-integral.md); cancellation works the same way. This is the geometric reason only the region's complete boundary survives.[Calculus Volume 3 by Gilbert Strang and others; §6.4, proof following Theorem 6.12: rectangle edge integrals and the fundamental theorem of calculus](calculus-volume-3-by-gilbert-strang-and-others/6-4-green-s-theorem.md)

**Table of contents**

- [Boundary formula for planar area](boundary-formula-for-planar-area.md)
- [Green theorem circulation examples](green-theorem-circulation-examples.md)
- [Green theorem with holes](green-theorem-with-holes.md)

## ↑ Ancestors (8)

1. [Vector calculus](vector-calculus.md)
2. [Multivariable calculus](multivariable-calculus-split.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Boundary formula for planar area](boundary-formula-for-planar-area.md)
- [Differential form](differential-form-split.md)
- [Generalized Stokes theorem](generalized-stokes-theorem.md)
- [Green theorem](green-theorem.md)
- [Green theorem circulation examples](green-theorem-circulation-examples.md)
- [Green-theorem proof of exactness on a disc](green-theorem-proof-of-exactness-on-a-disc.md)
- [Green theorem with holes](green-theorem-with-holes.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-3/9a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-3/9c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-115/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-2/3b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/25i/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a/section-d/d17/a/solution.md)
- [Vector calculus](vector-calculus.md)
