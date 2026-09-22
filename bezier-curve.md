<h1 id="bezier-curve">Bézier curve</h1>

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bézier_curve)

A [Bézier curve](bezier-curve.md) is a [parametric curve](parametric-curve.md) specified by [control points](control-point.md) $P_0,\ldots,P_n$ in a [Euclidean space](euclidean-norm.md) and the [Bernstein basis](bernstein-basis.md):

$$
C(t)=\sum_{i=0}^n b_{i,n}(t)P_i,\qquad b_{i,n}(t)=\binom ni(1-t)^{n-i}t^i,\qquad 0\leq t\leq1.
$$

Here $\binom ni$ is a [binomial coefficient](binomial-coefficient-split.md). Each coordinate is a [polynomial](polynomial-split.md) of [polynomial degree](degree-of-a-polynomial.md) at most $n$; special choices of [control points](control-point.md) can lower the [polynomial degree](degree-of-a-polynomial.md). The ordered [control points](control-point.md) form the [control polygon](control-polygon.md). A cubic [Bézier curve](bezier-curve.md) uses four [control points](control-point.md) and has the explicit form

$$
C(t)=(1-t)^3P_0+3(1-t)^2tP_1+3(1-t)t^2P_2+t^3P_3.
$$

The curve passes through $P_0$ and $P_3$; the interior [control points](control-point.md) steer its shape and need not lie on it.[MIT 6.837, Bézier Curves and Splines, slides 23–31 and 45–47, 2012](https://ocw.mit.edu/courses/6-837-computer-graphics-fall-2012/aba8735cf2cf7c71ca5d29b46873309a_MIT6_837F12_Lec01.pdf)

For a worked example, choose

$$
P_0=(0,0),\qquad P_1=(1,2),\qquad P_2=(3,2),\qquad P_3=(4,0).
$$

Substituting these [control points](control-point.md) gives

$$
C(t)=\bigl(3t+3t^2-2t^3,\;6t(1-t)\bigr),\qquad C(1/2)=\tfrac18P_0+\tfrac38P_1+\tfrac38P_2+\tfrac18P_3=(2,1.5).
$$

Here $y(t)=1.5-6(t-1/2)^2\leq1.5$, so neither interior [control point](control-point.md), both at height $2$, lies on the curve. [De Casteljau's algorithm](de-casteljau-s-algorithm.md) computes the same point using only successive [linear interpolations](linear-interpolation.md).

The endpoint [tangent vectors](tangent-vector-split.md) follow from the [Bézier derivative control polygon](bezier-derivative-control-polygon.md):

$$
C'(0)=3(P_1-P_0)=(3,6),\qquad C'(1)=3(P_3-P_2)=(3,-6).
$$

Thus the curve leaves $P_0$ toward $P_1$ and arrives at $P_3$ from $P_2$. These nonzero [derivatives](derivative.md) determine the endpoint [tangent lines](tangent-line.md); if an endpoint [derivative](derivative.md) vanishes, that formula alone does not determine its tangent direction. Endpoint handles are useful when arranging a [parametric first-derivative join of Bézier curves](parametric-first-derivative-join-of-bezier-curves.md).

The parameter $t$ is usually not [arc length](arc-length.md). For this example,

$$
C'(t)=\bigl(3+6t-6t^2,\;6-12t\bigr),\qquad \|C'(0)\|=\sqrt{45},\qquad \|C'(1/2)\|=4.5.
$$

Equal steps in $t$ therefore do not generally travel equal distances. Distance along the curve is instead the [arc length](arc-length.md), given by the [integral](integral-split.md) $s(t)=\int_0^t\|C'(u)\|\,du$; its [derivative](derivative.md) is the [norm](norm.md) of the [tangent vector](tangent-vector-split.md) and measures the rate of travel.

Two geometric facts make [Bézier curves](bezier-curve.md) especially convenient for design. First, the [Bernstein basis](bernstein-basis.md) weights are nonnegative and form a [partition of unity](partition-of-unity.md), since the [binomial theorem](binomial-theorem.md) gives $\sum_i b_{i,n}(t)=((1-t)+t)^n=1$. Hence $C(t)$ is a [convex combination](convex-combination.md) of the [control points](control-point.md) and lies in their [convex hull](convex-hull.md).[MIT 6.838, Bézier Curve and B-Spline Curve, §1.4.1, 1998](https://groups.csail.mit.edu/graphics/classes/6.838/S98/meetings/m15/) The [convex hull](convex-hull.md) is the smallest [convex set](convex-set-split.md) containing the [control points](control-point.md), not their [axis-aligned bounding box](axis-aligned-bounding-box.md). Here it is a trapezoid, strictly smaller than $[0,4]\times[0,2]$: the box corner $(0,2)$ is outside the [convex hull](convex-hull.md). The curve need not fill or touch every edge of either enclosure. The [convex hull](convex-hull.md) guarantee concerns $0\leq t\leq1$; outside that interval weights can be negative.

Second, applying an [affine map](affine-map.md) to every [control point](control-point.md) gives exactly the same result as applying it to the entire curve. For $T(x)=Ax+b$,

$$
\sum_i b_{i,n}(t)T(P_i)=A\sum_i b_{i,n}(t)P_i+b\sum_i b_{i,n}(t)=T(C(t)).
$$

This is [affine equivariance of a geometric basis](affine-equivariance-of-a-geometric-basis.md): a [translation](translation-geometry.md), [rotation](rotation-mathematics.md) or [shear mapping](shear-mapping.md) can be performed on a handful of [control points](control-point.md). For example, $T(x,y)=(2x+y,\;y+1)$ transforms the four [control points](control-point.md) to $(0,1),(4,3),(8,3),(8,1)$ and transforms the midpoint to $(5.5,2.5)$, also obtained from the same weights $(1,3,3,1)/8$.

These editable handles explain the usefulness of [Bézier curves](bezier-curve.md) in [computer aided geometric design](computer-aided-geometric-design-split.md), [vector graphics](vector-graphics.md) paths and [outline fonts](outline-font.md): a small collection of points controls an entire smooth stroke, and resizing the design preserves its mathematical shape. Cambridge's computer-graphics notes describe their use in graphic design, typography and PostScript outlines. The industrial context includes Pierre Bézier's work at Renault and Paul de Casteljau's work at Citroën.[Neil A. Dodgson and Peter Robinson, Cambridge Computer Graphics and Image Processing, slides 183 and 226–228, 2014](https://www.cl.cam.ac.uk/teaching/1415/CompGraph/cgip.pdf)

// Target: analysis.bigb

**Table of contents**

- [Bézier derivative control polygon](bezier-derivative-control-polygon.md)
  - [Parametric first-derivative join of Bézier curves](parametric-first-derivative-join-of-bezier-curves.md)
- [De Casteljau's algorithm](de-casteljau-s-algorithm.md)

## ↑ Ancestors (6)

1. [Computer aided geometric design](computer-aided-geometric-design-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (25)

- [Bézier curve](bezier-curve.md)
- [Bézier derivative control polygon](bezier-derivative-control-polygon.md)
- [Bounding volume](bounding-volume.md)
- [Control point](control-point.md)
- [Control-point influence on a curve](control-point-influence-on-a-curve.md)
- [Cubic B-spline Bézier extraction](cubic-b-spline-bezier-extraction.md)
- [De Casteljau's algorithm](de-casteljau-s-algorithm.md)
- [Knot insertion](knot-insertion.md)
- [Outline font](outline-font.md)
- [Parametric first-derivative join of Bézier curves](parametric-first-derivative-join-of-bezier-curves.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-59/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/3/ii/solution.md)
- [Quartic treble-knot representation of a quadratic B-spline](quartic-treble-knot-representation-of-a-quadratic-b-spline.md)
- [Vector graphics](vector-graphics.md)
