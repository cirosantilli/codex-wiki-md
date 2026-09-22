# Paper 15

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_15.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_15.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

An $n$-dimensional [smooth manifold](../../../differential-geometry.md#smooth-manifold) is a [Hausdorff space](../../../topology.md#hausdorff-space) with a countable topological base, equipped with a [smooth atlas](../../../differential-geometry.md#smooth-atlas) of [homeomorphisms](../../../topology.md#homeomorphism) from open subsets onto open subsets of $\mathbb R^n$, whose overlap maps are smooth [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism). The smooth structure is the maximal [smooth atlas](../../../differential-geometry.md#smooth-atlas) compatible with these [manifold charts](../../../differential-geometry.md#manifold-chart). Here manifolds have no boundary unless specified otherwise.

For a space with all the requested topological properties but no such atlas, take the [topological tripod](../../../topology.md#topological-tripod): three closed intervals joined at one endpoint. It is a [compact](../../../topology.md#compact-space) [connected](../../../geometry-and-topology.md#connected-space) subspace of the plane with its induced metric. A countable base of planar rational balls restricts to a countable base, the metric makes it [Hausdorff](../../../topology.md#hausdorff-space), and [compactness](../../../topology.md#compact-space) gives a finite subcover of every open cover, hence a locally finite refinement and paracompactness.

At an interior point of any arm, arbitrarily small neighborhoods are intervals. A coordinate ball in [dimension](../../../vector-space.md#dimension-vector-space) at least two would remain [connected](../../../geometry-and-topology.md#connected-space) after deleting its center; an interval does not. [Dimension](../../../vector-space.md#dimension-vector-space) zero would make the space discrete. Thus any possible [connected](../../../geometry-and-topology.md#connected-space) manifold structure would have [dimension](../../../vector-space.md#dimension-vector-space) one. But a sufficiently small neighborhood of the junction, minus the junction, has three components, whereas an interval chart has two. This contradiction rules out even a [topological manifold](../../../topology.md#topological-manifold) structure, and hence any smooth one.

The [product smooth structure](../../../differential-geometry.md#product-manifold) uses [manifold charts](../../../differential-geometry.md#manifold-chart) $(\phi,\psi):U\times V\to\phi(U)\times\psi(V)\subset\mathbb R^{m+n}$. Transition maps act separately in the two coordinate blocks and are smooth with smooth inverses. Products of countable bases give a countable base, and the product remains [Hausdorff](../../../topology.md#hausdorff-space). Therefore $\boxed{\dim(M\times N)=\dim M+\dim N}$ with this natural smooth structure.

Define the [tangent space by point derivations](../../../differential-geometry.md#tangent-space-by-point-derivations): a tangent vector at $x$ is an $\mathbb R$-linear map $D$ on [germs](../../../ringed-space.md#germ-of-a-sheaf-section) of smooth functions at $x$, satisfying $D(ab)=a(x)D(b)+b(x)D(a)$. Addition and scalar multiplication preserve this rule, so these [derivations](../../../associative-algebra.md#derivation-of-an-algebra) form a [vector space](../../../vector-space.md). In coordinates $u^1,\ldots,u^n$, the local identity

$$
h(u)-h(u(x))=\sum_i(u^i-u^i(x))h_i(u),\qquad h_i(u(x))=\partial_i h(u(x))
$$

follows by integrating the [derivative](../../../calculus.md#derivative) of $h$ along the coordinate line segment. [Derivations](../../../associative-algebra.md#derivation-of-an-algebra) annihilate constants, so it gives $Dh=\sum_iD(u^i)\partial_i h(u(x))$. The coordinate [derivations](../../../associative-algebra.md#derivation-of-an-algebra) $\partial_i|_x$ are independent since they evaluate the coordinate functions as $\delta_i^j$. Thus

$$
\boxed{T_xM=\operatorname{span}\{\partial_1|_x,\ldots,\partial_n|_x\},\qquad\dim T_xM=n}.
$$

For a [smooth map](../../../differential-geometry.md#smooth-map-between-manifolds), define the [differential of a smooth map](../../../differential-geometry.md#differential-of-a-smooth-map) intrinsically by $(f_*D)(h)=D(h\circ f)$. It is again linear and satisfies the [derivation](../../../associative-algebra.md#derivation-of-an-algebra) rule at $f(x)$, so it maps $T_xM$ into $T_{f(x)}N$. Its coordinate matrix is the Jacobian of the coordinate expression of $f$, independently of the charts by the intrinsic definition and [chain rule](../../../calculus.md#chain-rule).

Finally, a zero differential forces each target coordinate function to have all [derivatives](../../../calculus.md#derivative) zero on a small [connected](../../../geometry-and-topology.md#connected-space) source coordinate ball mapping into one target chart. Integration on straight segments makes those functions constant there. Hence $f$ is locally constant. Each nonempty fiber is both open and closed, so [connectedness](../../../geometry-and-topology.md#connected-space) gives the [zero-differential constancy theorem](../../../differential-geometry.md#zero-differential-constancy-theorem), $\boxed{f\text{ is constant}}$.

## 2

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [Riemannian metric](../../../differential-geometry.md#riemannian-metric) is a smooth field of positive-definite [symmetric bilinear forms](../../../linear-algebra.md#symmetric-bilinear-form) $g_x$ on the [tangent spaces](../../../differential-geometry.md#tangent-space), equivalently a smooth section of $\operatorname{Sym}^2T^*M$ with that positivity. Its [musical isomorphism](../../../differential-geometry.md#musical-isomorphism) is

$$
\boxed{\flat_g:TM\longrightarrow T^*M,\qquad v\longmapsto g(v,\cdot)}.
$$

Nondegeneracy makes every fiber map an isomorphism. In coordinates the map has matrix $g_{ij}$, and its inverse $\sharp_g$ has matrix $g^{ij}$. Smoothness of the inverse follows from the inverse-matrix formula and the nonvanishing [determinant](../../../linear-algebra.md#determinant). Both maps cover the identity on $M$, giving a smooth [vector bundle isomorphism](../../../fiber-bundle.md#vector-bundle-isomorphism).

For [local flattening of a Riemannian metric](../../../differential-geometry.md#local-flattening-of-a-riemannian-metric), choose a [manifold chart](../../../differential-geometry.md#manifold-chart) neighborhood $V$ around $p$ with closure contained in $U$, and let $h=\phi^*\delta$ on $V$. Choose a [smooth bump function](../../../partial-differential-equation.md#smooth-bump-function) $0\leq\chi\leq1$, with [compact support](../../../function.md#compact-support) in $V$ and equal to one on a smaller neighborhood $W$ of $p$. Set

$$
\boxed{\widetilde g=(1-\chi)g+\chi h\text{ on }V,\qquad\widetilde g=g\text{ off }V}.
$$

The formulas glue smoothly because the modification is supported strictly inside $V$. A convex combination of positive-definite forms is positive definite. On $W$ the metric is exactly $h$, so $\phi$ gives an [isometry](../../../riemannian-geometry.md#isometry) to a Euclidean open subset. Outside $U$ the original metric remains unchanged.

[Geodesic completeness](../../../riemannian-geometry.md#geodesic-completeness) means that every [geodesic](../../../riemannian-geometry.md#geodesic) with arbitrary initial point and tangent vector extends for every real affine parameter. On each [connected](../../../geometry-and-topology.md#connected-space) component, the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem) equates this with completeness of the [Riemannian distance](../../../riemannian-geometry.md#riemannian-distance).

The Euclidean-end claim needs a compact-core interpretation that is absent from its literal hypotheses. Indeed, $M=\{x\in\mathbb R^n:|x|>1\}$ with $n\geq2$, $X=\varnothing$ and $g=\delta$ satisfy those hypotheses. The [geodesic](../../../riemannian-geometry.md#geodesic) $\gamma(t)=(2-t)e_1$ reaches the missing unit sphere at $t=1$ and cannot continue within $M$. Thus the printed assumptions alone do not prove completeness.

Here is the intended [compact-core completeness for a Euclidean end](../../../riemannian-geometry.md#compact-core-completeness-for-a-euclidean-end). Write $\Phi:M\setminus X\to\{|x|>1\}$ for the end coordinates and assume additionally that

$$
K_R=X\cup\Phi^{-1}\{1<|x|\leq R\}
$$

is [compact](../../../topology.md#compact-space) for every sufficiently large $R$. Choose such an $R$ beyond the metric transition and large enough to include the initial point of a [geodesic](../../../riemannian-geometry.md#geodesic). Its speed $s$ is constant. On every segment outside $K_R$, the Euclidean radius changes at a rate at most $s$, so over a finite parameter interval it cannot exceed $R+sT$. The full segment therefore stays in the [compact](../../../topology.md#compact-space) set $K_{R+sT}$. Its velocities also stay in a [compact](../../../topology.md#compact-space) subset of $TM$, since their metric [norm](../../../functional-analysis.md#norm) is fixed and the base set is [compact](../../../topology.md#compact-space). The smooth [geodesic](../../../riemannian-geometry.md#geodesic) ordinary differential equation consequently extends past any supposed finite endpoint. The reversed-time argument is identical. This proves completeness under the compact-core condition, and explains exactly what the exterior-of-a-ball counterexample lacks.

For [upward stability of Riemannian completeness](../../../riemannian-geometry.md#upward-stability-of-riemannian-completeness), lengths of all curves satisfy $L_{\widetilde g}\geq L_g$, hence $d_{\widetilde g}\geq d_g$. A $d_{\widetilde g}$-Cauchy sequence is therefore $d_g$-Cauchy and has a limit $p$ because $g$ is complete. Smooth positive-definite metrics induce the manifold topology. More explicitly, on a small coordinate ball around $p$, $\widetilde g$ has a bounded largest matrix [eigenvalue](../../../linear-operator-theory.md#eigenvalue), so the coordinate straight segment gives $d_{\widetilde g}(p,q)\leq C|\phi(q)-\phi(p)|$. Thus convergence to $p$ is also in $d_{\widetilde g}$. That distance is complete, and Hopf-Rinow yields

$$
\boxed{\widetilde g\geq g,\quad g\text{ complete}\quad\Longrightarrow\quad\widetilde g\text{ complete}}.
$$

For disconnected $M$, apply this argument on each component.

## 3

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Combining [metric compatibility](../../../fiber-bundle.md#metric-compatibility) with the [torsion-free](../../../fiber-bundle.md#torsion-free-connection) condition forces the [Koszul formula](../../../fiber-bundle.md#koszul-formula):

$$
2g(\nabla_XY,Z)=Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
$$

Nondegeneracy of $g$ proves uniqueness of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). For existence, use the right side to define $2g(\nabla_XY,Z)$. Expanding brackets shows that this expression is $C^\infty$-linear in $Z$, so it defines a smooth one-form; the [musical isomorphism](../../../differential-geometry.md#musical-isomorphism) gives the required [vector field](../../../calculus.md#vector-field). The same expansion shows $\nabla_{aX}Y=a\nabla_XY$, additivity, and $\nabla_X(aY)=X(a)Y+a\nabla_XY$, establishing the connection rules. Subtracting the formulas with $X,Y$ exchanged gives $\nabla_XY-\nabla_YX=[X,Y]$. Adding the formulas pairing $\nabla_XY$ with $Z$ and $\nabla_XZ$ with $Y$ gives [metric compatibility](../../../fiber-bundle.md#metric-compatibility). Thus this construction has both required properties.

In coordinate [vector fields](../../../calculus.md#vector-field) the brackets vanish. Consequently the [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) and coordinate [derivative](../../../calculus.md#derivative) are

$$
\boxed{\Gamma^k_{ij}=\frac12g^{k\ell}(\partial_i g_{j\ell}+\partial_j g_{i\ell}-\partial_\ell g_{ij}),\qquad
\nabla_XY=\left(X^i\partial_iY^k+\Gamma^k_{ij}X^iY^j\right)\partial_k}.
$$

Repeated indices are summed. The displayed connection type in the source is best understood in its standard form on two [vector fields](../../../calculus.md#vector-field); if the first input is an individual tangent vector at a point, the output lies in the tangent fiber at that point rather than in the space of global sections.

For the [parallel metrics with a common Levi-Civita connection](../../../general-relativity.md#parallel-metrics-with-a-common-levi-civita-connection), let $\gamma$ be a piecewise smooth path from the point $x$ of equality to any $y$. [Connected](../../../geometry-and-topology.md#connected-space) [smooth manifolds](../../../differential-geometry.md#smooth-manifold) admit such paths because coordinate balls are path [connected](../../../geometry-and-topology.md#connected-space). [Parallel transport](../../../fiber-bundle.md#parallel-transport) $P_\gamma$ for the common connection is invertible and preserves both metrics. Therefore

$$
\widetilde g_y(P_\gamma u,P_\gamma v)=\widetilde g_x(u,v)=g_x(u,v)=g_y(P_\gamma u,P_\gamma v).
$$

Every pair of tangent vectors at $y$ arises this way, so $\boxed{\widetilde g=g}$ everywhere.

Dropping the agreement at one point removes the conclusion. For any constant $c>0$, $\widetilde g=cg$ has the same [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol). Nor must the two metrics be proportional: on $\mathbb R^n$, $n\geq2$, the constant metrics $\sum_i(dx^i)^2$ and $2(dx^1)^2+\sum_{i\geq2}(dx^i)^2$ both have zero connection coefficients. In general write $\widetilde g(u,v)=g(Au,v)$. Since both metrics are parallel, $0=(\nabla_X\widetilde g)(Y,Z)=g((\nabla_XA)Y,Z)$, so $\nabla A=0$. Conversely, a positive $g$-self-adjoint parallel $A$ makes the same [torsion-free](../../../fiber-bundle.md#torsion-free-connection) connection compatible with $\widetilde g$, proving equality of their [Levi-Civita connections](../../../general-relativity.md#levi-civita-connection). Thus one-point agreement specifies $A=I$ and forces it everywhere; without it, nontrivial parallel choices can remain.

## 4

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Fix the curvature convention

$$
\boxed{R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z}.
$$

To prove [tensoriality](../../../fiber-bundle.md#tensoriality), use $[hX,Y]=h[X,Y]-Y(h)X$ and the connection rules. The two $Y(h)\nabla_XZ$ terms cancel, giving $R(hX,Y)Z=hR(X,Y)Z$. Antisymmetry in $X,Y$ gives linearity over smooth functions in the second input. Expanding the third input gives

$$
R(X,Y)(hZ)=hR(X,Y)Z+\bigl(X(Yh)-Y(Xh)-[X,Y]h\bigr)Z=hR(X,Y)Z.
$$

It is therefore a smooth [tensor](../../../linear-algebra.md#tensor) of type $(1,3)$. Lowering the output with $g$ gives the type $(0,4)$ [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) $R_4(X,Y,Z,W)=g(R(X,Y)Z,W)$.

For an independent pair $X,Y$, define [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) by

$$
K(\operatorname{span}\{X,Y\})=\frac{g(R(X,Y)Y,X)}{g(X,X)g(Y,Y)-g(X,Y)^2}.
$$

Metric compatibility gives $g(R(X,Y)Z,W)=-g(R(X,Y)W,Z)$ by applying $XY-YX-[X,Y]$ to $g(Z,W)$. Together with antisymmetry in $X,Y$, this shows that replacing the pair by $(aX+bY,cX+dY)$ multiplies both numerator and denominator by $(ad-bc)^2$. Thus the value depends only on the plane. Define [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) by $\operatorname{Ric}(Y,Z)=\sum_i g(R(e_i,Y)Z,e_i)$ for any [orthonormal basis](../../../linear-algebra.md#orthonormal-basis); a trace is independent of the [orthonormal basis](../../../linear-algebra.md#orthonormal-basis).

For the [curvature of the round unit sphere](../../../second-fundamental-form.md#curvature-of-the-round-unit-sphere), the outward unit normal is the position vector $p$. The tangential projection of ambient differentiation is [torsion-free](../../../fiber-bundle.md#torsion-free-connection) and has [metric compatibility](../../../fiber-bundle.md#metric-compatibility), so uniqueness identifies it with $\nabla$. Ambient differentiation $D$ satisfies $D_Xp=X$ and

$$
D_XY=\nabla_XY-g(X,Y)p,
$$

since differentiating $g(Y,p)=0$ gives its normal component. The ambient curvature is zero. Take tangential components of $D_XD_YZ-D_YD_XZ-D_{[X,Y]}Z=0$ to obtain

$$
\boxed{R(X,Y)Z=g(Y,Z)X-g(X,Z)Y}.
$$

Hence

$$
\boxed{R_4(X,Y,Z,W)=g(Y,Z)g(X,W)-g(X,Z)g(Y,W)}.
$$

Every two-plane has [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) one. Tracing the first formula gives $\operatorname{Ric}(Y,Z)=ng(Y,Z)-g(Y,Z)$, and consequently

$$
\boxed{\operatorname{Ric}=(n-1)g,\qquad\Lambda=n-1}.
$$

Thus the sphere is an [Einstein manifold](../../../second-fundamental-form.md#einstein-manifold). When $n=1$ there are no tangent two-planes, the curvature [tensor](../../../linear-algebra.md#tensor) is zero and the same Ricci formula gives zero. The declared slot convention fixes all signs.

## 5

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [Bonnet-Myers theorem](../../../second-fundamental-form.md#myers-s-theorem) says that a [connected](../../../geometry-and-topology.md#connected-space) [geodesically complete](../../../riemannian-geometry.md#geodesic-completeness) $n$-dimensional [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold), with $n\geq2$ and $\operatorname{Ric}\geq(n-1)\kappa g$ for a constant $\kappa>0$, has

$$
\boxed{\operatorname{diam}M\leq\frac{\pi}{\sqrt\kappa},\qquad M\text{ compact},\qquad |\pi_1(M)|<\infty}.
$$

The [dimension](../../../vector-space.md#dimension-vector-space) and positive lower bound are essential: in [dimension](../../../vector-space.md#dimension-vector-space) one the Ricci condition is vacuous, and a zero lower bound does not imply bounded diameter.

By Hopf-Rinow, any two distinct points have a unit-speed [minimizing geodesic](../../../riemannian-geometry.md#minimizing-geodesic) $\gamma:[0,L]\to M$. Choose parallel orthonormal fields $E_1,\ldots,E_{n-1}$ perpendicular to its tangent $T$. For the endpoint-vanishing fields $V_i(t)=\sin(\pi t/L)E_i(t)$, the [second variation of geodesic energy](../../../riemannian-geometry.md#second-variation-of-geodesic-energy) gives nonnegative index forms

$$
I(V_i,V_i)=\int_0^L\bigl(|D_tV_i|^2-g(R(V_i,T)T,V_i)\bigr)\,dt\geq0.
$$

Summing and using the Ricci lower bound produces the [sine index-form bound for positive Ricci curvature](../../../riemannian-geometry.md#sine-index-form-bound-for-positive-ricci-curvature):

$$
0\leq\sum_iI(V_i,V_i)
\leq(n-1)\int_0^L\left[\frac{\pi^2}{L^2}\cos^2(\pi t/L)-\kappa\sin^2(\pi t/L)\right]dt
=\frac{n-1}{2}\left(\frac{\pi^2}{L}-\kappa L\right).
$$

If $L>\pi/\sqrt\kappa$, the last expression is negative, a contradiction. This proves the diameter bound. Hopf-Rinow makes closed bounded sets [compact](../../../topology.md#compact-space), so the entire manifold is [compact](../../../topology.md#compact-space).

Give the [universal cover](../../../algebraic-topology.md#universal-cover) the pullback metric. [Local isometry](../../../differential-geometry.md#local-isometry) preserves its Ricci bound, and lifting complete base [geodesics](../../../riemannian-geometry.md#geodesic) proves completeness of the cover. The same diameter and [compactness](../../../topology.md#compact-space) argument applies there. A fiber of the covering is closed and discrete, hence finite in this [compact](../../../topology.md#compact-space) cover; its cardinality is that of the [fundamental group](../../../algebraic-topology.md#fundamental-group). This proves the final assertion.

For a counterexample that also breaks the diameter conclusion, use the [incomplete positively curved strip with infinite diameter](../../../second-fundamental-form.md#incomplete-positively-curved-strip-with-infinite-diameter)

$$
M=(-\pi/4,\pi/4)\times\mathbb R,\qquad g=du^2+\cos^2u\,dv^2.
$$

The map $\Phi(u,v)=(\cos u\cos v,\cos u\sin v,\sin u)$ is a [local isometry](../../../differential-geometry.md#local-isometry) to the round unit sphere: its coordinate [derivatives](../../../calculus.md#derivative) are orthogonal, with squared lengths one and $\cos^2u$. Thus $K=1$ and $\operatorname{Ric}=g$, satisfying the required lower bound with $n=2$, $\kappa=1$.

The meridian $(u,v)=(t,0)$ is a unit-speed [geodesic](../../../riemannian-geometry.md#geodesic) and reaches the excluded boundary at $t=\pi/4$, so this metric is incomplete. Every curve joining $(0,0)$ to $(0,L)$ has length at least $\int\cos u\,|v'|\,dt\geq |L|/\sqrt2$, because $\cos u\geq1/\sqrt2$ on the strip. Therefore $\boxed{\operatorname{diam}M=\infty}$ despite the positive Ricci bound. Completeness cannot be omitted.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
