<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [vector field along a curve](../../../../../vector-field-along-a-curve.md) $\gamma:[a,b]\to M$ is a smooth section of the [pullback tangent bundle](../../../../../pullback-tangent-bundle.md) $\gamma^*TM$: it assigns $V(t)\in T_{\gamma(t)}M$ smoothly. It need not be the restriction of one ambient vector field, since its values at different times with the same image point may differ.

Given a [Koszul connection](../../../../../affine-connection.md), use a local frame $e_j$ of $TM$ and write $V(t)=\sum_jv^j(t)e_j(\gamma(t))$. Its [covariant derivative along a curve](../../../../../covariant-derivative-along-a-curve.md) is

$$
D_tV=\sum_j\dot v^j e_j(\gamma(t))+\sum_jv^j\nabla_{\dot\gamma(t)}e_j.
$$

The first term differentiates the time-dependent coefficients, and the second uses the connection on the local frame. Under a change of frame, differentiating the change matrix supplies exactly the extra term in the connection transformation, so the expression is independent of the frame. This definition also works when $\dot\gamma(t)=0$. In coordinate components it is

$$
(D_tV)^k=\dot V^k+\sum_{i,j}\Gamma^k_{ij}(\gamma(t))\dot\gamma^iV^j.
$$

A field is parallel when $D_tV=0$.

Thus a parallel field solves the linear system $\dot v=-A(t)v$, with smooth coefficient matrix $A(t)$. Given its value at one time, existence and uniqueness for a [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) determine it on each coordinate segment. To obtain it on all of $[a,b]$, cover the compact parameter interval by finitely many frame neighborhoods and subdivide so that each closed subinterval lies in one such neighborhood. The coefficients are bounded on each subinterval, and the standard estimate $\|v(t)\|\le\|v(t_0)\|\exp(\int\|A(s)\|ds)$ prevents finite-time blowup. The solutions match uniquely at the subdivision points. This proves existence and uniqueness of the requested global parallel field.

Define [parallel translation](../../../../../parallel-transport.md) by $\tau_t(v)=V_v(t)$, where $V_v(a)=v$ and $D_tV_v=0$. Linearity of the equation and uniqueness make $\tau_t$ linear. Solving the same equation backwards gives its inverse; equivalently, a solution zero at time $t$ must be identically zero. Therefore

$$
\boxed{\tau_t:T_{\gamma(a)}M\xrightarrow{\sim}T_{\gamma(t)}M.}
$$

A [metric connection](../../../../../metric-connection.md) for a [Riemannian metric](../../../../../riemannian-metric.md) satisfies $\nabla g=0$, or

$$
Xg(Y,Z)=g(\nabla_XY,Z)+g(Y,\nabla_XZ).
$$

Pulling this identity along the curve gives

$$
\frac d{dt}g(V,W)=g(D_tV,W)+g(V,D_tW).
$$

For parallel fields the right side vanishes, proving

$$
\boxed{g_{\gamma(t)}(\tau_tv,\tau_tw)=g_{\gamma(a)}(v,w).}
$$

For a piecewise smooth path compose the [parallel transport](../../../../../parallel-transport.md) maps on its smooth segments. On a closed path their domain and codomain are the same tangent space, so the resulting map is orthogonal. Its determinant need not be positive on a nonorientable surface.

An explicit reflection example is the [reflection holonomy along a closed projective geodesic](../../../../../reflection-holonomy-along-a-closed-projective-geodesic.md). Give $\mathbb{RP}^2$ the round metric induced from the sphere by the antipodal quotient. The [Levi-Civita connection](../../../../../levi-civita-connection.md) descends because the antipodal map is an isometry, so the quotient map is a local isometry carrying geodesics and parallel fields to their counterparts. The great-circle arc

$$
c(t)=(\cos t,\sin t,0),\qquad0\le t\le\pi,
$$

projects to a smooth closed [geodesic](../../../../../geodesic.md): $c(t+\pi)=-c(t)$, including all derivatives under the quotient identification. Along it the fields

$$
E_1(t)=\dot c(t)=(-\sin t,\cos t,0),\qquad E_2(t)=(0,0,1)
$$

are parallel. The first is the velocity of a great-circle geodesic. The second is tangent, unit length, and orthogonal to the first. Metric compatibility makes its covariant derivative orthogonal to both frame vectors: differentiate its constant length and its zero inner product with the parallel first vector. Its derivative therefore vanishes in the two-dimensional tangent plane. At $t=\pi$, $E_1(\pi)=-E_1(0)$ and $E_2(\pi)=E_2(0)$. Identifying the endpoint with the start through the derivative of the antipodal map, namely $-I$, fixes the returned $E_1$ and negates the returned $E_2$. Hence

$$
\boxed{\tau(E_1(0))=E_1(0),\qquad\tau(E_2(0))=-E_2(0),\qquad[\tau]=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.}
$$

This is a reflection fixing the geodesic direction.

Finally orient the unit sphere outward and traverse a [spherical triangle](../../../../../spherical-triangle.md) with its interior on the left. Let its angles be $\alpha,\beta,\gamma$. Its [parallel transport](../../../../../parallel-transport.md) preserves both the metric and orientation, so is a rotation by some angle $\delta$ in the initial tangent plane. On each geodesic side the unit tangent is parallel. At a vertex with angle $\alpha$, the actual forward tangent turns left by $\pi-\alpha$ relative to the transported incoming tangent. Tracking the tangent around all three sides and making those three corner turns returns it to its initial direction.

Rotations of oriented two-dimensional tangent planes commute with orientation-preserving parallel transport. Consequently the total angle in this tracking procedure is the transport angle plus the three corner turns:

$$
\delta+(\pi-\alpha)+(\pi-\beta)+(\pi-\gamma)\equiv0\pmod{2\pi}.
$$

This determines [parallel transport around a spherical triangle](../../../../../parallel-transport-around-a-spherical-triangle.md) as

$$
\boxed{\delta\equiv\alpha+\beta+\gamma-\pi\pmod{2\pi},\qquad[\tau]=\begin{pmatrix}\cos\delta&-\sin\delta\\\sin\delta&\cos\delta\end{pmatrix}.}
$$

By the [spherical excess formula](../../../../../spherical-excess-formula.md), this is rotation by the enclosed area on the unit sphere. Reversing traversal negates the angle. For an octant triangle all three angles are $\pi/2$, giving a positive $\pi/2$ rotation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
