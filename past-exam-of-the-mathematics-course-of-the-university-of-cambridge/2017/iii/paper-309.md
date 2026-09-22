# Paper 309

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_309.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_309.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $D=\operatorname{diag}(a_1,\ldots,a_{n+1})$. The invertible [linear map](../../../vector-space.md#linear-map) $x\mapsto u=Dx$ takes the [ellipsoid](../../../geometry-and-topology.md#ellipsoid) to the unit [sphere](../../../geometry-and-topology.md#sphere) $S^n$. Write $u=(v,s)$ with $v\in\mathbb R^n$, and let $N=(0,1)$ and $S=(0,-1)$ be its two poles. The following two [stereographic projections](../../../complex-analysis.md#stereographic-projection) define [manifold charts](../../../differential-geometry.md#manifold-chart) on the ellipsoid:

$$
U_N=\mathcal Q_n\setminus\{D^{-1}N\},\qquad \chi_N(x)=\frac{v}{1-s},\qquad U_S=\mathcal Q_n\setminus\{D^{-1}S\},\qquad \chi_S(x)=\frac{v}{1+s}.
$$

Their ranges are $\mathbb R^n$. With $r^2=|w|^2$, their inverses, followed by $D^{-1}$, are

$$
\chi_N^{-1}(w)=D^{-1}\left(\frac{2w}{1+r^2},\frac{r^2-1}{1+r^2}\right),\qquad \chi_S^{-1}(w)=D^{-1}\left(\frac{2w}{1+r^2},\frac{1-r^2}{1+r^2}\right).
$$

These are continuous and [smooth functions](../../../analysis.md#smooth-function), and directly satisfy the defining constraint. On the overlap, the [smooth transition map](../../../differential-geometry.md#smooth-transition-map) is

$$
\boxed{\chi_S\circ\chi_N^{-1}(w)=\frac{w}{|w|^2}\quad(w\ne0).}
$$

It is its own inverse and is smooth away from zero. The two domains are open in the [subspace topology](../../../topology.md#subspace-topology) and cover the ellipsoid. Its [subspace topology](../../../topology.md#subspace-topology) is inherited from [Euclidean space](../../../functional-analysis.md#euclidean-norm), so the ellipsoid is [Hausdorff](../../../topology.md#hausdorff-space) and has a [second-countable space](../../../topology.md#second-countable-space) topology. Thus these charts form a [smooth atlas](../../../differential-geometry.md#smooth-atlas) and make it an $n$-dimensional [smooth manifold](../../../differential-geometry.md#smooth-manifold), with an explicit [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) to $S^n$. For the degenerate dimension $n=0$, each chart consists of a single point with range $\mathbb R^0$, and their overlap is empty; the same conclusion holds.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

At $p\in\mathcal Q$, the [differential of a smooth map](../../../differential-geometry.md#differential-of-a-smooth-map) defines the [pushforward of a vector field](../../../differential-geometry.md#pushforward-of-a-vector-field) by

$$
\boxed{(\psi_*X)_p=d\psi_p(X_p),\qquad ((\psi_*X)_p f)=X_p(f\circ\psi),\quad f\in C^\infty(N).}
$$

This is a [tangent vector](../../../differential-geometry.md#tangent-vector) at $\psi(p)$, and varies smoothly as a section of the [pullback tangent bundle](../../../fiber-bundle.md#pullback-tangent-bundle). In [local coordinates](../../../complex-analysis.md#local-coordinate) its components are $X^i(p)\partial_i\psi^a(p)$.

For a general [smooth map between manifolds](../../../differential-geometry.md#smooth-map-between-manifolds), this is a [vector field along a map](../../../fiber-bundle.md#vector-field-along-a-map), rather than an intrinsic vector field on all of $N$. A vector field $Y$ on the image can be defined only if these vectors agree whenever two points have the same image, and the resulting field must also be smooth; a [projectable vector field](../../../differential-geometry.md#projectable-vector-field) must meet that requirement. For a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), there is no ambiguity and $Y_q=d\psi_{\psi^{-1}(q)}X_{\psi^{-1}(q)}$. For example, $\psi(x)=x^2$ on $\mathbb R$ and $X=\partial_x$ give $2x\partial_y$, with opposite nonzero values at the two preimages of $y>0$. Thus the source's notation must be read with this qualification.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

On a branch where $(\rho,\phi)$ are valid [local coordinates](../../../complex-analysis.md#local-coordinate), the [inclusion map](../../../topology.md#inclusion-map) is $j(\rho,\phi)=(x(\rho),\rho\cos\phi,\rho\sin\phi)$, with $x^2=1-a^2\rho^2$. Its [differential](../../../differential-geometry.md#differential-of-a-smooth-map) gives

$$
\boxed{j_*\partial_\phi=-z\partial_y+y\partial_z=:K.}
$$

Strictly this is first a [vector field along a map](../../../fiber-bundle.md#vector-field-along-a-map) on the surface. The displayed formula extends it canonically to a [smooth](../../../analysis.md#smooth-function) [vector field](../../../calculus.md#vector-field) on all of $\mathbb R^3$. Its [integral curves of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) through $(x_0,y_0,z_0)$ obey $\dot x=0$, $\dot y=-z$, $\dot z=y$, hence

$$
\boxed{x(s)=x_0,\qquad y(s)+iz(s)=(y_0+iz_0)e^{is}.}
$$

These are circles around the $x$-axis, traversed with angular speed one; points on the axis are stationary. Since $K(x^2+a^2(y^2+z^2))=0$, curves starting on the ellipsoid stay there. The local angular chart can expire while the ambient [flow map](../../../dynamical-systems.md#flow-map) and the geometric curve remain well defined.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [induced metric](../../../riemannian-geometry.md#induced-metric) is obtained from the ambient [Euclidean metric](../../../differential-geometry.md#euclidean-metric) by the [pullback of a Riemannian metric](../../../differential-geometry.md#pullback-of-a-riemannian-metric) operation. Differentiating $x^2+a^2\rho^2=1$ on a branch with $x\ne0$ gives $dx=-a^2\rho\,d\rho/x$. Also $dy^2+dz^2=d\rho^2+\rho^2d\phi^2$. Consequently

$$
\boxed{g=E(\rho)d\rho^2+\rho^2d\phi^2,\qquad E(\rho)=1+\frac{a^4\rho^2}{1-a^2\rho^2}=\frac{1+a^2(a^2-1)\rho^2}{1-a^2\rho^2}.}
$$

The assumption that $(\rho,\phi)$ are coordinates already excludes the equator $x=0$ as well as the poles $\rho=0$. On such a chart, $0<\rho<1/|a|$ and $E>0$.

The [conformal flattening of a surface of revolution](../../../differential-geometry.md#conformal-flattening-of-a-surface-of-revolution) supplies the particularly simple [conformal factor](../../../general-relativity.md#conformal-factor)

$$
\boxed{\Omega=\rho^{-1},\qquad \Omega^2g=\frac{E(\rho)}{\rho^2}d\rho^2+d\phi^2=d\sigma^2+d\phi^2,\quad \sigma(\rho)=\int_{\rho_*}^{\rho}\frac{\sqrt{E(r)}}r\,dr.}
$$

Since $\sigma'>0$, these are [isothermal coordinates](../../../differential-geometry.md#isothermal-coordinates) with a flat rescaled metric. An angular coordinate is understood on a local branch; the flat metric may equally be viewed locally as a cylinder metric. The apparent divergence of $E$ at the equator is a coordinate failure, not a singularity of the [induced metric](../../../riemannian-geometry.md#induced-metric). For example, $(x,\phi)$ give $g=[1+x^2/(a^2(1-x^2))]dx^2+(1-x^2)d\phi^2/a^2$, regular at $x=0$.

## 2

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a timelike tangent $v=dx/du$, put $L=\sqrt{-g(v,v)}>0$ and $\mathscr L=L^2/2=-g(v,v)/2$, and use the [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation). For the quadratic [geodesic Lagrangian](../../../riemannian-geometry.md#geodesic-lagrangian), they reduce to

$$
\frac d{du}(g_{\mu\nu}v^\nu)-\frac12\partial_\mu g_{\alpha\beta}v^\alpha v^\beta=0,
\qquad \nabla_vv=0.
$$

Here the first equation has been multiplied by an irrelevant minus sign. For the length Lagrangian, its derivatives are $L^{-1}$ times those of $\mathscr L$, and differentiating that factor yields instead

$$
\boxed{\nabla_vv=\frac{\dot L}{L}\,v.}
$$

This is the [unparametrized geodesic equation](../../../riemannian-geometry.md#unparametrized-geodesic-equation), the key to why [timelike length and energy have the same geodesic images](../../../riemannian-geometry.md#timelike-length-and-energy-have-the-same-geodesic-images). Define [proper time](../../../special-relativity.md#proper-time) locally by $d\tau/du=L>0$ and put $w=dx/d\tau=v/L$. The product rule then gives $\nabla_ww=L^{-2}[\nabla_vv-(\dot L/L)v]=0$ and $g(w,w)=-1$. Conversely an affinely parametrized timelike [geodesic](../../../riemannian-geometry.md#geodesic) has constant $L$, by [metric compatibility](../../../fiber-bundle.md#metric-compatibility), and therefore satisfies both equations.

Thus **the two variational problems have the same oriented timelike geodesic images, after reparametrization**. They do not have exactly the same parametrized solutions with an arbitrary fixed $u$: in [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime), $t(u)=u^2$, $\mathbf x=0$, $u>0$, satisfies the length equation but not the quadratic equation. The timelike assumption excludes $L=0$, where this argument and the length derivative would fail.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use spatial indices $i,j=1,2,3$, set $\phi_i=\partial_i\phi$, and assume $\phi$ is smooth. The [inverse metric](../../../general-relativity.md#inverse-metric) has $g^{tt}=-c^{-2}e^{-2\phi/c^2}$ and $g^{ij}=\delta^{ij}$. The [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) follow from $\Gamma^\alpha{}_{\beta\gamma}=g^{\alpha\delta}(\partial_\beta g_{\gamma\delta}+\partial_\gamma g_{\beta\delta}-\partial_\delta g_{\beta\gamma})/2$:

$$
\boxed{\Gamma^t{}_{ti}=\Gamma^t{}_{it}=\frac{\phi_i}{c^2},\qquad \Gamma^i{}_{tt}=e^{2\phi/c^2}\phi_i.}
$$

All other components vanish. Although $g_{tt}=-c^2-2\phi+O(c^{-2})$ diverges, its [affine connection](../../../fiber-bundle.md#affine-connection) has a smooth limit on compact subsets:

$$
\boxed{\Gamma^{(\infty)i}{}_{tt}=\phi_i,\qquad \text{all other limiting components}=0.}
$$

This is the [Newtonian connection from an exponential lapse](../../../general-relativity.md#newtonian-connection-from-an-exponential-lapse). It is [torsion-free](../../../fiber-bundle.md#torsion-free-connection), and its [geodesic equation](../../../riemannian-geometry.md#geodesic-equation), using $t$ as an [affine parameter](../../../riemannian-geometry.md#affine-parameter) when $\dot t\ne0$, is $d^2x^i/dt^2=-\partial_i\phi$. Thus $\phi$ has the role of a [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential). There is no finite limiting nondegenerate [Lorentzian metric](../../../general-relativity.md#lorentzian-metric) in these fixed coordinates; $-g(c)/c^2$ tends to $dt^2$, a rank-one tensor. The limiting connection preserves $dt$ and the contravariant spatial tensor with components $h^{ij}=\delta^{ij}$, $h^{t\mu}=0$, which describe the degenerate temporal/spatial structures of this limit.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Fix the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) convention

$$
R^\alpha{}_{\beta\mu\nu}=\partial_\mu\Gamma^\alpha{}_{\nu\beta}-\partial_\nu\Gamma^\alpha{}_{\mu\beta}+\Gamma^\alpha{}_{\mu\lambda}\Gamma^\lambda{}_{\nu\beta}-\Gamma^\alpha{}_{\nu\lambda}\Gamma^\lambda{}_{\mu\beta},\qquad R_{\beta\nu}=R^\alpha{}_{\beta\alpha\nu}.
$$

For the limiting [affine connection](../../../fiber-bundle.md#affine-connection), every product of two nonzero connection coefficients is zero, because its only nonzero coefficients have spatial upper index and both lower indices $t$. Its only possibly nonzero [curvature](../../../differential-geometry.md#curvature) components, apart from antisymmetry in the last two indices, are

$$
R^i{}_{tjt}=\partial_j\partial_i\phi.
$$

The [Ricci tensor](../../../general-relativity.md#ricci-tensor) is therefore

$$
\boxed{\operatorname{Ric}(\nabla^{(\infty)})=(\Delta\phi)\,dt\otimes dt.}
$$

All other components vanish, so the limiting connection is a connection with vanishing [Ricci tensor](../../../general-relativity.md#ricci-tensor) exactly when $\phi$ satisfies the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) on spatial [Euclidean space](../../../functional-analysis.md#euclidean-norm). This is Ricci-flatness, not necessarily vanishing curvature: $\phi=x^2-y^2$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) but has nonzero [Hessian matrix](../../../calculus.md#hessian-matrix) and hence a nonflat limiting connection. Reversing the curvature sign convention reverses the displayed Ricci sign but leaves the equivalence unchanged.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Use $x^0=t$ and the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) $\epsilon^1{}_{23}=1$. Define a smooth [affine connection](../../../fiber-bundle.md#affine-connection) by

$$
\boxed{\Gamma^i{}_{00}=-E^i,\qquad \Gamma^i{}_{0j}=\Gamma^i{}_{j0}=\epsilon^i{}_{jk}B^k,\qquad \Gamma^0{}_{ab}=\Gamma^i{}_{jk}=0.}
$$

The lower indices are symmetric, so it is a [torsion-free connection](../../../fiber-bundle.md#torsion-free-connection). With $t$ itself as parameter, the time component of the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) is identically satisfied, while its spatial components become

$$
\ddot x^i=-\Gamma^i{}_{00}-2\Gamma^i{}_{0j}\dot x^j=E^i+2\epsilon^i{}_{kj}B^k\dot x^j.
$$

The last term is $2(\mathbf B\times\dot{\mathbf x})^i$, with the wedge in the source interpreted as the three-dimensional [cross product](../../../vector-space.md#cross-product). Thus the spacetime lifts $(t,\mathbf x(t))$ are actually affinely parametrized [geodesics](../../../riemannian-geometry.md#geodesic), which proves the requested unparametrized claim. Conversely a geodesic with nonzero constant $dt/ds$ can be parametrized by $t$ and obeys this particle equation; purely spatial geodesics with $dt/ds=0$ are not such trajectories. No field equations or metric compatibility are needed. This construction is the [affine connection for a velocity-linear force](../../../fiber-bundle.md#affine-connection-for-a-velocity-linear-force).

## 3

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a [smooth](../../../analysis.md#smooth-function) [vector field](../../../calculus.md#vector-field) $X$, solve the initial-value problem $d\phi_t(p)/dt=X(\phi_t(p))$, $\phi_0(p)=p$. Local existence, uniqueness and smooth dependence for [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation) give a [local flow](../../../differential-geometry.md#local-flow). Uniqueness yields $\phi_{t+s}(p)=\phi_t(\phi_s(p))$ whenever both sides are defined, and $\phi_{-t}$ is the inverse of $\phi_t$ on the corresponding domains. Thus each local flow map is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) between open subsets.

**A group of diffeomorphisms of the entire manifold for every real $t$ requires a [complete vector field](../../../differential-geometry.md#complete-vector-field).** This follows, for example, on a [compact](../../../topology.md#compact-space) manifold without boundary: local existence times can be made uniform on a finite cover, and repeated continuation prevents finite-time escape. Without completeness, the source's group is only local. The vector field $x^2\partial_x$ on $\mathbb R$ has flow $x\mapsto x/(1-tx)$ and blows up at $t=1/x$ for $x>0$, so smoothness alone cannot imply a global one-parameter group.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Define the [Lie derivative of a differential form](../../../differential-form.md#lie-derivative-of-a-differential-form) by $\mathcal L_X\alpha=(d/dt)_{t=0}\phi_t^*\alpha$, using the [local flow](../../../differential-geometry.md#local-flow). The [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) respects the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms) and commutes with the [exterior derivative](../../../differential-form.md#exterior-derivative). Therefore $\mathcal L_X$ is a [derivation of an algebra](../../../associative-algebra.md#derivation-of-an-algebra) of degree zero and commutes with $d$.

Let $D_X=\iota_Xd+d\iota_X$, where $\iota_X$ is the [interior product of a differential form](../../../differential-form.md#interior-product). The graded product rules for $d$ and $\iota_X$ show that their anticommutator $D_X$ is also a degree-zero [derivation of an algebra](../../../associative-algebra.md#derivation-of-an-algebra): the two mixed terms cancel. Since $d^2=0$, it commutes with $d$. On a function $f$, $\iota_Xf=0$ and $D_Xf=\iota_Xdf=Xf=\mathcal L_Xf$. Hence $D_X(df)=d(Xf)=\mathcal L_X(df)$.

In a [manifold chart](../../../differential-geometry.md#manifold-chart), every [differential form](../../../differential-form.md) is a sum of functions times products $dx^{i_1}\wedge\cdots\wedge dx^{i_p}$. The two derivations agree on its generators $f$ and $dx^i$, and therefore agree on every such form. This proves [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula), including the case $p=0$:

$$
\boxed{\mathcal L_X\alpha=\iota_Xd\alpha+d(\iota_X\alpha).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Use [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula). The [exterior derivative](../../../differential-form.md#exterior-derivative) and [interior product of a differential form](../../../differential-form.md#interior-product) give

$$
d\alpha=-2\,dx\wedge dy,\qquad \iota_X\alpha=-x^2-y^2+z^2,\qquad \iota_Xd\alpha=2x\,dx+2y\,dy.
$$

Thus $d(\iota_X\alpha)=-2x\,dx-2y\,dy+2z\,dz$, and the first two components cancel:

$$
\boxed{\mathcal L_X\alpha=2z\,dz.}
$$

The rotation in the $xy$-plane leaves $y\,dx-x\,dy$ invariant, while the dilation in $z$ doubles the infinitesimal weight of $z\,dz$, providing a geometric check of this [Lie derivative](../../../differential-form.md#lie-derivative-of-a-differential-form).

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

Integrating the two [vector fields](../../../calculus.md#vector-field) gives their complete [flow maps](../../../dynamical-systems.md#flow-map):

$$
\boxed{\phi_t(x,y,z)=(x\cos t-y\sin t,\ x\sin t+y\cos t,\ e^t z),\qquad \psi_t(x,y,z)=(e^t x,e^t y,e^t z).}
$$

The first is a simultaneous [rotation about the z-axis](../../../quantum-circuit.md#rotation-about-the-z-axis) through angle $t$ and a dilation by $e^t$ in the $z$-direction. The second is an isotropic dilation about the origin. Both satisfy the group law for all real $t$ and have inverse given by time $-t$. In particular $\phi_t$ is not a pure rotation unless restricted to the plane $z=0$.

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

The [Jacobian determinant](../../../calculus.md#jacobian-determinant) of $\phi_t$ is $e^t$, while every coordinate and every coordinate differential is multiplied by $e^t$ under $\psi_t$. Hence the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) operation gives

$$
\boxed{\phi_t^*\mu=e^t\mu,\qquad \psi_t^*\alpha=e^{2t}\alpha,\qquad \mathcal L_X\mu=\mu,\qquad \mathcal L_Y\alpha=2\alpha.}
$$

To compare directly with [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula), note $d\mu=0$ and compute

$$
\iota_X\mu=-y\,dy\wedge dz-x\,dx\wedge dz+z\,dx\wedge dy,\qquad d(\iota_X\mu)=\mu.
$$

The first two differentiated terms vanish because their coordinate differentials repeat; the last contributes $dz\wedge dx\wedge dy=\mu$. Also

$$
\iota_Y\alpha=z^2,\qquad \iota_Yd\alpha=2y\,dx-2x\,dy,\qquad d(\iota_Y\alpha)=2z\,dz.
$$

Their sum is $2\alpha$, as required. Equivalently the [divergence](../../../calculus.md#divergence) of $X$ relative to the standard [volume form](../../../differential-form.md#volume-form) is one.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

An [electromagnetic field tensor](../../../electromagnetism.md#electromagnetic-field-tensor) obeys the homogeneous [Maxwell equations](../../../electromagnetism.md#maxwell-equations) $dF=0$. Together with its invariance under the [Killing vector field](../../../general-relativity.md#killing-vector-field) $V$, [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) gives $d(\iota_VF)=\mathcal L_VF-\iota_VdF=0$. The [local potential of a closed differential one-form](../../../differential-form.md#local-potential-of-a-closed-differential-one-form) construction, the one-form [Poincaré lemma](../../../differential-form.md#poincare-lemma), therefore supplies a [scalar field](../../../quantum-field-theory.md#scalar-field) $\Phi$ on a sufficiently small [contractible](../../../algebraic-topology.md#contractible-space) neighborhood with

$$
\boxed{\iota_VF=d\Phi.}
$$

For an explicit local proof, write $\iota_VF=\alpha_i(x)dx^i$ on a coordinate ball centered at zero and take $\Phi(x)=\int_0^1 x^i\alpha_i(sx)\,ds$. Since $d\alpha=0$, differentiating under the integral gives $\partial_j\Phi=\int_0^1[\alpha_j(sx)+s x^i\partial_i\alpha_j(sx)]ds=\alpha_j(x)$. There need not be a global potential when this closed one-form has nonzero periods. The homogeneous Maxwell equation is essential; an arbitrary invariant two-form would not suffice.

Use [proper time](../../../special-relativity.md#proper-time) for the massive particle, let $u$ be its tangent, and assume $m\ne0$. The [Killing equation](../../../general-relativity.md#killing-equation) makes $u^au^b\nabla_aV_b=0$. The [Lorentz force](../../../electromagnetism.md#lorentz-force) equation then implies

$$
\frac d{d\tau}(V_au^a)=\frac qm V_aF^a{}_bu^b=\frac qm V^aF_{ab}u^b=\frac qm\frac{d\Phi}{d\tau}.
$$

Consequently the local conserved quantity is

$$
\boxed{mV_au^a-q\Phi=\text{constant}.}
$$

The sign follows from contracting $F$ in its first argument, exactly as in the source. Adding a constant to $\Phi$ merely shifts the conserved quantity. This is a [charged-particle conserved quantity from a Killing symmetry](../../../general-relativity.md#charged-particle-conserved-quantity-from-a-killing-symmetry).

## 4

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Choose signature $(-,+,+,+)$, with $e^0$ timelike. The [orthonormal coframe in spacetime](../../../general-relativity.md#orthonormal-coframe-in-spacetime) reconstructs the [Lorentzian metric](../../../general-relativity.md#lorentzian-metric) as

$$
\boxed{g=-(e^0)^2+(e^1)^2+(e^2)^2+(e^3)^2=-dt^2+A(t-z)^2dx^2+B(t-z)^2dy^2+dz^2.}
$$

Because $A$ and $B$ are nowhere zero on the domain, the coframe is invertible and the metric nondegenerate; either sign of each function is allowed. In [retarded and advanced null coordinates](../../../special-relativity.md#retarded-and-advanced-null-coordinates) $u=t-z$, $v=t+z$ the metric is $-du\,dv+A(u)^2dx^2+B(u)^2dy^2$, a diagonal example of [Rosen coordinates for a plane gravitational wave](../../../general-relativity.md#rosen-coordinates-for-a-plane-gravitational-wave). Multiplication by $-1$ would give the opposite overall signature convention; all subsequent signs here use the displayed one.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Put $u=t-z$, $\ell=du=e^0-e^3$, $p=A'/A$, $q=B'/B$, with primes denoting $d/du$. The [exterior derivatives](../../../differential-form.md#exterior-derivative) are $de^0=de^3=0$, $de^1=p\ell\wedge e^1$, $de^2=q\ell\wedge e^2$. For a [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection), the [connection 1-forms](../../../connection-1-form.md) obey both [Cartan's first structure equation](../../../connection-1-form.md#cartan-s-first-structure-equation) and [metric compatibility](../../../fiber-bundle.md#metric-compatibility). With lower indices $\omega_{ab}=\eta_{ac}\omega^c{}_b$, the result is

$$
\boxed{\omega_{01}=\omega_{13}=-p\,e^1,\qquad \omega_{02}=\omega_{23}=-q\,e^2,\qquad \alpha=\beta=-\frac{A'}A,\quad \gamma=\delta=-\frac{B'}B.}
$$

All other lower-index forms vanish or follow from $\omega_{ab}=-\omega_{ba}$. Raising the first time index changes its sign: for example $\omega^0{}_1=\omega^1{}_0=p e^1$, whereas $\omega^1{}_3=-p e^1$ and $\omega^3{}_1=p e^1$.

For direct verification, $\omega^1{}_0\wedge e^0+\omega^1{}_3\wedge e^3=-p\ell\wedge e^1=-de^1$, and the same holds for index two. For indices zero and three each term wedges $e^1$ or $e^2$ with itself, so it is zero. These forms are metric-compatible, and uniqueness follows from the [existence and uniqueness of the Levi-Civita connection](../../../fiber-bundle.md#existence-and-uniqueness-of-the-levi-civita-connection). The printed uniqueness statement implicitly includes metric compatibility: the torsion equation alone permits adding nonzero forms $C^a{}_{bc}e^c$ with $C^a{}_{bc}=C^a{}_{cb}$, since their wedge with $e^b$ vanishes.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Keep $\ell=e^0-e^3$ and set $P=p'+p^2=A''/A$, $Q=q'+q^2=B''/B$. Differentiation gives $d(p e^1)=P\ell\wedge e^1$ and $d(q e^2)=Q\ell\wedge e^2$. In [Cartan's second structure equation](../../../connection-1-form.md#cartan-s-second-structure-equation), the quadratic terms for these components vanish. The apparently possible transverse component cancels:

$$
\omega^1{}_0\wedge\omega^0{}_2+\omega^1{}_3\wedge\omega^3{}_2=pq\,e^1\wedge e^2-pq\,e^1\wedge e^2=0.
$$

Thus the potentially nonzero mixed-index [curvature 2-forms](../../../connection-1-form.md#curvature-2-form) are

$$
\boxed{\begin{aligned}
\Theta^0{}_1=\Theta^1{}_0=\Theta^3{}_1&=P\ell\wedge e^1,&\Theta^1{}_3&=-P\ell\wedge e^1,\\
\Theta^0{}_2=\Theta^2{}_0=\Theta^3{}_2&=Q\ell\wedge e^2,&\Theta^2{}_3&=-Q\ell\wedge e^2.
\end{aligned}}
$$

All other components vanish. Equivalently, the independent lower-index forms are $\Theta_{01}=\Theta_{13}=-P\ell\wedge e^1$ and $\Theta_{02}=\Theta_{23}=-Q\ell\wedge e^2$, with the rest supplied by lower-index antisymmetry. These signs use $\Theta^a{}_b=\tfrac12R^a{}_{bcd}e^c\wedge e^d$ and the curvature convention in question 2(c). This is the [curvature of a diagonal plane wave in Rosen coordinates](../../../general-relativity.md#curvature-of-a-diagonal-plane-wave-in-rosen-coordinates).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $E_a$ denote the frame dual to the coframe. For the convention just stated, the [Ricci tensor](../../../general-relativity.md#ricci-tensor) is obtained from the [curvature 2-forms](../../../connection-1-form.md#curvature-2-form) through the Ricci one-forms $\mathcal R_b=\sum_a\iota_{E_a}\Theta^a{}_b=R_{bd}e^d$. In particular $\iota_{E_1}(\ell\wedge e^1)=-\ell$ and likewise for index two. It follows that

$$
\mathcal R_0=-(P+Q)\ell,\qquad \mathcal R_3=(P+Q)\ell,\qquad \mathcal R_1=\mathcal R_2=0.
$$

Thus

$$
\boxed{\operatorname{Ric}=-(P+Q)\,du\otimes du,\qquad R_{tt}=R_{zz}=-(P+Q),\quad R_{tz}=R_{zt}=P+Q.}
$$

The [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) vanishes even before imposing vacuum because $du$ is null, but the full tensor vanishes exactly when

$$
\boxed{\frac{A''}{A}+\frac{B''}{B}=0.}
$$

This is the [Vacuum Einstein equations](../../../general-relativity.md#vacuum-einstein-equations) in this family. The nonzero-coframe hypothesis makes division by $A$ and $B$ legitimate. A nonzero $P=-Q$ can leave the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) nonzero even in vacuum.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Use [linearization](../../../algebra.md#linearization) around [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) after constant rescaling of $x,y$: set $A=1+\varepsilon a(u)$, $B=1+\varepsilon b(u)$, $u=t-z$. To first order,

$$
g=\eta+2\varepsilon a(u)\,dx^2+2\varepsilon b(u)\,dy^2+O(\varepsilon^2),\qquad a''+b''=0.
$$

Hence $s=a+b$ is affine in $u$, while $h=a-b$ is the freely propagating profile. The [affine transverse trace in a diagonal linearized plane wave is pure gauge](../../../general-relativity.md#affine-transverse-trace-in-a-diagonal-linearized-plane-wave-is-pure-gauge): it has zero linearized curvature and is locally a coordinate artifact. To see this without imposing extra boundary conditions, use a first-order [linearized coordinate gauge transformation](../../../general-relativity.md#linearized-coordinate-gauge-transformation) $h_{\mu\nu}\mapsto h_{\mu\nu}-\partial_\mu\xi_\nu-\partial_\nu\xi_\mu$, with

$$
\xi_x=\frac{\varepsilon s x}{2},\quad \xi_y=\frac{\varepsilon s y}{2},\quad \xi_t=-\frac{\varepsilon s'(x^2+y^2)}4,\quad \xi_z=\frac{\varepsilon s'(x^2+y^2)}4.
$$

The $tx,ty,zx,zy$ changes cancel and the remaining time/longitudinal changes are proportional to $s''=0$. The transverse perturbation becomes

$$
\boxed{h_{xx}=\varepsilon h(t-z),\qquad h_{yy}=-\varepsilon h(t-z),\qquad h_{xy}=0,}
$$

with all time and longitudinal components zero. It is a [transverse-traceless gauge](../../../general-relativity.md#transverse-traceless-gauge) plane [gravitational wave](../../../general-relativity.md#gravitational-wave) travelling in the positive $z$-direction, with [plus polarization](../../../general-relativity.md#plus-polarization) and no [cross polarization](../../../general-relativity.md#cross-polarization) in these transverse axes.

For freely falling nearby particles, [geodesic deviation](../../../general-relativity.md#geodesic-deviation) gives opposite transverse tidal accelerations, since $R_{txtx}=-\varepsilon a''$ and $R_{tyty}=-\varepsilon b''=+\varepsilon a''$ in vacuum. Thus the transverse [geodesic deviation](../../../general-relativity.md#geodesic-deviation) [eigenvalues](../../../linear-operator-theory.md#eigenvalue) have opposite signs; the stretching and compressing roles interchange when the [curvature](../../../differential-geometry.md#curvature) profile changes sign. If $h''=0$ as well, there is no linearized tidal wave: that special profile is also locally flat to this order. The exact diagonal metric describes a fixed transverse polarization through its opposite vacuum curvature eigenvalues; the linearized calculation identifies it as plus relative to the chosen axes.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
