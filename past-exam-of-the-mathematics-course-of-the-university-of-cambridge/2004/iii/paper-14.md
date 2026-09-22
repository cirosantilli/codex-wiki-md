# Paper 14

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper14.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper14.pdf)

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

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A smooth [vector field](../../../calculus.md#vector-field) on a [smooth manifold](../../../differential-geometry.md#smooth-manifold) $M$ is a smooth [section of a vector bundle](../../../fiber-bundle.md#section-of-a-vector-bundle) $X:M\to TM$ of the [tangent bundle](../../../fiber-bundle.md#tangent-bundle) projection $\pi$, so $\pi\circ X=\mathrm{id}_M$. In a coordinate chart it has the form $X=\sum_iX^i\partial_i$ with smooth component functions $X^i$.

Suppose a smooth [vector bundle isomorphism](../../../fiber-bundle.md#vector-bundle-isomorphism) $\Phi:M\times\mathbb R^n\to TM$ covering the identity is given. For the standard [basis](../../../vector-space.md#basis) $e_1,\ldots,e_n$ of $\mathbb R^n$, put $X_i(p)=\Phi(p,e_i)$. These are smooth [vector fields](../../../calculus.md#vector-field), and the [linear isomorphism](../../../vector-space.md#linear-isomorphism) on each fibre makes $X_1(p),\ldots,X_n(p)$ a [basis](../../../vector-space.md#basis) of $T_pM$.

Conversely, given such a global [frame of a vector bundle](../../../fiber-bundle.md#frame-of-a-vector-bundle), define

$$
\boxed{\Phi(p,a_1,\ldots,a_n)=\sum_{i=1}^na_iX_i(p).}
$$

It is smooth, covers the identity and is a [linear isomorphism](../../../vector-space.md#linear-isomorphism) on each fibre. Its inverse is smooth as well: in any coordinate chart, the component columns of the $X_i$ form an invertible smooth [matrix](../../../vector-space.md#matrix) $C(p)$, and the fibre coordinates of the inverse are $C(p)^{-1}v$. [matrix](../../../vector-space.md#matrix) inversion is smooth on the invertible [matrices](../../../vector-space.md#matrix). Thus **the [tangent bundle](../../../fiber-bundle.md#tangent-bundle) is trivial exactly when a global frame exists**, the defining property of a [parallelizable manifold](../../../differential-geometry.md#parallelizable-manifold).

For a [Lie group](../../../lie-theory.md#lie-group) $G$, write $L_h(g)=hg$. A [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field) is a field satisfying

$$
X(hg)=(dL_h)_gX(g).
$$

Such a field is determined by $v=X(e)\in T_eG$, since $X(g)=(dL_g)_ev$. Conversely, this formula defines a left-invariant field, by the [chain rule](../../../calculus.md#chain-rule) and $L_hL_g=L_{hg}$.

It also proves smoothness even if smoothness was not initially assumed. Choose a [smooth curve](../../../differential-geometry.md#smooth-curve) $c(t)$ with $c(0)=e$, $c'(0)=v$. Then

$$
X(g)=\left.\frac{d}{dt}\right|_{t=0}g\,c(t).
$$

Multiplication is a [smooth map](../../../differential-geometry.md#smooth-map-between-manifolds) on a [Lie group](../../../lie-theory.md#lie-group), so differentiating its coordinate functions in the second variable yields a [smooth function](../../../analysis.md#smooth-function) of $g$. This gives smooth components for $X$ in every local chart.

Choose a [basis](../../../vector-space.md#basis) $v_1,\ldots,v_m$ of $T_eG$, where $m=\dim G$, and left translate it. Each $L_g$ is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), with inverse $L_{g^{-1}}$, so $(dL_g)_e$ is a [linear isomorphism](../../../vector-space.md#linear-isomorphism) and the translated fields are a [basis](../../../vector-space.md#basis) at every $g$. The explicit [parallelization of a Lie group by left translations](../../../lie-theory.md#parallelization-of-a-lie-group-by-left-translations) is

$$
\boxed{G\times T_eG\longrightarrow TG,\qquad(g,v)\longmapsto(dL_g)_ev.}
$$

Its inverse sends $w\in T_gG$ to $(g,(dL_{g^{-1}})_gw)$. Identifying $T_eG$ with $\mathbb R^m$ gives the required product bundle. The differential facts used are linearity, the chain rule, $d(\mathrm{id})=\mathrm{id}$ and smooth dependence of the differential of a [smooth map](../../../differential-geometry.md#smooth-map-between-manifolds) on its base point.

## 2

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A smooth right [group action](../../../group-theory.md#group-action) is a [smooth map](../../../differential-geometry.md#smooth-map-between-manifolds) $(p,g)\mapsto p\cdot g$ from $P\times G$ to $P$, with $p\cdot e=p$ and $(p\cdot g)\cdot h=p\cdot(gh)$. It is a [free action of a group](../../../group-theory.md#free-action-of-a-group) if $p\cdot g=p$ implies $g=e$.

A smooth [principal bundle](../../../fiber-bundle.md#principal-bundle) consists of such a free action and a surjective map $\pi:P\to B$ whose fibres are the orbits, together with equivariant [local trivializations](../../../fiber-bundle.md#local-trivialization)

$$
\Phi:\pi^{-1}(N)\longrightarrow N\times G,
\qquad \operatorname{pr}_1\Phi=\pi,
\qquad \Phi(p\cdot h)=\Phi(p)\cdot h,
$$

where $(x,g)\cdot h=(x,gh)$. The trivializations are [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism); in particular the bundle projection is a [submersion](../../../differential-geometry.md#submersion).

For two such trivializations, $H=\Phi_2\Phi_1^{-1}$ fixes the base coordinate and is equivariant. Write $H(x,e)=(x,\psi(x))$. Equivariance immediately gives

$$
\boxed{H(x,g)=H((x,e)\cdot g)=(x,\psi(x)g).}
$$

The function $\psi$ is smooth because $x\mapsto(x,e)$ and $H$ are smooth. This proves the general [transition function of a principal bundle](../../../fiber-bundle.md#transition-function-of-a-principal-bundle) formula; the multiplier is on the left, even though the original action is on the right.

For the explicit bundle, represent a point of $\mathbb{RP}^3$ by a nonzero vector $w=(w_1,w_2)\in\mathbb C^2$ modulo nonzero real scaling. The map sends $[w]$ to the complex line $[w_1:w_2]$, so it is well-defined and surjective. Its smoothness follows from the local ratio charts below. Ordinary scalar multiplication by $u\in U(1)$ would not be free, since $u=-1$ acts trivially on real projective classes. Instead define

$$
\boxed{[w]\cdot u=[\lambda w],\qquad \lambda\in U(1),\quad\lambda^2=u.}
$$

The two possible roots differ by a real sign, so give the same class. This is independent of the real representative of $[w]$. Products of chosen roots show the right action law, and the identity acts trivially. Locally on $U(1)$ a smooth square-root branch exists; these local definitions agree projectively and prove global smoothness of the action.

If $[\lambda w]=[w]$, then $\lambda w=rw$ for some nonzero real $r$. Since $w\ne0$ and $|\lambda|=1$, this forces $\lambda=\pm1$ and hence $u=1$. The action is free. Two points in the same fibre have representatives $w'=cw$ for some $c\in\mathbb C^*$; absorb $|c|$ into the real scaling and use $u=(c/|c|)^2$. Thus the orbits are exactly the fibres.

Let $N_1=\{[z:1]\}$ and $N_2=\{[1:\zeta]\}$. Using these base coordinates, define

$$
\begin{aligned}
\Phi_1([w_1,w_2])&=\left(\frac{w_1}{w_2},\left(\frac{w_2}{|w_2|}\right)^2\right)\quad(w_2\ne0),\\
\Phi_2([w_1,w_2])&=\left(\frac{w_2}{w_1},\left(\frac{w_1}{|w_1|}\right)^2\right)\quad(w_1\ne0).
\end{aligned}
$$

Both formulas are invariant under real nonzero scaling, including negative scaling. Their inverses are

$$
\Phi_1^{-1}(z,u)=[\lambda z,\lambda],\qquad
\Phi_2^{-1}(\zeta,u)=[\lambda,\lambda\zeta],\qquad\lambda^2=u.
$$

Again the sign of the root does not matter. Direct substitution shows they are two-sided inverses. The forward maps are smooth, and local square-root branches prove that the inverses are smooth. Under the right action, each squared phase is multiplied by $u$, so the maps are equivariant. They are therefore genuine principal trivializations of the [principal circle bundle on real projective three-space](../../../fiber-bundle.md#principal-circle-bundle-on-real-projective-three-space).

On the overlap $z\ne0$, we have $\zeta=1/z$ and

$$
\left(\frac{w_1}{|w_1|}\right)^2
=\left(\frac{z}{|z|}\right)^2\left(\frac{w_2}{|w_2|}\right)^2.
$$

Consequently

$$
\boxed{\Phi_2\Phi_1^{-1}(z,u)=\left(\frac1z,\frac{z}{\overline z}u\right),
\qquad\psi_{21}(z)=\frac{z}{\overline z}.}
$$

When the base point itself, rather than its chart coordinate, is written as $x$, its coordinate remains $x$ in the general transition formula. The opposite transition has reciprocal multiplier. The doubled phase is essential to freeness and is not the ordinary Hopf-bundle phase.

## 3

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) $E\to M$ is a linear map $D:\Gamma(E)\to\Omega^1(M;E)$ with $D(fs)=df\otimes s+fDs$. Write a [local frame](../../../fiber-bundle.md#frame-of-a-vector-bundle) as a row $e=(e_1,\ldots,e_r)$, and a section as $s=eu$ with a coefficient column $u$. If the [connection one-form](../../../fiber-bundle.md#connection-one-form) is the [matrix](../../../vector-space.md#matrix) $A=\sum_iA_i\,dx^i$, then

$$
\boxed{D(eu)=e(du+Au),\qquad
(D_is)^a=\partial_i u^a+\sum_b(A_i)^a{}_bu^b.}
$$

This fixes the [matrix](../../../vector-space.md#matrix) convention for all subsequent signs.

For an $E$-valued [differential form](../../../differential-form.md) of degree $k$, represented locally by a column $\alpha$ of ordinary forms, its [covariant exterior derivative](../../../fiber-bundle.md#exterior-covariant-derivative) is

$$
\boxed{d_A\alpha=d\alpha+A\wedge\alpha.}
$$

The defining [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) with a scalar form $\omega$ of degree $j$ is

$$
d_A(\omega\wedge\alpha)=d\omega\wedge\alpha+(-1)^j\omega\wedge d_A\alpha.
$$

It follows by moving the one-form $A$ past $\omega$, which introduces $(-1)^j$. It uniquely extends the connection on sections.

The induced [endomorphism bundle connection](../../../fiber-bundle.md#endomorphism-bundle-connection) is characterized on an endomorphism section $T$ by $(D^{\rm End}T)s=D(Ts)-T(Ds)$. For a matrix-valued form $\beta$ of degree $k$, the extension is

$$
\boxed{d_A^{\rm End}\beta=d\beta+A\wedge\beta-(-1)^k\beta\wedge A.}
$$

Indeed it is exactly the formula that makes

$$
d_A(\beta\wedge\alpha)=(d_A^{\rm End}\beta)\wedge\alpha+(-1)^k\beta\wedge d_A\alpha.
$$

The [endomorphism-valued exterior product](../../../fiber-bundle.md#endomorphism-valued-exterior-product) uses [matrix](../../../vector-space.md#matrix) composition as well as the ordinary [exterior product](../../../linear-algebra.md#exterior-product), so factors cannot in general be interchanged.

Define the [curvature form of a connection](../../../fiber-bundle.md#curvature-form) by $D^2$ acting on sections, or equivalently by

$$
F(X,Y)s=D_XD_Ys-D_YD_Xs-D_{[X,Y]}s.
$$

It is tensorial in both vector arguments and in $s$: the derivatives of multiplying functions cancel by the connection rule. For example $D^2(fs)=D(df\,s+fDs)=fD^2s$, since the two $df\wedge Ds$ terms cancel and $d^2f=0$. Thus curvature is a two-form with values in the [endomorphism bundle](../../../fiber-bundle.md#endomorphism-bundle). Locally, applying the graded rule gives

$$
(d+A\wedge)^2\alpha=(dA+A\wedge A)\wedge\alpha,
$$

so

$$
\boxed{F(A)=dA+A\wedge A,\qquad
F_{ij}=\partial_iA_j-\partial_jA_i+[A_i,A_j].}
$$

For a [change of frame of a vector-bundle connection](../../../fiber-bundle.md#change-of-frame-of-a-vector-bundle-connection) $e'=eg$, the coefficients satisfy $u'=g^{-1}u$, and differentiation gives

$$
A'=g^{-1}Ag+g^{-1}dg,\qquad d_{A'}=g^{-1}d_Ag.
$$

Squaring yields $F'=g^{-1}Fg$, precisely the transformation rule of an endomorphism-valued two-form. This independently proves that the local expressions define one global [curvature form of a connection](../../../fiber-bundle.md#curvature-form).

For the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity), use the endomorphism formula with degree two:

$$
\begin{aligned}
d_A^{\rm End}F
&=dF+A\wedge F-F\wedge A\\
&=(dA\wedge A-A\wedge dA)
 +(A\wedge dA+A\wedge A\wedge A)\\
&\hspace{1em}-(dA\wedge A+A\wedge A\wedge A)=0.
\end{aligned}
$$

Every term cancels with its indicated sign. Therefore

$$
\boxed{d_A F(A)=0,}
$$

where $d_A$ here means the induced derivative on the [endomorphism bundle](../../../fiber-bundle.md#endomorphism-bundle).

For a [line bundle](../../../ringed-space.md#line-bundle), the [endomorphism bundle](../../../fiber-bundle.md#endomorphism-bundle) is canonically the trivial scalar bundle: every fibre endomorphism is a scalar times the identity. Scalar multiplication commutes, so $A\wedge A=0$ and the endomorphism covariant derivative on scalar-valued forms reduces to $d$. The [Bianchi identity](../../../fiber-bundle.md#bianchi-identity) consequently says $dF=0$.

If $D'$ is another connection, their difference is $C^\infty$-linear in sections because the Leibniz terms cancel. Hence $D'-D=\eta$ is a global endomorphism-valued one-form; for a [line bundle](../../../ringed-space.md#line-bundle) it is an ordinary global scalar one-form. Locally $A'=A+\eta$, so

$$
F(D')-F(D)=d\eta.
$$

Thus the two closed curvatures differ by an exact form, proving the [connection-independent curvature class of a line bundle](../../../fiber-bundle.md#connection-independent-curvature-class-of-a-line-bundle):

$$
\boxed{[F(D')]=[F(D)]\in H^2_{\rm dR}(M;\mathbb K).}
$$

No global trivialization of the [line bundle](../../../ringed-space.md#line-bundle) itself was assumed; it is its [endomorphism bundle](../../../fiber-bundle.md#endomorphism-bundle) that has the canonical scalar identification.

## 4

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [geodesic](../../../riemannian-geometry.md#geodesic) is an affinely parametrized [curve](../../../topology.md#curve) satisfying $\nabla_{\dot\gamma}\dot\gamma=0$ for the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) of the [Riemannian metric](../../../differential-geometry.md#riemannian-metric). In coordinates, write $\nabla_{\partial_i}\partial_j=\Gamma^k_{ij}\partial_k$. For a [vector field](../../../calculus.md#vector-field) $V(t)=V^k(t)\partial_k$ along the [curve](../../../topology.md#curve),

$$
\left(\nabla_{\dot\gamma}V\right)^k=\frac{dV^k}{dt}+\Gamma^k_{ij}(\gamma(t))\dot\gamma^iV^j.
$$

Putting $V=\dot\gamma$ gives the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation)

$$
\boxed{\ddot\gamma^k+\Gamma^k_{ij}(\gamma)\dot\gamma^i\dot\gamma^j=0.}
$$

This is a smooth second-order ordinary differential system, so the [Picard-Lindelöf theorem](../../../differential-equation.md#picard-lindelof-theorem) gives local existence and uniqueness for prescribed position and velocity.

To prove [local extension of geodesic velocity](../../../riemannian-geometry.md#local-extension-of-geodesic-velocity), first suppose $\dot\gamma(0)=0$. The constant [curve](../../../topology.md#curve) through $\gamma(0)$ solves this initial value problem, so uniqueness makes $\gamma$ constant locally. The zero [vector field](../../../calculus.md#vector-field) is the desired extension.

Otherwise choose a chart about $\gamma(0)$ in which the first component of the coordinate velocity is nonzero. Write the coordinate [curve](../../../topology.md#curve) as $c(t)\in\mathbb R^n$ and define

$$
\Psi(t,z_2,\ldots,z_n)=c(t)+\sum_{j=2}^nz_je_j.
$$

At $(0,0)$ its derivative has columns $c'(0),e_2,\ldots,e_n$ and is invertible, because the first component of $c'(0)$ is nonzero. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) therefore supplies coordinates $(t,z_2,\ldots,z_n)$ on an open neighbourhood after shrinking the parameter interval to $|t|<\delta$. Along the [curve](../../../topology.md#curve) these coordinates are $(t,0,\ldots,0)$. The smooth coordinate field $\partial/\partial t$, pushed back through $\Psi$ and the original chart, agrees with $\dot\gamma(t)$. This proves the extension without assuming that a long [geodesic](../../../riemannian-geometry.md#geodesic) has no self-intersections.

By [metric compatibility](../../../fiber-bundle.md#metric-compatibility), differentiation along the [curve](../../../topology.md#curve) gives

$$
\frac d{dt}g(\dot\gamma,\dot\gamma)
=2g(\nabla_{\dot\gamma}\dot\gamma,\dot\gamma)=0.
$$

The local extension above permits the ordinary vector-field version of the metric identity to be used along the arc, or the same identity follows directly from the coordinate derivative. Hence **an affinely parametrized [geodesic](../../../riemannian-geometry.md#geodesic) has constant speed**, including the zero-speed case.

Now let $S^n$ be the unit [sphere](../../../geometry-and-topology.md#sphere) in $\mathbb R^{n+1}$. Its induced Levi-Civita derivative is the tangential projection of the ordinary ambient derivative: projection preserves the metric identity, and the commuting ambient coordinate derivatives give zero torsion. By uniqueness of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection), proved in Question 5, this is the induced connection.

Thus a [curve](../../../topology.md#curve) on the [sphere](../../../geometry-and-topology.md#sphere) is a [geodesic](../../../riemannian-geometry.md#geodesic) exactly when its ambient acceleration has no tangential component. The normal space is spanned by $\gamma$, so $\gamma''=a(t)\gamma$. Differentiating $\gamma\cdot\gamma=1$ twice gives $\gamma\cdot\gamma'=0$ and

$$
a(t)=\gamma\cdot\gamma''=-|\gamma'|^2=-c^2,
$$

where $c\geq0$ is the constant speed. Therefore $\gamma''+c^2\gamma=0$. With initial data $\gamma(0)=p$ and $\gamma'(0)=v$, all solutions are

$$
\boxed{\gamma(t)=p\cos(ct)+\frac vc\sin(ct),\quad
|p|=1,\quad p\cdot v=0,\quad |v|=c>0,}
$$

and, when $v=0$, $\boxed{\gamma(t)=p}$. The [orthogonality](../../../linear-algebra.md#orthogonal-vectors) and length conditions show directly that the displayed [curve](../../../topology.md#curve) remains on the [sphere](../../../geometry-and-topology.md#sphere), and its acceleration is $-c^2\gamma$, so it is indeed a [geodesic](../../../riemannian-geometry.md#geodesic). The nonconstant [geodesics](../../../riemannian-geometry.md#geodesic) are the [great circles](../../../geometry-and-topology.md#great-circle) traversed at any constant speed; arbitrary parameter intervals give their restrictions, and shifting the initial parameter simply shifts the formula. There are no other [geodesics](../../../riemannian-geometry.md#geodesic).

## 5

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) is a connection on the [tangent bundle](../../../fiber-bundle.md#tangent-bundle) which is [torsion-free](../../../fiber-bundle.md#torsion-free-connection) and compatible with the [Riemannian metric](../../../differential-geometry.md#riemannian-metric). Its defining identities are

$$
\nabla_XY-\nabla_YX=[X,Y],\qquad
Xg(Y,Z)=g(\nabla_XY,Z)+g(Y,\nabla_XZ).
$$

To obtain uniqueness, write the metric identity for $(X,Y,Z)$, $(Y,Z,X)$ and $(Z,X,Y)$, add the first two and subtract the third, and use the torsion identity to interchange the derivatives. This gives the [Koszul formula](../../../fiber-bundle.md#koszul-formula)

$$
\begin{aligned}
2g(\nabla_XY,Z)
={}&Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)\\
&-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
\end{aligned}
$$

The metric is nondegenerate, so these [inner products](../../../linear-algebra.md#inner-product) determine $\nabla_XY$ uniquely.

For existence, let $K(X,Y,Z)$ denote the right-hand side. The bracket rules $[X,fY]=f[X,Y]+X(f)Y$ and $[fX,Y]=f[X,Y]-Y(f)X$ give, by cancellation of all extra derivatives,

$$
\begin{aligned}
K(fX,Y,Z)&=fK(X,Y,Z),\\
K(X,fY,Z)&=fK(X,Y,Z)+2X(f)g(Y,Z),\\
K(X,Y,fZ)&=fK(X,Y,Z).
\end{aligned}
$$

Thus the nondegenerate metric defines a unique smooth [vector field](../../../calculus.md#vector-field) $\nabla_XY$ from $2g(\nabla_XY,Z)=K(X,Y,Z)$, and these identities give the connection rules. In coordinates the construction reads

$$
\boxed{\Gamma^k_{ij}=\frac12g^{k\ell}
\big(\partial_i g_{j\ell}+\partial_jg_{i\ell}-\partial_\ell g_{ij}\big).}
$$

The coefficients are smooth and symmetric in $i,j$, proving zero torsion. Substituting them gives

$$
g_{\ell k}\Gamma^\ell_{ij}+g_{j\ell}\Gamma^\ell_{ik}=\partial_i g_{jk},
$$

which is exactly [metric compatibility](../../../fiber-bundle.md#metric-compatibility). Since the construction was given intrinsically by $K$, the local formulas agree on overlaps. This proves [existence and uniqueness of the Levi-Civita connection](../../../fiber-bundle.md#existence-and-uniqueness-of-the-levi-civita-connection) on every [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold).

Define the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) by

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z.
$$

The connection rules make this expression tensorial in all three arguments. To fix the component convention, throughout this solution use

$$
R_{ijkl}=g\big(R(e_i,e_j)e_l,e_k\big).
$$

With this convention, the unit [sphere](../../../geometry-and-topology.md#sphere) has $R_{ijkl}=g_{ik}g_{jl}-g_{il}g_{jk}$ and positive [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature). In a coordinate frame, the components are obtained from

$$
\big(R(\partial_i,\partial_j)\partial_l\big)^a
=\partial_i\Gamma^a_{jl}-\partial_j\Gamma^a_{il}
+\Gamma^a_{ib}\Gamma^b_{jl}-\Gamma^a_{jb}\Gamma^b_{il}.
$$

The algebraic curvature symmetries are

$$
\boxed{R_{ijkl}=-R_{jikl}=-R_{ijlk},\qquad R_{ijkl}=R_{klij},}
$$

together with the [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity)

$$
R(X,Y)Z+R(Y,Z)X+R(Z,X)Y=0,
\qquad R_{ijkl}+R_{jlki}+R_{likj}=0.
$$

The first antisymmetry follows from the definition. [Metric compatibility](../../../fiber-bundle.md#metric-compatibility) gives $g(R(X,Y)Z,W)+g(Z,R(X,Y)W)=0$, giving the second. Torsion-freeness reduces the cyclic sum to the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) for [Lie brackets of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields); pair interchange follows algebraically from these antisymmetries and the cyclic identity. These explain the identities rather than choosing unrelated sign conventions.

Define the [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) by the [tensor contraction](../../../linear-algebra.md#tensor-contraction)

$$
\operatorname{Ric}(Y,Z)=\operatorname{tr}\{X\mapsto R(X,Y)Z\},
\qquad \operatorname{Ric}_{jl}=g^{ik}R_{ijkl}.
$$

This is a [bilinear form](../../../linear-algebra.md#bilinear-form), since $R$ is tensorial and [trace](../../../linear-algebra.md#matrix-trace) is linear. At a point choose an orthonormal [basis](../../../vector-space.md#basis). Pair interchange gives

$$
\operatorname{Ric}_{lj}=\sum_iR_{ilij}
=\sum_iR_{ijil}=\operatorname{Ric}_{jl},
$$

so **[Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) is symmetric**.

For the final determination in dimension three, an algebraic curvature tensor is determined by its entries in the three unordered index pairs $12,13,23$: antisymmetry removes repeated indices, and pair interchange makes the resulting $3\times3$ array symmetric. It therefore has at most six independent entries. Write

$$
K_{12}=R_{1212},\quad K_{13}=R_{1313},\quad K_{23}=R_{2323}.
$$

The diagonal Ricci components give

$$
\operatorname{Ric}_{11}=K_{12}+K_{13},\quad
\operatorname{Ric}_{22}=K_{12}+K_{23},\quad
\operatorname{Ric}_{33}=K_{13}+K_{23},
$$

so, for example, $K_{12}=(\operatorname{Ric}_{11}+\operatorname{Ric}_{22}-\operatorname{Ric}_{33})/2$, and the other two follow cyclically. The three off-diagonal entries are also recovered explicitly:

$$
R_{1323}=\operatorname{Ric}_{12},\qquad
R_{1223}=-\operatorname{Ric}_{13},\qquad
R_{1213}=\operatorname{Ric}_{23}.
$$

Thus every independent curvature entry is determined by Ricci; this proves injectivity, not merely a dimension count.

An invariant formula making the reconstruction explicit is, with $S=\operatorname{tr}_g\operatorname{Ric}$,

$$
\boxed{\begin{aligned}
R_{ijkl}={}&g_{ik}\operatorname{Ric}_{jl}+g_{jl}\operatorname{Ric}_{ik}
-g_{il}\operatorname{Ric}_{jk}-g_{jk}\operatorname{Ric}_{il}\\
&-\frac S2(g_{ik}g_{jl}-g_{il}g_{jk}).
\end{aligned}}
$$

To verify it, the right-hand side has the two antisymmetries, pair interchange and the cyclic identity by symmetry of $g$ and Ricci. Contracting its first and third indices in dimension three gives

$$
3\operatorname{Ric}_{jl}+Sg_{jl}-2\operatorname{Ric}_{jl}-Sg_{jl}
=\operatorname{Ric}_{jl}.
$$

Subtract it from the original tensor. The difference has zero Ricci contraction, and the six recovered-entry formulas above force it to vanish. This completes the proof of [three-dimensional curvature from the Ricci tensor](../../../general-relativity.md#three-dimensional-curvature-from-the-ricci-tensor) in arbitrary coordinates.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
