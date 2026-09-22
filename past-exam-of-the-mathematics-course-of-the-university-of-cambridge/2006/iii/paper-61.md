# Paper 61

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper61.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper61.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 61](paper-61.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the paper's curvature convention throughout, and define the [Ricci tensor](../../../general-relativity.md#ricci-tensor) and [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) by $R_{kn}=R^i{}_{kin}$ and $R=g^{kn}R_{kn}$. In particular, if semicolons are read from left to right, $X^i{}_{;km}=\nabla_m(\nabla_kX)^i$, including the connection on the derivative index. This ordering matters for the [Ricci identity](../../../general-relativity.md#curvature-commutator-on-a-covariant-tensor) sign.

Choose [Riemann normal coordinates](../../../general-relativity.md#normal-coordinates) at an arbitrary point $P$. The [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) vanish there, and the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) formula gives

$$
R_{ikmn}(P)=\frac12\left(g_{im,kn}+g_{kn,im}-g_{km,in}-g_{in,km}\right)(P).
$$

Metric symmetry and commuting partial derivatives show directly that exchanging $m,n$ or $i,k$ changes the sign, while interchanging the pairs $(i,k)$ and $(m,n)$ leaves the expression unchanged. Adding its three cyclic versions over $k,m,n$ cancels every second derivative. These are tensorial statements and $P$ was arbitrary, so

$$
\boxed{R^i{}_{k(mn)}=0,\qquad R^i{}_{[kmn]}=0,\qquad R_{(ik)mn}=0,\qquad R_{ikmn}=R_{mnik}.}
$$

The cyclic relation is the [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity); its reduction to the total antisymmetrization uses last-pair antisymmetry. These arguments use zero [torsion tensor](../../../fiber-bundle.md#torsion-tensor) and [metric compatibility](../../../fiber-bundle.md#metric-compatibility), not a field equation.

At $P$, the [covariant derivative](../../../general-relativity.md#covariant-derivative) of curvature equals its partial derivative. Differentiating the connection expression for curvature gives derivatives of $\partial_n\Gamma^i{}_{km}-\partial_m\Gamma^i{}_{kn}$; derivatives of the quadratic connection terms vanish because $\Gamma(P)=0$. In the cyclic sum over $m,n,p$, every second derivative of a connection coefficient occurs twice with opposite signs. Thus

$$
R^i{}_{kmn;p}+R^i{}_{knp;m}+R^i{}_{kpm;n}=0,
\qquad\boxed{R^i{}_{k[mn;p]}=0.}
$$

This is the [second Bianchi identity](../../../general-relativity.md#second-bianchi-identity), valid everywhere by tensoriality.

Lower the first curvature index and contract the differential identity with $g^{im}$. [Metric compatibility](../../../fiber-bundle.md#metric-compatibility) allows the metric to pass through the [covariant derivatives](../../../general-relativity.md#covariant-derivative). Using the pair antisymmetries yields

$$
\boxed{\nabla^iR_{ikmn}=\nabla_mR_{kn}-\nabla_nR_{km}.}
$$

Contract again with $g^{km}$. The left side is $-\nabla^iR_{in}$, while the right side is $\nabla^kR_{kn}-\nabla_nR$. Hence the [contracted Bianchi identity](../../../general-relativity.md#contracted-bianchi-identity) is

$$
\boxed{\nabla^iR_{in}=\frac12\nabla_nR,\qquad
\nabla^i\left(R_{in}-\frac12g_{in}R\right)=0.}
$$

The [Ricci tensor](../../../general-relativity.md#ricci-tensor) is symmetric, as follows by contracting the pair-exchange symmetry. The final divergence is that of the [Einstein tensor](../../../general-relativity.md#einstein-tensor).

For the vector commutator, at the same normal-coordinate point,

$$
X^i{}_{;km}=\partial_m\partial_kX^i+(\partial_m\Gamma^i{}_{jk})X^j.
$$

The terms involving undifferentiated connection coefficients vanish at $P$. Subtracting the reversed expression leaves $(\Gamma^i{}_{jk,m}-\Gamma^i{}_{jm,k})X^j$, exactly the stated curvature convention at $P$. Therefore

$$
\boxed{X^i{}_{;km}-X^i{}_{;mk}=R^i{}_{jkm}X^j.}
$$

For a [covector field](../../../differential-form.md#one-form), its connection term has the opposite sign: $\omega_{i;k}=\partial_k\omega_i-\Gamma^j{}_{ik}\omega_j$. The same calculation gives

$$
\boxed{\omega_{i;km}-\omega_{i;mk}=-R^j{}_{ikm}\omega_j.}
$$

Equivalently, apply the commutator to the scalar $\omega_iX^i$, whose two [covariant derivatives](../../../general-relativity.md#covariant-derivative) commute, and cancel the vector contribution. Each covariant index contributes a negative curvature action and each contravariant index a positive one in this semicolon ordering.

To prove the requested [double divergence of the Riemann tensor](../../../general-relativity.md#double-divergence-of-the-riemann-tensor), let

$$
D_{mn}=R^{ik}{}_{mn;ik}=\nabla_k\nabla_iR^{ik}{}_{mn}.
$$

The once-contracted identity gives

$$
D_{mn}=\nabla_k\nabla_mR^k{}_n-\nabla_k\nabla_nR^k{}_m.
$$

Commuting the outer derivative past $\nabla_m$ and $\nabla_n$ leaves a difference of scalar Hessians, $\tfrac12(\nabla_m\nabla_n-\nabla_n\nabla_m)R=0$, plus curvature terms. The operator commutator $[\nabla_k,\nabla_m]$ has the negative of the paper's curvature sign, since it reverses the semicolon order. On the mixed [Ricci tensor](../../../general-relativity.md#ricci-tensor) it gives

$$
[\nabla_k,\nabla_m]R^k{}_n
=-R_{am}R^a{}_n+R^a{}_{nkm}R^k{}_a.
$$

The first term is symmetric in $m,n$: it is the metric contraction of two symmetric [Ricci tensors](../../../general-relativity.md#ricci-tensor). The second is $S_{mn}=R^{ak}R_{ankm}$ and is also symmetric, since

$$
S_{mn}=R^{ak}R_{kman}=R^{ak}R_{amkn}=S_{nm},
$$

where the first equality uses curvature pair exchange and the second swaps the dummy indices $a,k$. Thus the two commutator terms cancel on antisymmetrization in $m,n$, proving

$$
\boxed{R^{ik}{}_{mn;ik}=0.}
$$

No assumption such as vacuum, constant curvature or vanishing [Ricci tensor](../../../general-relativity.md#ricci-tensor) was used.

## 2

↑ **Parent:** [Paper 61](paper-61.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use units $c=1$ and signature $(+---)$. For a massive [test particle](../../../classical-mechanics.md#test-particle), write its [four-momentum](../../../special-relativity.md#four-momentum) as $p^i=mu^i$, where $u^i=dx^i/d\tau$, $\tau$ is Minkowski [proper time](../../../special-relativity.md#proper-time), and $u^iu_i=1$. The stated [flat-background scalar-force theory of gravity](../../../general-relativity.md#flat-background-scalar-force-theory-of-gravity) then gives

$$
\frac{dp^i}{d\tau}=m\left(\partial^i\Phi-u^i u^j\partial_j\Phi\right).
$$

Contract with $p_i=mu_i$. The two terms cancel:

$$
\frac{d(m^2)}{d\tau}=2p_i\frac{dp^i}{d\tau}
=2m^2\left(u^j\partial_j\Phi-u^iu_i u^j\partial_j\Phi\right)=0.
$$

Thus [rest mass](../../../special-relativity.md#invariant-mass) is conserved and the [acceleration](../../../classical-mechanics.md#acceleration) law is

$$
\boxed{\frac{du^i}{d\tau}=\partial^i\Phi-u^i(u\cdot\partial\Phi).}
$$

There is no mass or composition parameter in this equation. Particles released at the same event with the same [velocity](../../../classical-mechanics.md#velocity) consequently have identical trajectories. In a static weak field at small speed, its spatial part becomes $d^2\mathbf x/dt^2=-\boldsymbol\nabla\Phi$, since raising a spatial index introduces a minus sign. The field equation likewise reduces to $\nabla^2\Phi=4\pi G\rho$ for nonrelativistic matter, because $T^i{}_i\simeq\rho$ and $\Box=-\nabla^2$ in the static limit.

Therefore **yes: the model agrees with the Eötvös test of universal free fall**. In the point-particle/test-body approximation, inertial and passive gravitational masses have the same universal ratio. This is the [weak equivalence principle](../../../general-relativity.md#weak-equivalence-principle) tested by the [Eötvös experiment](../../../general-relativity.md#eotvos-experiment); it is not a claim about strongly self-gravitating bodies or a proof of all aspects of the [Einstein equivalence principle](../../../general-relativity.md#einstein-equivalence-principle).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a [photon](../../../quantum-mechanics.md#photon), $p^ip_i=0$ and the null displacement along the ray is parallel to $p^i$. Consequently $p_jdx^j=0$, and the first term of the momentum law vanishes. Write $dx^i=p^i d\lambda$ with an appropriate path parameter. Then

$$
dp^i=-(p^j\partial_j\Phi)p^i d\lambda=-p^i d\Phi,
\qquad\boxed{d(e^\Phi p^i)=0.}
$$

For a static potential, a [photon](../../../quantum-mechanics.md#photon) emitted and received by laboratories at rest in the background frame has [energy](../../../classical-mechanics.md#energy) proportional to $p^0$. Using $E=h_{\rm P}\nu$, the [scalar-force gravitational redshift](../../../general-relativity.md#scalar-force-gravitational-redshift) is

$$
\boxed{\frac{\nu_r}{\nu_e}=e^{\Phi_e-\Phi_r}
=1-(\Phi_r-\Phi_e)+O((\Delta\Phi)^2).}
$$

Restoring $c$, the leading fractional shift is $\Delta\nu/\nu=-\Delta\Phi_N/c^2$, where $\Phi_N$ is the dimensional [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential). Near Earth's surface, an upward displacement $H$ has $\Delta\Phi_N=gH>0$, hence $\Delta\nu/\nu=-gH/c^2$: the receiver sees a redshift.

Thus **yes: the predicted weak-field [frequency](../../../physics.md#frequency) shift agrees with the [Pound-Rebka experiment](../../../general-relativity.md#pound-rebka-experiment)**. The calculation concerns stationary emitter and receiver, with identical local transition-energy standards; it does not add a Doppler shift due to their relative motion. Agreement with this [gravitational redshift](../../../general-relativity.md#gravitational-redshift) measurement alone does not establish the [tensor](../../../linear-algebra.md#tensor) theory of [general relativity](../../../general-relativity.md).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The null momentum equation gives $p^i=C^i e^{-\Phi}$, with a constant [null vector](../../../special-relativity.md#null-vector) $C^i$. Since the tangent is parallel to $p^i$, every spatial direction ratio is constant:

$$
\frac{dx^a}{dx^0}=\frac{p^a}{p^0}=\frac{C^a}{C^0},\qquad a=1,2,3.
$$

The changing potential changes the scale of the [four-momentum](../../../special-relativity.md#four-momentum), not its direction. [Photon](../../../quantum-mechanics.md#photon) paths are therefore straight lines in the background [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime), up to reparametrization. This is also consistent with [conformal preservation of null geodesic paths](../../../general-relativity.md#conformal-preservation-of-null-geodesic-paths): the particle motion law can be expressed through a conformally flat metric, which cannot change the unparametrized null trajectories of the background.

Hence **no: the theory predicts zero solar light deflection**, in disagreement with the observed nonzero bending of light. For comparison, the leading [Schwarzschild light deflection](../../../general-relativity.md#schwarzschild-light-deflection) is $4GM/(bc^2)$ at impact parameter $b$. The scalar theory's nonzero [gravitational redshift](../../../general-relativity.md#gravitational-redshift) does not rescue this failed directional prediction.

## 3

↑ **Parent:** [Paper 61](paper-61.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Raise perturbation indices with the background [Minkowski metric](../../../special-relativity.md#minkowski-metric). To first order, the inverse metric is $g^{ik}=\eta^{ik}-\epsilon h^{ik}+O(\epsilon^2)$ and the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) is

$$
\Gamma^i{}_{km}=\frac\epsilon2\eta^{ij}(h_{jk,m}+h_{jm,k}-h_{km,j})+O(\epsilon^2).
$$

Quadratic connection products in the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) are of order $\epsilon^2$. Substitution into the paper's curvature convention gives

$$
\boxed{R_{ikmn}=\frac\epsilon2(h_{im,kn}+h_{nk,im}-h_{mk,in}-h_{in,km})+O(\epsilon^2).}
$$

The signs follow the convention on the cover sheet; reversing the curvature definition would reverse this expression.

The gauge freedom is the freedom to identify points of the perturbed spacetime with points of the flat background in slightly different coordinates. Under the passive infinitesimal change $x'^i=x^i+\epsilon\xi^i(x)$, the metric transformation law gives the [linearized coordinate gauge transformation](../../../general-relativity.md#linearized-coordinate-gauge-transformation)

$$
h'_{ik}=h_{ik}-\partial_i\xi_k-\partial_k\xi_i.
$$

Thus a nonzero perturbation can partly represent a coordinate change rather than physical curvature. Substituting this variation into the displayed curvature formula gives

$$
\delta R_{ikmn}=-\frac\epsilon2\left(
\xi_{i,mkn}+\xi_{m,ikn}+\xi_{n,kim}+\xi_{k,nim}
-\xi_{m,kin}-\xi_{k,min}-\xi_{i,nkm}-\xi_{n,ikm}\right)=0.
$$

Each third derivative has a partner differing only by the order of its commuting partial derivatives. This explicitly proves [gauge invariance of the linearized Riemann tensor](../../../general-relativity.md#gauge-invariance-of-the-linearized-riemann-tensor). The restriction to first order matters: a coordinate change acts on nonzero background curvature as well, but the background here is flat.

Define the [trace-reversed metric perturbation](../../../general-relativity.md#trace-reversed-metric-perturbation) and [d'Alembert operator](../../../wave-equation.md#d-alembert-operator) by

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

up to $O(\epsilon^2)$. Consequently the [Einstein tensor](../../../general-relativity.md#einstein-tensor) is

$$
G_{ik}=\frac\epsilon2\left(\Box\bar h_{ik}
+\eta_{ik}\partial^a\partial^b\bar h_{ab}
-\partial_i\partial^a\bar h_{ak}-\partial_k\partial^a\bar h_{ai}\right).
$$

Choose [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity), $\partial^k\bar h_{ik}=0$. It can be imposed locally by solving $\Box\xi_i=\partial^k\bar h_{ik}$, since the gauge transformation changes this divergence by $-\Box\xi_i$. The remaining coordinate freedom satisfies $\Box\xi_i=0$. In this gauge,

$$
G_{ik}=\frac\epsilon2\Box\bar h_{ik},\qquad
\boxed{\Box\bar h_{ik}=-16\pi G\epsilon^{-1}T_{ik}.}
$$

This is the requested [Linearized Einstein equations](../../../general-relativity.md#linearized-einstein-equations) in the stated sign convention. Their divergence requires $\partial^kT_{ik}=0$ to this order.

For the [photon](../../../quantum-mechanics.md#photon) beam, introduce $u=t-x$ and the constant null covector $\ell_i=(1,-1,0,0)$, so $\ell^i=(1,1,0,0)$. The [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) is

$$
T_{ik}=\epsilon\rho(u)\ell_i\ell_k.
$$

It is trace-free and conserved: $\ell^i\partial_i\rho(u)=0$. A beam-adapted particular solution, with no independently added homogeneous gravitational field, is

$$
\bar h_{ik}=h_{ik}=H(u,y,z)\ell_i\ell_k.
$$

The equality follows because its trace is zero, and the Lorenz condition holds because $\ell^k\partial_kH=0$. The field equation becomes a transverse [Poisson equation](../../../partial-differential-equation.md#poisson-equation):

$$
\Box H=-\Delta_\perp H=-16\pi G\rho(u),\qquad
\boxed{\Delta_\perp H=16\pi G\rho(u).}
$$

For the transversely uniform source in the question, one particular solution is $H=4\pi G\rho(u)(y^2+z^2)$. Thus the sourced components can be chosen as

$$
\boxed{h_{00}=h_{11}=-h_{01}=-h_{10}=H,\qquad\text{all other components zero}.}
$$

Boundary conditions and homogeneous solutions determine additional freedom; the source does not uniquely specify every component in every gauge. In particular, taking $H$ to depend only on $t-x$ would give $\Box H=0$ and cannot solve the equation for nonzero $\rho$. The uniform idealization is not an asymptotically flat finite beam, and its quadratic particular solution is a weak-field description only where $|\epsilon H|\ll1$.

Finally consider another [photon](../../../quantum-mechanics.md#photon) with tangent proportional to $\ell^i$. Its tangent remains null because $h_{ik}\ell^i\ell^k=0$. Moreover $h_{ik}\ell^k=0$, and since $\ell$ is constant, the connection contraction is

$$
\Gamma^i{}_{jk}\ell^j\ell^k
=\frac\epsilon2\eta^{ia}\left(2\ell^j\partial_j(h_{ak}\ell^k)-\partial_a(h_{jk}\ell^j\ell^k)\right)=0.
$$

The [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) is therefore satisfied by a straight affinely parametrized ray along the beam. Hence **co-propagating [photons](../../../quantum-mechanics.md#photon) experience no deflection from the beam's gravitational field**. This is [parallel photon beams in linearized gravity](../../../general-relativity.md#parallel-photon-beams-in-linearized-gravity); it does not assert absence of forces on counter-propagating [photons](../../../quantum-mechanics.md#photon) or effects from unrelated homogeneous gravitational perturbations.

## 4

↑ **Parent:** [Paper 61](paper-61.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Take both curvature radii to be one. Coordinate ranges depend on the global identification, which a line element alone cannot fix. For the ordinary [two-dimensional de Sitter spacetime](../../../general-relativity.md#two-dimensional-de-sitter-spacetime),

$$
\boxed{t\in\mathbb R,\qquad\chi\in\mathbb R/(2\pi\mathbb Z).}
$$

This is the unit hyperboloid $X_0^2-X_1^2-X_2^2=-1$ in ambient signature $(+--)$, parametrized by $X_0=\sinh t$, $X_1=\cosh t\cos\chi$, $X_2=\cosh t\sin\chi$. Unwrapping $\chi$ instead gives its [universal cover](../../../algebraic-topology.md#universal-cover).

For [two-dimensional anti-de Sitter spacetime](../../../general-relativity.md#two-dimensional-anti-de-sitter-spacetime), the embedding $X_0^2+X_1^2-X_2^2=1$ in ambient signature $(++-)$ is parametrized by $X_0=\cosh r\cos t$, $X_1=\cosh r\sin t$, $X_2=\sinh r$. On this hyperboloid $r\in\mathbb R$ and $t$ is periodic modulo $2\pi$, creating closed timelike circles. The physically usual [universal cover](../../../algebraic-topology.md#universal-cover) removes that periodicity:

$$
\boxed{r\in\mathbb R,\qquad t\in\mathbb R\quad\text{on the covering AdS spacetime}.}
$$

Both signs of $r$ are needed for the full two-dimensional spatial line. Taking $r\geq0$ without an additional construction would omit one of its two ends. The following causal comparison uses the AdS [universal cover](../../../algebraic-topology.md#universal-cover).

Both models are maximally symmetric [Lorentzian manifolds](../../../topology.md#lorentzian-manifold), with [constant sectional curvature](../../../general-relativity.md#constant-sectional-curvature) and no curvature singularities. In the paper's convention their [Ricci scalars](../../../general-relativity.md#ricci-scalar) are respectively $+2$ and $-2$. The de Sitter spatial scale factor $a(t)=\cosh t$ contracts to a nonzero minimum and then expands; $t=0$ is not a big-bang singularity. The AdS metric is static, and $\partial_t$ is timelike everywhere because $g_{tt}=\cosh^2r>0$.

The embeddings give a concise classification of all affinely parametrized [geodesics](../../../riemannian-geometry.md#geodesic). [Geodesic](../../../riemannian-geometry.md#geodesic) [acceleration](../../../classical-mechanics.md#acceleration) in the ambient space is normal to the hyperboloid, hence proportional to $X$. Differentiating the constraint and setting $X'^2=\kappa$, with $\kappa=1,0,-1$ for timelike, null and spacelike curves, gives

$$
X''=\kappa X\quad\text{in de Sitter},\qquad
X''=-\kappa X\quad\text{in anti-de Sitter}.
$$

Every solution stays in the two-plane spanned by its initial point $P$ and tangent $V$, so every [geodesic](../../../riemannian-geometry.md#geodesic) is a plane section through the ambient origin. For de Sitter, these are $P\cosh s+V\sinh s$ for timelike curves, $P+sV$ for null curves, and $P\cos s+V\sin s$ for spacelike curves. Thus [timelike geodesics](../../../general-relativity.md#timelike-geodesic) and [null geodesics](../../../special-relativity.md#null-geodesic) are complete and nonclosed, while [spacelike geodesics](../../../riemannian-geometry.md#spacelike-geodesic) are closed circles on the ordinary hyperboloid. These are the [geodesics of two-dimensional de Sitter spacetime](../../../general-relativity.md#geodesics-of-two-dimensional-de-sitter-spacetime).

For AdS the roles of the circular and hyperbolic solutions are reversed: timelike curves are $P\cos s+V\sin s$, null curves are $P+sV$, and spacelike curves are $P\cosh s+V\sinh s$. Timelike curves close after [proper time](../../../special-relativity.md#proper-time) $2\pi$ on the hyperboloid, but their lifts on the [universal cover](../../../algebraic-topology.md#universal-cover) continue to ever later time rather than forming closed curves. All three kinds extend for arbitrary [affine parameter](../../../riemannian-geometry.md#affine-parameter). This is [geodesics of two-dimensional anti-de Sitter spacetime](../../../general-relativity.md#geodesics-of-two-dimensional-anti-de-sitter-spacetime), not an assertion that [geodesics](../../../riemannian-geometry.md#geodesic) reach the [conformal boundary](../../../geometry-and-topology.md#conformal-boundary) in finite physical affine length.

The coordinate first integrals make the behavior concrete. In de Sitter, spatial rotational symmetry gives a conserved $P_\chi=\cosh^2t\,d\chi/ds$, and normalization gives

$$
\left(\frac{dt}{ds}\right)^2=\kappa+\frac{P_\chi^2}{\cosh^2t},\qquad
\frac{d\chi}{ds}=\frac{P_\chi}{\cosh^2t}.
$$

Constant-$\chi$ observers are [timelike geodesics](../../../general-relativity.md#timelike-geodesic). Nontrivial [null geodesics](../../../special-relativity.md#null-geodesic) have [affine parameter](../../../riemannian-geometry.md#affine-parameter) proportional to $\sinh t$, which diverges at both $t\to\pm\infty$. In AdS the conserved static [energy](../../../classical-mechanics.md#energy) is $E=\cosh^2r\,dt/ds$, with

$$
\left(\frac{dr}{ds}\right)^2=\frac{E^2}{\cosh^2r}-\kappa.
$$

For timelike curves, $E\geq1$ and

$$
\sinh r=\sqrt{E^2-1}\sin(s-s_0).
$$

They oscillate through the center and never reach spatial infinity; $r=0$ is the $E=1$ [geodesic](../../../riemannian-geometry.md#geodesic). For null curves, $\lambda=\pm\sinh r/E+\text{constant}$, so both ends are at infinite [affine parameter](../../../riemannian-geometry.md#affine-parameter). Spacelike AdS [geodesics](../../../riemannian-geometry.md#geodesic) likewise extend to the two spatial ends.

For the [conformal structure](../../../geometry-and-topology.md#conformal-structure), introduce de Sitter [conformal time](../../../cosmology.md#conformal-time)

$$
\eta=\arctan(\sinh t),\qquad -\frac\pi2<\eta<\frac\pi2,\qquad
\boxed{ds^2=\sec^2\eta\,(d\eta^2-d\chi^2).}
$$

Multiplying by $\cos^2\eta$ gives the [conformal cylinder of two-dimensional de Sitter spacetime](../../../general-relativity.md#conformal-cylinder-of-two-dimensional-de-sitter-spacetime). The past and future conformal infinities are spacelike circles at $\eta=\mp\pi/2$. Null curves are $\chi=\pm\eta+\text{constant}$ modulo $2\pi$. Although the conformal-time interval is finite, their physical [affine parameters](../../../riemannian-geometry.md#affine-parameter) and timelike observers' proper times are infinite at its ends. Constant-$\eta$ circles are [Cauchy hypersurfaces](../../../general-relativity.md#cauchy-surface); global de Sitter is [globally hyperbolic](../../../general-relativity.md#globally-hyperbolic-spacetime).

For AdS put

$$
\psi=\arctan(\sinh r),\qquad -\frac\pi2<\psi<\frac\pi2,\qquad
\boxed{ds^2=\sec^2\psi\,(dt^2-d\psi^2).}
$$

The [conformal strip of two-dimensional anti-de Sitter spacetime](../../../general-relativity.md#conformal-strip-of-two-dimensional-anti-de-sitter-spacetime) has unbounded time and timelike [conformal boundaries](../../../geometry-and-topology.md#conformal-boundary) at $\psi=\pm\pi/2$. Null curves have $t\pm\psi=\text{constant}$. A signal from any finite $r$ reaches the center in coordinate time $|\psi|<\pi/2$, and a null curve crosses the entire conformal strip in time $\pi$. This finite coordinate travel time coexists with infinite physical affine length to the boundary. The covering spacetime has no [closed timelike curves](../../../general-relativity.md#closed-timelike-curve), but is not [globally hyperbolic](../../../general-relativity.md#globally-hyperbolic-spacetime): causal curves can arrive from timelike infinity without meeting a proposed initial slice. Field evolution consequently requires boundary conditions as well as initial data. Unwrapping time removes [closed timelike curves](../../../general-relativity.md#closed-timelike-curve), not the timelike boundary.

The contrast in [observer event horizons](../../../general-relativity.md#observer-event-horizon) follows directly from these null curves. For the complete de Sitter observer $\chi=0$, let $d(\chi,0)\in[0,\pi]$ be shortest angular distance. An event can send a signal to this observer before its future endpoint precisely when

$$
d(\chi,0)<\frac\pi2-\eta.
$$

Equality is its future [observer event horizon](../../../general-relativity.md#observer-event-horizon). It can receive a signal emitted by the observer after its past endpoint precisely when $d(\chi,0)<\eta+\pi/2$, whose equality is the past horizon. In the observer's fundamental domain these horizons are null lines

$$
\chi=\pm(\pi/2-\eta),\qquad\chi=\pm(\eta+\pi/2).
$$

Their intersection encloses the observer's [static patch of de Sitter spacetime](../../../general-relativity.md#static-patch-of-de-sitter-spacetime), the diamond $d(\chi,0)<\pi/2-|\eta|$. They are observer-dependent [cosmological horizons](../../../general-relativity.md#cosmological-horizon), not curvature singularities or [Cauchy horizons](../../../general-relativity.md#cauchy-horizon). Every inertial observer has the corresponding horizons by de Sitter symmetry.

For the complete AdS static observer at $r=0$, every event at finite $r$ can send a signal to the observer, and can receive one, because time is unbounded and the coordinate distance $|\psi|$ is finite. Thus there is no corresponding global static-observer event horizon. The lapse never vanishes in these coordinates. Restricted accelerated-observer patches can have observer horizons, but those are distinct from the global static model. On the original periodic-time AdS hyperboloid, the more serious issue is [closed timelike curves](../../../general-relativity.md#closed-timelike-curve).

<a id="4/image-conformal-cylinder-of-de-sitter-and-covering-anti-de-sitter-strip-showing-null-geodesics-observer-horizons-and-causal-boundaries"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-61-conformal-models.png)

**[Figure 1](#4/image-conformal-cylinder-of-de-sitter-and-covering-anti-de-sitter-strip-showing-null-geodesics-observer-horizons-and-causal-boundaries). Conformal cylinder of de Sitter and covering anti-de Sitter strip, showing null geodesics, observer horizons and causal boundaries**.

The figure identifies the de Sitter spatial edges and displays only a finite time window of the AdS covering strip, whose time continues indefinitely. Solid red curves are [null geodesics](../../../special-relativity.md#null-geodesic); the oscillating AdS curve is a [timelike geodesic](../../../general-relativity.md#timelike-geodesic). The shaded de Sitter diamond is the static observer's two-way communication region, not the entire spacetime.

The concise comparison is **de Sitter has spacelike conformal infinities and cosmological observer horizons; covering AdS has timelike [conformal boundaries](../../../geometry-and-topology.md#conformal-boundary) and no horizon for an eternal global static observer**. Both are constant-curvature and geodesically complete, but their [geodesic](../../../riemannian-geometry.md#geodesic) recurrence, global topology, causal boundaries and initial-value properties differ.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
