<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Raise perturbation indices with the background [Minkowski metric](../../../../../minkowski-metric.md). To first order, the inverse metric is $g^{ik}=\eta^{ik}-\epsilon h^{ik}+O(\epsilon^2)$ and the [Levi-Civita connection](../../../../../levi-civita-connection.md) is

$$
\Gamma^i{}_{km}=\frac\epsilon2\eta^{ij}(h_{jk,m}+h_{jm,k}-h_{km,j})+O(\epsilon^2).
$$

Quadratic connection products in the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) are of order $\epsilon^2$. Substitution into the paper's curvature convention gives

$$
\boxed{R_{ikmn}=\frac\epsilon2(h_{im,kn}+h_{nk,im}-h_{mk,in}-h_{in,km})+O(\epsilon^2).}
$$

The signs follow the convention on the cover sheet; reversing the curvature definition would reverse this expression.

The gauge freedom is the freedom to identify points of the perturbed spacetime with points of the flat background in slightly different coordinates. Under the passive infinitesimal change $x'^i=x^i+\epsilon\xi^i(x)$, the metric transformation law gives the [linearized coordinate gauge transformation](../../../../../linearized-coordinate-gauge-transformation.md)

$$
h'_{ik}=h_{ik}-\partial_i\xi_k-\partial_k\xi_i.
$$

Thus a nonzero perturbation can partly represent a coordinate change rather than physical curvature. Substituting this variation into the displayed curvature formula gives

$$
\delta R_{ikmn}=-\frac\epsilon2\left(
\xi_{i,mkn}+\xi_{m,ikn}+\xi_{n,kim}+\xi_{k,nim}
-\xi_{m,kin}-\xi_{k,min}-\xi_{i,nkm}-\xi_{n,ikm}\right)=0.
$$

Each third derivative has a partner differing only by the order of its commuting partial derivatives. This explicitly proves [gauge invariance of the linearized Riemann tensor](../../../../../gauge-invariance-of-the-linearized-riemann-tensor.md). The restriction to first order matters: a coordinate change acts on nonzero background curvature as well, but the background here is flat.

Define the [trace-reversed metric perturbation](../../../../../trace-reversed-metric-perturbation.md) and [d'Alembert operator](../../../../../d-alembert-operator.md) by

$$
h=\eta^{ik}h_{ik},\qquad
\bar h_{ik}=h_{ik}-\frac12\eta_{ik}h,\qquad
\Box=\eta^{ik}\partial_i\partial_k=\partial_t^2-\partial_x^2-\partial_y^2-\partial_z^2.
$$

In four dimensions $\bar h=-h$ and $h_{ik}=\bar h_{ik}-\tfrac12\eta_{ik}\bar h$. Contract the curvature formula using $R_{ik}=R^m{}_{imk}$:

$$
R_{ik}=\frac\epsilon2\left(\Box h_{ik}+\partial_i\partial_kh
-\partial_i\partial^a h_{ak}-\partial_k\partial^a h_{ai}\right),\qquad
R=\epsilon(\Box h-\partial^a\partial^bh_{ab}),
$$

up to $O(\epsilon^2)$. Consequently the [Einstein tensor](../../../../../einstein-tensor.md) is

$$
G_{ik}=\frac\epsilon2\left(\Box\bar h_{ik}
+\eta_{ik}\partial^a\partial^b\bar h_{ab}
-\partial_i\partial^a\bar h_{ak}-\partial_k\partial^a\bar h_{ai}\right).
$$

Choose [Lorenz gauge in linearized gravity](../../../../../lorenz-gauge-in-linearized-gravity.md), $\partial^k\bar h_{ik}=0$. It can be imposed locally by solving $\Box\xi_i=\partial^k\bar h_{ik}$, since the gauge transformation changes this divergence by $-\Box\xi_i$. The remaining coordinate freedom satisfies $\Box\xi_i=0$. In this gauge,

$$
G_{ik}=\frac\epsilon2\Box\bar h_{ik},\qquad
\boxed{\Box\bar h_{ik}=-16\pi G\epsilon^{-1}T_{ik}.}
$$

This is the requested [Linearized Einstein equations](../../../../../linearized-einstein-equations.md) in the stated sign convention. Their divergence requires $\partial^kT_{ik}=0$ to this order.

For the [photon](../../../../../photon.md) beam, introduce $u=t-x$ and the constant null covector $\ell_i=(1,-1,0,0)$, so $\ell^i=(1,1,0,0)$. The [stress-energy tensor](../../../../../stress-energy-tensor.md) is

$$
T_{ik}=\epsilon\rho(u)\ell_i\ell_k.
$$

It is trace-free and conserved: $\ell^i\partial_i\rho(u)=0$. A beam-adapted particular solution, with no independently added homogeneous gravitational field, is

$$
\bar h_{ik}=h_{ik}=H(u,y,z)\ell_i\ell_k.
$$

The equality follows because its trace is zero, and the Lorenz condition holds because $\ell^k\partial_kH=0$. The field equation becomes a transverse [Poisson equation](../../../../../poisson-equation.md):

$$
\Box H=-\Delta_\perp H=-16\pi G\rho(u),\qquad
\boxed{\Delta_\perp H=16\pi G\rho(u).}
$$

For the transversely uniform source in the question, one particular solution is $H=4\pi G\rho(u)(y^2+z^2)$. Thus the sourced components can be chosen as

$$
\boxed{h_{00}=h_{11}=-h_{01}=-h_{10}=H,\qquad\text{all other components zero}.}
$$

Boundary conditions and homogeneous solutions determine additional freedom; the source does not uniquely specify every component in every gauge. In particular, taking $H$ to depend only on $t-x$ would give $\Box H=0$ and cannot solve the equation for nonzero $\rho$. The uniform idealization is not an asymptotically flat finite beam, and its quadratic particular solution is a weak-field description only where $|\epsilon H|\ll1$.

Finally consider another [photon](../../../../../photon.md) with tangent proportional to $\ell^i$. Its tangent remains null because $h_{ik}\ell^i\ell^k=0$. Moreover $h_{ik}\ell^k=0$, and since $\ell$ is constant, the connection contraction is

$$
\Gamma^i{}_{jk}\ell^j\ell^k
=\frac\epsilon2\eta^{ia}\left(2\ell^j\partial_j(h_{ak}\ell^k)-\partial_a(h_{jk}\ell^j\ell^k)\right)=0.
$$

The [geodesic equation](../../../../../geodesic-equation.md) is therefore satisfied by a straight affinely parametrized ray along the beam. Hence **co-propagating [photons](../../../../../photon.md) experience no deflection from the beam's gravitational field**. This is [parallel photon beams in linearized gravity](../../../../../parallel-photon-beams-in-linearized-gravity.md); it does not assert absence of forces on counter-propagating [photons](../../../../../photon.md) or effects from unrelated homogeneous gravitational perturbations.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
