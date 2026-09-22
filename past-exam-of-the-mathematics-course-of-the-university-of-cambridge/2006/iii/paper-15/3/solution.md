<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $p,q\in M$, define the [Riemannian distance](../../../../../riemannian-distance.md) by

$$
\boxed{d_g(p,q)=\inf\{L_g(c):c\text{ is piecewise smooth from }p\text{ to }q\},\qquad
L_g(c)=\int|\dot c(t)|_g\,dt.}
$$

A [connected](../../../../../connected-space.md) [smooth manifold](../../../../../smooth-manifold.md) is locally path [connected](../../../../../connected-space.md), so any two points are joined by a finite concatenation of coordinate paths. Thus the infimum is finite. It is nonnegative, $d_g(p,p)=0$, and reversing a [curve](../../../../../curve.md) proves symmetry. Concatenating two [curves](../../../../../curve.md) whose lengths approach their respective infima proves the [triangle inequality](../../../../../triangle-inequality.md).

For positivity and the topology, choose a coordinate ball about $p$ whose closure is contained in a chart. On its closure there are constants $0<c<C$ with

$$
c|v|_{\mathrm{Eucl}}\le |v|_g\le C|v|_{\mathrm{Eucl}}.
$$

A [curve](../../../../../curve.md) staying in the ball has length at least $c$ times its coordinate displacement. A [curve](../../../../../curve.md) leaving it must first reach its boundary, costing at least $c$ times the positive coordinate distance from $p$ to that boundary. Therefore a distinct $q$ has $d_g(p,q)>0$, whether it lies inside or outside the ball. For $q$ sufficiently close to $p$, the coordinate line segment gives $d_g(p,q)\le C|x(q)-x(p)|$, while the preceding lower bounds prevent a short [curve](../../../../../curve.md) from taking a shortcut outside the chart. These inequalities prove that the [Riemannian distance induces the manifold topology](../../../../../riemannian-distance-induces-the-manifold-topology.md). In particular it defines a genuine [metric space](../../../../../metric-space.md).

A [Riemannian manifold](../../../../../riemannian-manifold.md) is [geodesically complete](../../../../../geodesic-completeness.md) if every maximal affinely parametrized [geodesic](../../../../../geodesic.md) exists for all real parameter values. We prove both implications of the [Hopf-Rinow theorem](../../../../../hopf-rinow-theorem.md) rather than assuming global distance minimizers.

First assume completeness as a [metric space](../../../../../metric-space.md). Let a constant-speed [geodesic](../../../../../geodesic.md) have a finite maximal right endpoint $b$. The bound $d_g(\gamma(t),\gamma(s))\le c|t-s|$ makes $\gamma(t)$ a [Cauchy sequence](../../../../../cauchy-sequence.md) as $t\uparrow b$, hence gives a limit $p\in M$. The distance topology just established puts the final portion inside a relatively [compact](../../../../../compact-space.md) coordinate ball about $p$. The positive lower bound on the [Riemannian metric](../../../../../riemannian-metric.md) bounds all coordinate velocity components. The [Christoffel symbols](../../../../../christoffel-symbol.md) are bounded on the closure of that ball, and the [geodesic equation](../../../../../geodesic-equation.md)

$$
\ddot x^i=-\Gamma^i_{jk}(x)\dot x^j\dot x^k
$$

then bounds the coordinate acceleration. The velocity has a limit $v$ as $t\uparrow b$. Local existence and uniqueness for the [geodesic equation](../../../../../geodesic-equation.md) with data $(p,v)$ continue $\gamma$ through $b$, contradicting maximality. The same argument applies at a finite left endpoint. Hence **metric completeness implies [geodesic completeness](../../../../../geodesic-completeness.md)**.

Conversely assume [geodesic completeness](../../../../../geodesic-completeness.md). Fix $p,q$, put $r=d_g(p,q)>0$, and choose $0<\epsilon<r$ so small that a closed radius-$2\epsilon$ normal ball about $p$ lies inside a [convex normal neighborhood](../../../../../convex-normal-neighbourhood.md). By the [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md), its radial [geodesics](../../../../../geodesic.md) minimize; a [curve](../../../../../curve.md) leaving the larger ball cannot improve on a radius-$\epsilon$ radial segment. Thus the radius-$\epsilon$ [geodesic sphere](../../../../../geodesic-sphere.md) $S_\epsilon(p)$ is [compact](../../../../../compact-space.md) and consists of points at distance exactly $\epsilon$ from $p$.

The [distance splitting through a small geodesic sphere](../../../../../distance-splitting-through-a-small-geodesic-sphere.md) has an elementary proof here. Every path from $p$ to $q$ must cross $S_\epsilon(p)$, and its initial portion has length at least $\epsilon$. Hence

$$
r\ge\epsilon+\min_{x\in S_\epsilon(p)}d_g(x,q).
$$

The [triangle inequality](../../../../../triangle-inequality.md) proves the reverse bound. Continuity of $d_g(\cdot,q)$ and [compactness](../../../../../compact-space.md) give a point $x$ achieving the minimum, so $d_g(x,q)=r-\epsilon$. Let $\gamma(t)=\exp_p(tv)$ be the complete unit-speed radial [geodesic](../../../../../geodesic.md) through $x$ at time $\epsilon$.

Consider the closed subset

$$
A=\{t\in[\epsilon,r]:d_g(p,\gamma(t))=t,\quad d_g(\gamma(t),q)=r-t\}.
$$

It is nonempty since $\epsilon\in A$, and has a largest member $t_*$. Suppose $t_*<r$. At $x_*=\gamma(t_*)$, choose a small normal [sphere](../../../../../sphere.md) of radius $\eta<r-t_*$ and repeat the splitting argument. It supplies a radial endpoint $y$ with

$$
d_g(x_*,y)=\eta,\qquad d_g(y,q)=r-t_*-\eta.
$$

The [triangle inequality](../../../../../triangle-inequality.md) gives $d_g(p,y)\ge t_*+\eta$, while the broken path following $\gamma$ to $x_*$ and then the short radial segment to $y$ has exactly that length. It is therefore minimizing. Its two velocities at the joining point must agree: if unit incoming and outgoing velocities are $u,w$, moving the join in direction $w-u$ changes the sum of lengths by $-|u-w|^2$ to first order, using the [first variation of geodesic energy](../../../../../first-variation-of-geodesic-energy.md) or the equivalent unit-speed length formula. A corner would strictly shorten it. Uniqueness of the [geodesic equation](../../../../../geodesic-equation.md) consequently gives $y=\gamma(t_*+\eta)$, contradicting the maximality of $t_*$. Thus $t_*=r$, $\gamma(r)=q$, and $\gamma|_{[0,r]}$ is a [minimizing geodesic](../../../../../minimizing-geodesic.md).

This [radial continuation proof of Hopf-Rinow](../../../../../radial-continuation-proof-of-hopf-rinow.md) also proves [compactness](../../../../../compact-space.md) of closed balls. For every $R\ge0$,

$$
\overline B_g(p,R)=\exp_p\{v\in T_pM:|v|\le R\}.
$$

The inclusion from right to left follows from the length of a radial [geodesic](../../../../../geodesic.md); the reverse inclusion uses the minimizing [geodesic](../../../../../geodesic.md) just constructed. The [Riemannian exponential map](../../../../../exponential-map-riemannian-geometry.md) is defined on all of $T_pM$ by [geodesic completeness](../../../../../geodesic-completeness.md), and the closed tangent ball is [compact](../../../../../compact-space.md) in a finite-dimensional [vector space](../../../../../vector-space-split.md). Its continuous image is [compact](../../../../../compact-space.md). Every [Cauchy sequence](../../../../../cauchy-sequence.md) is bounded, hence has a convergent subsequence in such a ball, and the Cauchy property makes the whole sequence converge. Therefore **[geodesic completeness](../../../../../geodesic-completeness.md) implies metric completeness**, completing both directions.

For the [hyperbolic plane](../../../../../hyperbolic-plane.md), use the [upper half-plane model](../../../../../poincare-half-plane-model.md) with $g=(dx^2+dy^2)/y^2$, $y>0$. Its [geodesic equation](../../../../../geodesic-equation.md) is

$$
x''-\frac{2x'y'}y=0,\qquad y''+\frac{x'^2-y'^2}y=0.
$$

Every nonconstant unit-speed solution is either a vertical [curve](../../../../../curve.md) $x=a$, $y=be^{\pm t}$ or, after translating and possibly reversing $t$,

$$
x(t)=a+R\tanh(t-t_0),\qquad y(t)=R\operatorname{sech}(t-t_0),\qquad R>0.
$$

Substitution verifies both equations and $g(\dot\gamma,\dot\gamma)=1$. These [curves](../../../../../curve.md) cover every unit initial tangent: a nonvertical tangent at $(x,y)$ determines the circle center $a=x+yy'/x'$ and radius $R=\sqrt{(x-a)^2+y^2}$, and its orientation determines the sign of the parameter. Constant solutions and constant-speed rescalings cover arbitrary initial velocities. In every case $y(t)>0$ for all finite $t$, and the solution is defined for every real $t$. Thus **the real [hyperbolic plane](../../../../../hyperbolic-plane.md) is [geodesically complete](../../../../../geodesic-completeness.md)**, directly, and the proved [Hopf-Rinow theorem](../../../../../hopf-rinow-theorem.md) also makes its distance complete.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
