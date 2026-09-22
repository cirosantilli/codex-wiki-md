<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Under a smooth coordinate change $x\mapsto x'$, a [contravariant vector](../../../../contravariant-vector.md) obeys

$$
\boxed{T'^a=\frac{\partial x'^a}{\partial x^b}T^b.}
$$

The [scalar](../../../../scalar.md)-contraction hypothesis gives $U'_a(\partial x'^a/\partial x^b)T^b=U_bT^b$ for every choice of $T^b$. Equality of all coefficients and multiplication by the inverse [Jacobian matrix](../../../../jacobian-matrix.md) give $\boxed{U'_a=(\partial x^b/\partial x'^a)U_b}$, the [covector](../../../../covector.md) law.

Let $V^a=dx^a/ds$ be a [timelike geodesic](../../../../timelike-geodesic.md) tangent. [Metric compatibility](../../../../metric-compatibility.md) and the [geodesic equation](../../../../geodesic-equation.md) give

$$
\frac d{ds}(T_aV^a)=V^aV^b\nabla_bT_a+T_a\frac{DV^a}{Ds}
=V^aV^b\nabla_{(a}T_{b)}.
$$

A [Killing vector](../../../../killing-vector-field-split.md) therefore gives a conserved contraction. Conversely, if that contraction is conserved along every [timelike geodesic](../../../../timelike-geodesic.md), then at any point its symmetric [tensor](../../../../tensor.md) $S_{ab}=\nabla_{(a}T_{b)}$ satisfies $S_{ab}V^aV^b=0$ for every unit timelike initial tangent. Homogeneity extends this to the entire [timelike cone](../../../../timelike-cone.md), an open set of tangent vectors. A [quadratic polynomial](../../../../quadratic-polynomial.md) vanishing on an open set has every coefficient zero, so $\boxed{\nabla_{(a}T_{b)}=0}$. Considering a single selected [geodesic](../../../../geodesic.md) would not suffice. This is the [Converse geodesic characterization of a Killing vector](../../../../converse-geodesic-characterization-of-a-killing-vector.md).

For the given exterior transformation, differentiating at fixed $r$ gives

$$
\boxed{T=\partial_t=-\frac{U}{4m}\partial_U+\frac{V}{4m}\partial_V.}
$$

The transformation also gives $UV=(2m-r)e^{r/(2m)}$. This determines $r$ smoothly for $r>0$ throughout $UV<2m$. The flow of the displayed vector field rescales $U\mapsto e^{-\lambda/(4m)}U$, $V\mapsto e^{\lambda/(4m)}V$. It leaves $UV$, $r$, $dU\,dV$ and the angular metric unchanged. Thus it preserves the full metric everywhere in that region and extends as a global [Killing field](../../../../killing-vector-field-split.md), not merely by a formal exterior coordinate substitution.

Its squared norm is

$$
\boxed{g(T,T)=-\frac{UV}{r}e^{-r/(2m)}=1-\frac{2m}{r}.}
$$

It is **timelike** for $UV<0$ ($r>2m$), **spacelike** for $0<UV<2m$ ($0<r<2m$), and a nonzero **[null vector](../../../../null-vector.md)** on either horizon $UV=0$ away from $U=V=0$. At $U=V=0$ it is the **[zero vector](../../../../zero-vector.md)**, on the whole [bifurcation surface](../../../../bifurcation-surface.md) of angular points. Zero must be distinguished from a nonzero [null vector](../../../../null-vector.md). This is the [Schwarzschild time-translation Killing field in Kruskal coordinates](../../../../schwarzschild-time-translation-killing-field-in-kruskal-coordinates.md).

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the mathematical physics course of the University of Oxford](../../../split.md)
5. [Mathematical physics course of the University of Oxford](../../../../mathematical-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
