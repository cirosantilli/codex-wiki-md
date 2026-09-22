# Paper 64

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper64.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper64.pdf)

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
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)

## 1

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

An [orthonormal coframe](../../../general-relativity.md#orthonormal-coframe-in-spacetime) writes a metric as $g=\eta_{ab}\theta^a\otimes\theta^b$ with constant diagonal signature [matrix](../../../vector-space.md#matrix) $\eta$. In [Cartan's first structure equation](../../../connection-1-form.md#cartan-s-first-structure-equation), solve

$$
d\theta^a+\omega^a{}_b\wedge\theta^b=0,\qquad
\omega_{ab}=-\omega_{ba},\qquad \omega_{ab}=\eta_{ac}\omega^c{}_b.
$$

These are the torsion-free and metric-compatibility conditions and determine the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). Then [Cartan's second structure equation](../../../connection-1-form.md#cartan-s-second-structure-equation) gives

$$
\Omega^a{}_b=d\omega^a{}_b+\omega^a{}_c\wedge\omega^c{}_b
=\frac12 R^a{}_{bcd}\theta^c\wedge\theta^d.
$$

Contract $R^a{}_{bad}$ to obtain the [Ricci tensor](../../../general-relativity.md#ricci-tensor) and then contract again for the [scalar curvature](../../../second-fundamental-form.md#scalar-curvature). This fixes the curvature convention; reversing the definition of the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) reverses the resulting curvature signs.

On $z>0$, choose $\theta^0=dt/z$, $\theta^1=dx/z$, $\theta^2=dy/z$, $\theta^3=dz/z$, with $\eta=\operatorname{diag}(-1,1,1,1)$. For $a=0,1,2$,

$$
d\theta^a=\theta^a\wedge\theta^3,\qquad d\theta^3=0.
$$

A torsion-free metric connection therefore has

$$
\omega^a{}_3=-\theta^a,\qquad
\omega^3{}_a=\eta_{aa}\theta^a,\qquad
\omega^a{}_b=0\quad(a,b<3).
$$

For example, $\Omega^a{}_3=-d\theta^a=-\theta^a\wedge\theta^3$, while for $a,b<3$,

$$
\Omega^a{}_b=\omega^a{}_3\wedge\omega^3{}_b
=-\eta_{bb}\theta^a\wedge\theta^b.
$$

Metric antisymmetry supplies the remaining components, giving uniformly

$$
\boxed{\Omega^a{}_b=-\theta^a\wedge\theta_b,\qquad
R_{abcd}=-(\eta_{ac}\eta_{bd}-\eta_{ad}\eta_{bc}).}
$$

Thus the metric has constant [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) $-1$. In four dimensions,

$$
\boxed{\operatorname{Ric}_{\mu\nu}=-3g_{\mu\nu},\qquad R=-12.}
$$

It is an [Einstein manifold](../../../second-fundamental-form.md#einstein-manifold), with Einstein constant $-3$ in the stated curvature convention.

These are [Poincare coordinates on anti-de Sitter spacetime](../../../general-relativity.md#poincare-coordinates-on-anti-de-sitter-spacetime) of unit radius. Constant curvature gives the maximal ten-dimensional local [isometry](../../../riemannian-geometry.md#isometry) algebra $\mathfrak{so}(3,2)$. This can also be checked directly: set $u=(t,x,y)$, $\eta_{ab}=\operatorname{diag}(-1,1,1)$ and $u_a=\eta_{ab}u^b$. The ten independent [Killing vector fields](../../../general-relativity.md#killing-vector-field) are

$$
P_a=\partial_a,\qquad
M_{ab}=u_a\partial_b-u_b\partial_a,\qquad
D=u^a\partial_a+z\partial_z,\qquad
K_a=2u_aD-(u^bu_b+z^2)\partial_a.
$$

Translations and [Lorentz transformations](../../../special-relativity.md#lorentz-transformation) leave the numerator and $z$ unchanged. A dilation rescales numerator and denominator equally. For $K_a$, direct differentiation gives $\mathcal L_{K_a}\eta^{(4)}=4u_a\eta^{(4)}$ and $K_a(z)=2u_a z$, so the [conformal factor](../../../general-relativity.md#conformal-factor) cancels and $\mathcal L_{K_a}g=0$.

Hence the maximally extended [Anti-de Sitter spacetime](../../../general-relativity.md#anti-de-sitter-spacetime) has connected [isometry](../../../riemannian-geometry.md#isometry) group locally $SO_0(3,2)$, with the appropriate covering group if one unwraps its time coordinate. The displayed coordinates cover only a patch. The ten local generators do not all give globally complete flows preserving that patch; for example special conformal flows can cross its horizon. The manifest complete patch symmetries include the boundary Poincare transformations and positive dilations. This distinguishes local maximal symmetry from the global [isometries](../../../riemannian-geometry.md#isometry) of a chosen coordinate domain.

## 2

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $\mathcal J=\star J$ be the current $(d-1)$-form on an oriented $d$-dimensional spacetime. For a slab bounded by two spacelike hypersurfaces $\Sigma_1,\Sigma_2$ and a side boundary $B$, the [Stokes theorem](../../../calculus.md#stokes-theorem) gives

$$
0=\int_Vd\mathcal J=\int_{\Sigma_2}\mathcal J-\int_{\Sigma_1}\mathcal J+\int_B\mathcal J.
$$

Thus $Q(\Sigma)=\int_\Sigma\mathcal J$ is conserved if the side flux vanishes, for example for a spatially compact current or appropriate falloff at infinity. With side flux it instead obeys the corresponding charge-balance equation. This is the differential-form version of current conservation.

For the [Abelian Chern--Simons theory](../../../topological-quantum-matter.md#abelian-chern-simons-theory), take $A\mapsto A+d\chi$ with a smooth compactly supported gauge parameter. The change in the gauge-field term is a boundary term because $d\chi\wedge dA=d(\chi\,dA)$. For the source,

$$
\mathcal J\wedge d\chi=d(\chi\mathcal J)-\chi\,d\mathcal J.
$$

Discarding the boundary terms, the action variation is

$$
\delta_\chi S=c\int\chi\,d\mathcal J.
$$

[Gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) for every such $\chi$ and $c\ne0$ therefore gives **$d\star J=0$**. If $c=0$, the current decouples and [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) places no condition on it. On a spacetime with boundary, boundary conditions or boundary degrees of freedom are also needed to handle the discarded terms; on a nontrivial compact gauge bundle, large-gauge invariance is an additional global issue.

For the field equation, use

$$
\delta(A\wedge dA)=2\delta A\wedge dA-d(A\wedge\delta A).
$$

The [one-form](../../../differential-form.md#one-form) $\delta A$ commutes with the [two-form](../../../differential-form.md#2-form) $\mathcal J$ under the [wedge product](../../../linear-algebra.md#exterior-product), so

$$
\delta S=\int\delta A\wedge(2dA-c\mathcal J)
$$

up to the boundary term. Consequently

$$
\boxed{2dA=c\star J.}
$$

Applying $d$ and using $d^2=0$ again gives current conservation for $c\ne0$. The factor two comes from varying both occurrences of $A$.

Orient a spatial region $D$ so its boundary is $\gamma$, and define $Q_D=\int_D\mathcal J$. Applying [Stokes theorem](../../../calculus.md#stokes-theorem) and the field equation yields

$$
\boxed{\Phi=\oint_\gamma A=\int_DdA=\frac c2Q_D.}
$$

For a [U(1) connection](../../../fiber-bundle.md#u-1-connection), in a convention with unit minimal charge, the gauge-invariant quantity is its [holonomy](../../../fiber-bundle.md#holonomy) $e^{i\Phi}$, the Wilson-loop or Aharonov-Bohm phase. A large [gauge transformation](../../../electromagnetism.md#gauge-transformation) can change the chosen representative of $\Phi$ by $2\pi n$. Therefore **$\Phi$ is a phase angle modulo $2\pi$, rather than an absolute gauge-invariant real number**. A particle of charge $q$ has phase $e^{iq\Phi}$ in the corresponding normalization. The flux-charge relation thus attaches a gauge phase to enclosed charge.

The metric variation requires specifying the independent source. The pure Chern-Simons term $A\wedge dA$ has no metric dependence, hence contributes zero [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor). If the [one-forms](../../../differential-form.md#one-form) named in the question have fixed covariant components $A_\mu,J_\mu$, the [Hodge star](../../../differential-form.md#hodge-star-operator) in the source does depend on the metric:

$$
S_{\mathrm{source}}=-c\int d^3x\,\sqrt{-g}\,g^{\rho\sigma}J_\rho A_\sigma.
$$

Using $\delta\sqrt{-g}=-\sqrt{-g}g_{\mu\nu}\delta g^{\mu\nu}/2$ gives

$$
\delta S_{\mathrm{source}}
=-c\int d^3x\,\sqrt{-g}\left[J_{(\mu}A_{\nu)}-\frac12g_{\mu\nu}J_\rho A^\rho\right]\delta g^{\mu\nu}.
$$

Under that literal fixed-one-form convention,

$$
\boxed{T_{\mu\nu}=2cJ_{(\mu}A_{\nu)}-cg_{\mu\nu}J_\rho A^\rho.}
$$

There is another common convention in the topological source theory: hold the conserved [two-form](../../../differential-form.md#2-form) $\mathcal J=\star J$, equivalently the vector current density, fixed as the metric varies. Then both $A\wedge dA$ and $\mathcal J\wedge A$ are metric-independent, and **$T_{\mu\nu}=0$** for this action. These are different variations, not contradictory calculations. The [Chern-Simons source stress convention](../../../topological-quantum-matter.md#chern-simons-source-stress-convention) explains why a source prescription is necessary; a dynamical matter source would contribute its own action and stress as well.

## 3

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use $\omega=\sum_i dq_i\wedge dp_i$, $\iota_{X_f}\omega=df$ and

$$
\{f,g\}=\sum_i\left(\frac{\partial f}{\partial q_i}\frac{\partial g}{\partial p_i}-\frac{\partial f}{\partial p_i}\frac{\partial g}{\partial q_i}\right).
$$

Then $X_f(g)=\{g,f\}$ and $[X_f,X_g]=-X_{\{f,g\}}$. For a left [group action](../../../group-theory.md#group-action), let $\xi_P(p)=\left.\frac{d}{dt}\right|_0\exp(t\xi)\cdot p$; its fundamental fields obey $[\xi_P,\eta_P]=-[\xi,\eta]_P$.

The components of a [moment map](../../../symplectic-geometry.md#moment-map) satisfy

$$
\mu_\xi(p)=\langle\mu(p),\xi\rangle,\qquad
d\mu_\xi=\iota_{\xi_P}\omega.
$$

Thus $\xi_P=X_{\mu_\xi}$. A [Hamiltonian](../../../classical-mechanics.md#hamiltonian) [moment map](../../../symplectic-geometry.md#moment-map) additionally has coadjoint equivariance,

$$
\mu(gp)=\operatorname{Ad}_{g^{-1}}^*\mu(p).
$$

Here the right side evaluates on $\xi$ as $\langle\mu(p),\operatorname{Ad}_{g^{-1}}\xi\rangle$. With that convention its infinitesimal form is $\{\mu_\xi,\mu_\eta\}=\mu_{[\xi,\eta]}$. Some definitions reserve “[moment map](../../../symplectic-geometry.md#moment-map)” for this equivariant version; choosing Hamiltonians for every generator first gives a [weakly Hamiltonian action](../../../symplectic-geometry.md#weakly-hamiltonian-action).

To derive the obstruction, compare the two antihomomorphism identities:

$$
X_{\{\mu_\xi,\mu_\eta\}-\mu_{[\xi,\eta]}}=0.
$$

On connected $P$, nondegeneracy of $\omega$ makes

$$
\kappa(\xi,\eta)=\{\mu_\xi,\mu_\eta\}-\mu_{[\xi,\eta]}
$$

a constant alternating bilinear form. The two Jacobi identities imply

$$
\kappa([\xi,\eta],\zeta)+\kappa([\eta,\zeta],\xi)+\kappa([\zeta,\xi],\eta)=0.
$$

Replacing $\mu_\xi$ by $\mu_\xi+b(\xi)$ changes $\kappa$ to $\kappa-b([\xi,\eta])$. Thus vanishing of this class in [Lie algebra cohomology](../../../lie-algebra.md#lie-algebra-cohomology) is the precise [moment-map equivariance obstruction](../../../symplectic-geometry.md#moment-map-equivariance-obstruction). In particular **a connected group with $H^2(\mathfrak g,\mathbb R)=0$ permits constants to be chosen so that the component [Poisson algebra](../../../algebra.md#poisson-algebra) is the [Lie algebra](../../../lie-algebra.md)**. A locally effective action makes this realization faithful; otherwise it realizes the quotient by the infinitesimal kernel. The linear span of the components has the Lie brackets; the entire algebra of polynomial products of them is, of course, larger.

A useful sufficient condition is semisimplicity, which can be proved here without assuming the desired equivariance. Let $B$ be the nondegenerate [Killing form](../../../lie-algebra.md#killing-form) and define $D$ by $B(D\xi,\eta)=\kappa(\xi,\eta)$. Invariance of $B$ and the cocycle identity give

$$
B(D[\xi,\eta],\zeta)
=B(D\xi,[\eta,\zeta])+B(D\eta,[\zeta,\xi])
=B([D\xi,\eta]+[\xi,D\eta],\zeta),
$$

so $D$ is a derivation. Choose $Z$ uniquely by $B(Z,\xi)=\operatorname{tr}(D\operatorname{ad}\xi)$. Since $[D,\operatorname{ad}\xi]=\operatorname{ad}(D\xi)$, cyclicity of trace gives

$$
\begin{aligned}
B([Z,\xi],\eta)
&=B(Z,[\xi,\eta])
=\operatorname{tr}\bigl(D[\operatorname{ad}\xi,\operatorname{ad}\eta]\bigr)\\
&=\operatorname{tr}\bigl([D,\operatorname{ad}\xi]\operatorname{ad}\eta\bigr)
=B(D\xi,\eta).
\end{aligned}
$$

Hence $D=\operatorname{ad}Z$ and $\kappa(\xi,\eta)=B(Z,[\xi,\eta])$. The shift $b(\xi)=B(Z,\xi)$ removes the obstruction. This proves [semisimple moment-map equivariance](../../../symplectic-geometry.md#semisimple-moment-map-equivariance); for connected $G$ infinitesimal equivariance integrates along its one-parameter subgroups to group equivariance. It does not claim that arbitrary symplectic actions of arbitrary groups have [moment maps](../../../symplectic-geometry.md#moment-map).

For the Kepler calculation, put $k=Mm$ and work on $r=|\mathbf r|>0$, since the [Hamiltonian](../../../classical-mechanics.md#hamiltonian) is singular at the origin. The [Hamilton equations](../../../classical-mechanics.md#hamilton-s-equations) are

$$
\dot{\mathbf r}=\mathbf p,\qquad
\dot{\mathbf p}=-k\frac{\mathbf r}{r^3}.
$$

The [angular momentum](../../../classical-mechanics.md#angular-momentum) therefore obeys

$$
\dot{\mathbf L}=\mathbf p\times\mathbf p+\mathbf r\times\dot{\mathbf p}=0.
$$

For the [Runge-Lenz vector](../../../classical-mechanics.md#laplace-runge-lenz-vector),

$$
\dot{\mathbf K}=\dot{\mathbf p}\times\mathbf L
-k\left(\frac{\mathbf p}{r}-\frac{\mathbf r(\mathbf r\cdot\mathbf p)}{r^3}\right).
$$

The [vector triple product identity](../../../calculus.md#vector-triple-product) gives $\mathbf r\times\mathbf L=\mathbf r(\mathbf r\cdot\mathbf p)-r^2\mathbf p$. Therefore

$$
\dot{\mathbf p}\times\mathbf L
=k\frac{\mathbf p}{r}-k\frac{\mathbf r(\mathbf r\cdot\mathbf p)}{r^3},
$$

and the terms cancel. Since $\dot f=\{f,H\}$, this proves

$$
\boxed{\{L_i,H\}=\{K_i,H\}=0.}
$$

The conserved quantities consequently generate transformations preserving energy. Their brackets give the [Kepler dynamical symmetry algebra](../../../classical-mechanics.md#kepler-dynamical-symmetry-algebra). On $H<0$, define $\mathbf A=\mathbf K/\sqrt{-2H}$ as a function on that whole open region. Because $H$ Poisson commutes with both vectors, its brackets are

$$
\{L_i,L_j\}=\epsilon_{ijk}L_k,\qquad
\{L_i,A_j\}=\epsilon_{ijk}A_k,\qquad
\{A_i,A_j\}=\epsilon_{ijk}L_k.
$$

With $\mathbf J_\pm=(\mathbf L\pm\mathbf A)/2$ one obtains two commuting $\mathfrak{so}(3)$ algebras:

$$
\{J_{\pm i},J_{\pm j}\}=\epsilon_{ijk}J_{\pm k},\qquad
\{J_{+i},J_{-j}\}=0.
$$

Thus the negative-energy algebra is **$\mathfrak{so}(4)$**. On $H>0$, using $\mathbf A=\mathbf K/\sqrt{2H}$ instead changes the last bracket to $-\epsilon_{ijk}L_k$, yielding **$\mathfrak{so}(3,1)$**, with $\mathbf L$ rotations and $\mathbf A$ boosts. At zero energy the brackets of conserved functions on the characteristic orbit quotient give **$\mathfrak e(3)=\mathfrak{so}(3)\ltimes\mathbb R^3$**, with commuting $\mathbf K$.

There are two global qualifications. First, an energy hypersurface carries a [presymplectic form](../../../symplectic-geometry.md#presymplectic-form): its restricted [two-form](../../../differential-form.md#2-form) has characteristic direction $X_H$. At $H=0$, the literal vector fields of $\mathbf K$ need only commute modulo $X_H$, since differentiating $\{K_i,K_j\}=-2H\epsilon_{ijk}L_k$ still produces an $L_kX_H$ term. On nonzero-energy regions the energy-dependent normalization above gives an exact [Hamiltonian](../../../classical-mechanics.md#hamiltonian) [Lie algebra](../../../lie-algebra.md); one must differentiate that normalization before restricting to a level. Second, completeness is required for a global [group action](../../../group-theory.md#group-action). The collision-excluded Kepler phase space need not have complete hidden-symmetry flows, so the brackets establish local actions (or the appropriate simply connected covers), not an unconditional global action on every unregularized trajectory. Collision regularization supplies the familiar global bound-motion symmetry; this distinction is developed in [https://math.berkeley.edu/~alanw/277papers00/tang.pdf](https://math.berkeley.edu/~alanw/277papers00/tang.pdf) . It does not change the three energy-dependent [Lie algebras](../../../lie-algebra.md) just derived.

## 4

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [principal bundle](../../../fiber-bundle.md#principal-bundle) $\pi:P\to B$ with structure group $G$ has a smooth free right $G$-action, each fibre is a single orbit, and it is locally equivariantly isomorphic to $U\times G\to U$. A representation $\rho:G\to GL(V)$ defines the [associated vector bundle](../../../fiber-bundle.md#associated-vector-bundle)

$$
E=P\times_\rho V=(P\times V)/\sim,\qquad
(p,v)\sim(pg,\rho(g)^{-1}v).
$$

Local sections of $P$ identify $E$ with $U\times V$, and changes of section act by $\rho$ on the fibre coordinates.

A [principal bundle](../../../fiber-bundle.md#principal-bundle) is **trivial if and only if it has a global smooth section**. Given $s:B\to P$, the map $(b,g)\mapsto s(b)g$ is an equivariant isomorphism $B\times G\to P$: freeness and transitivity give its unique inverse on each fibre, and local trivializations make that inverse smooth. Conversely a product bundle has section $b\mapsto(b,e)$. This proves [principal bundle trivialization by a global section](../../../fiber-bundle.md#principal-bundle-trivialization-by-a-global-section). A contractible paracompact base is a sufficient condition for triviality of such a bundle; local sections alone are insufficient on a general base.

A manifold is [parallelizable](../../../differential-geometry.md#parallelizable-manifold) when its [tangent bundle](../../../fiber-bundle.md#tangent-bundle) is trivial, equivalently when it possesses a global smooth frame. The circle $S^1$ is an example, with its nowhere-vanishing unit tangent field. The sphere $S^3$ is another: regard it as the [unit quaternions](../../../algebra.md#unit-quaternion). At a [unit quaternion](../../../algebra.md#unit-quaternion) $q$, the three tangent vectors $qi,qj,qk$ are independent and smoothly depend on $q$. [Quaternion](../../../algebra.md#quaternion) multiplication preserves the [norm](../../../functional-analysis.md#norm), so these form an orthonormal frame. This gives the [quaternionic left-invariant frame on the three-sphere](../../../differential-geometry.md#quaternionic-left-invariant-frame-on-the-three-sphere).

For any [Lie group](../../../lie-theory.md#lie-group) $G$ of dimension $n$, choose a [basis](../../../vector-space.md#basis) $E_1,\ldots,E_n$ of $T_eG$. [Left translations](../../../lie-theory.md#left-and-right-translation-on-a-lie-group) define

$$
X_i(g)=(dL_g)_eE_i.
$$

These fields are smooth; at every $g$, the differential of the [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) $L_g$ is invertible, so they are a [basis](../../../vector-space.md#basis) of $T_gG$. Hence **every [Lie group](../../../lie-theory.md#lie-group) manifold is [parallelizable](../../../differential-geometry.md#parallelizable-manifold)**, as in [parallelization of a Lie group by left translations](../../../lie-theory.md#parallelization-of-a-lie-group-by-left-translations).

For a real [semisimple Lie group](../../../lie-theory.md#semisimple-lie-group), let $B(X,Y)=\operatorname{tr}(\operatorname{ad}X\operatorname{ad}Y)$ be the [Killing form](../../../lie-algebra.md#killing-form). It is nondegenerate and invariant under the adjoint action. Left translating $B$ gives a [bi-invariant pseudo-Riemannian metric](../../../lie-theory.md#bi-invariant-pseudo-riemannian-metric). For left-invariant fields, the [Koszul formula](../../../fiber-bundle.md#koszul-formula) reduces to

$$
2B(\nabla_XY,Z)
=B([X,Y],Z)-B([Y,Z],X)+B([Z,X],Y)
=B([X,Y],Z).
$$

Thus $\nabla_XY=[X,Y]/2$. The curvature convention of Question 1 gives

$$
\begin{aligned}
R(X,Y)Z
&=\frac14[X,[Y,Z]]-\frac14[Y,[X,Z]]-\frac12[[X,Y],Z]\\
&=-\frac14[[X,Y],Z].
\end{aligned}
$$

To obtain the [Ricci tensor](../../../general-relativity.md#ricci-tensor), trace the [linear map](../../../vector-space.md#linear-map) $X\mapsto R(X,Y)Z$. Since $[[X,Y],Z]=\operatorname{ad}Z\,\operatorname{ad}Y\,X$,

$$
\boxed{\operatorname{Ric}(Y,Z)=-\frac14B(Y,Z)=-\frac14g(Y,Z).}
$$

This proves the [Killing-form Einstein metric](../../../lie-theory.md#killing-form-einstein-metric) construction for every real [semisimple group](../../../lie-theory.md#semisimple-lie-group). If $G$ is compact semisimple, $-B$ is positive definite and its [Ricci tensor](../../../general-relativity.md#ricci-tensor) is $-\tfrac14B=\tfrac14g$, giving a Riemannian [Einstein metric](../../../second-fundamental-form.md#einstein-metric). For a noncompact [semisimple group](../../../lie-theory.md#semisimple-lie-group) the general Killing-form construction is indefinite. Thus the unrestricted assertion is understood in the pseudo-Riemannian sense appropriate here; positive definiteness is not obtained by simply taking $-B$ in the noncompact case.

## 5

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The two unheaded requests are addressed here; the individual group-cover calculations are in the scoped parts below. A [quaternion](../../../algebra.md#quaternion) $q=a+bi+cj+dk$ has [norm](../../../functional-analysis.md#norm) $|q|^2=a^2+b^2+c^2+d^2$. Thus the [unit quaternions](../../../algebra.md#unit-quaternion) form exactly the sphere $S^3\subset\mathbb R^4$, with [quaternion](../../../algebra.md#quaternion) multiplication giving its smooth group structure. The explicit identification with the [special unitary group](../../../topological-group.md#special-unitary-group) $SU(2)$ is

$$
q\longmapsto
\begin{pmatrix}
a+ib&c+id\\
-c+id&a-ib
\end{pmatrix}.
$$

The [matrices](../../../vector-space.md#matrix) representing $i,j,k$ satisfy the [quaternion](../../../algebra.md#quaternion) multiplication relations. The displayed [matrix](../../../vector-space.md#matrix) obeys $U^\dagger U=|q|^2I$ and $\det U=|q|^2$; conversely every $SU(2)$ [matrix](../../../vector-space.md#matrix) has that form with $|q|=1$. Hence **$S^3$ is the manifold of [unit quaternions](../../../algebra.md#unit-quaternion), and its group is $SU(2)$**.

For the [exterior-square double cover of SO(3,3)](../../../semisimple-lie-algebra.md#exterior-square-double-cover-of-so-3-3), fix a [basis](../../../vector-space.md#basis) $e_1,\ldots,e_4$ and volume element $v=e_1\wedge e_2\wedge e_3\wedge e_4$. Define the symmetric bilinear form $Q$ on the six-dimensional exterior square by

$$
\alpha\wedge\beta=Q(\alpha,\beta)v.
$$

It is symmetric because [two-forms](../../../differential-form.md#2-form) commute under the [wedge product](../../../linear-algebra.md#exterior-product). Put

$$
a_1=e_1\wedge e_2,\quad a_2=e_1\wedge e_3,\quad a_3=e_1\wedge e_4,\qquad
b_1=e_3\wedge e_4,\quad b_2=-e_2\wedge e_4,\quad b_3=e_2\wedge e_3.
$$

Then $Q(a_i,a_j)=Q(b_i,b_j)=0$ and $Q(a_i,b_j)=\delta_{ij}$. The Gram [matrix](../../../vector-space.md#matrix) is $\begin{pmatrix}0&I_3\\I_3&0\end{pmatrix}$: the vectors $(a_i+b_i)/\sqrt2$ have [norm](../../../functional-analysis.md#norm) $+1$, while $(a_i-b_i)/\sqrt2$ have [norm](../../../functional-analysis.md#norm) $-1$. Therefore **the quadratic form $\omega\mapsto\omega\wedge\omega$ has signature $(3,3)$**.

For $A\in SL(4,\mathbb R)$,

$$
(\Lambda^2A\,\alpha)\wedge(\Lambda^2A\,\beta)
=\Lambda^4A(\alpha\wedge\beta)=\alpha\wedge\beta.
$$

Thus $\rho(A)=\Lambda^2A$ preserves $Q$. The [special linear group](../../../group-theory.md#special-linear-group) is connected: [polar decomposition of an invertible real matrix](../../../linear-algebra.md#polar-decomposition-of-an-invertible-real-matrix) writes $A=OP$ with $O\in SO(4)$ and $P$ positive definite of [determinant](../../../linear-algebra.md#determinant) one, and both factors can be joined to the identity. The image consequently lies in $SO_0(3,3)$.

If $\Lambda^2A=I$, then $Au\wedge Aw=u\wedge w$ for every pair, so $A$ preserves every two-plane. A line is an intersection of two such planes, hence every line is preserved. A [linear map](../../../vector-space.md#linear-map) preserving every line is scalar: apply it to [basis](../../../vector-space.md#basis) vectors and then to their pairwise sums. Thus $A=\lambda I$, and $\Lambda^2A=I$ forces $\lambda^2=1$. The kernel is exactly $\{\pm I\}$. It is discrete, so the derivative of $\rho$ is injective. Both [Lie algebras](../../../lie-algebra.md) have dimension $15$, making the image open; an open subgroup of a connected group is the whole group. Hence

$$
\boxed{SO_0(3,3)\cong SL(4,\mathbb R)/\{\pm I\}.}
$$

The identity-component restriction is essential. The same principle of an explicit form-preserving representation, kernel calculation and dimension argument supplies the five remaining covers.

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Identify $\mathbb R^4$ with the [quaternions](../../../algebra.md#quaternion), and use the identification of [unit quaternions](../../../algebra.md#unit-quaternion) with $SU(2)$ proved in the root Solution. The action

$$
(q_L,q_R):v\longmapsto q_Lvq_R^{-1}
$$

preserves the Euclidean [norm](../../../functional-analysis.md#norm) by multiplicativity of [quaternion](../../../algebra.md#quaternion) [norms](../../../functional-analysis.md#norm). It is a homomorphism $SU(2)\times SU(2)\to SO(4)$: its domain is connected, so the orthogonal image has [determinant](../../../linear-algebra.md#determinant) $+1$.

An element in the kernel fixes $v=1$, giving $q_L=q_R=q$. Fixing every other $v$ means $q$ commutes with all [quaternions](../../../algebra.md#quaternion), so $q$ is real; since it has unit [norm](../../../functional-analysis.md#norm), $q=\pm1$. Hence the kernel is the diagonal subgroup $\{(1,1),(-1,-1)\}$.

The differential acts as $v\mapsto av-vb$ for imaginary [quaternions](../../../algebra.md#quaternion) $a,b$. If it vanishes, $v=1$ gives $a=b$, and commutation with all $v$ makes $a$ real and imaginary, hence zero. The differential is injective, and both [Lie algebras](../../../lie-algebra.md) have dimension six. The image is therefore an open subgroup of connected $SO(4)$, hence all of $SO(4)$. Thus

$$
\boxed{SO(4)\cong\bigl(SU(2)\times SU(2)\bigr)/\mathbb Z_2,}
$$

where $\mathbb Z_2$ acts diagonally, not separately on the two factors.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Identify a Minkowski vector $(t,x,y,z)$ with the [Hermitian matrix representation of Minkowski four-vectors](../../../special-relativity.md#hermitian-matrix-representation-of-minkowski-four-vectors)

$$
X=\begin{pmatrix}t+z&x-iy\\x+iy&t-z\end{pmatrix},\qquad
\det X=t^2-x^2-y^2-z^2.
$$

For $A\in SL(2,\mathbb C)$, the real-linear action $X\mapsto AXA^\dagger$ preserves Hermiticity and the [determinant](../../../linear-algebra.md#determinant), so it preserves the Lorentz quadratic form. It also preserves the cone of positive-definite [Hermitian matrices](../../../hilbert-space.md#hermitian-operator), hence the future timelike cone. The group $SL(2,\mathbb C)$ is connected, by [polar decomposition of an invertible complex matrix](../../../linear-algebra.md#polar-decomposition-of-an-invertible-complex-matrix) into $SU(2)$ and positive determinant-one [Hermitian matrices](../../../hilbert-space.md#hermitian-operator). Thus its image lies in the [Proper orthochronous Lorentz group](../../../special-relativity.md#proper-orthochronous-lorentz-group).

If $AXA^\dagger=X$ for every Hermitian $X$, taking $X=I$ makes $A$ unitary; the remaining equations then say it commutes with every [Hermitian matrix](../../../hilbert-space.md#hermitian-operator). Their real span is all [Hermitian matrices](../../../hilbert-space.md#hermitian-operator) and their complex span is all complex [matrices](../../../vector-space.md#matrix), so $A$ is scalar. The [determinant](../../../linear-algebra.md#determinant) condition leaves precisely $A=\pm I$. A discrete kernel gives an injective differential, and the real dimensions of both groups are six. The image is therefore open and equals the connected [Lorentz group](../../../special-relativity.md#lorentz-group):

$$
\boxed{SO_0(3,1)\cong SL(2,\mathbb C)/\{\pm I\}.}
$$

The quotient does not include the disconnected time-reversing component of $SO(3,1)$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The space of real $2\times2$ [matrices](../../../vector-space.md#matrix) has a [determinant](../../../linear-algebra.md#determinant) form of signature $(2,2)$: write

$$
X=\begin{pmatrix}u+x&y+v\\y-v&u-x\end{pmatrix},
\qquad \det X=u^2+v^2-x^2-y^2.
$$

The action $(A,B):X\mapsto AXB^{-1}$ of $SL(2,\mathbb R)\times SL(2,\mathbb R)$ preserves this [determinant](../../../linear-algebra.md#determinant). Each factor is connected by [polar decomposition of an invertible real matrix](../../../linear-algebra.md#polar-decomposition-of-an-invertible-real-matrix): its orthogonal factor lies in connected $SO(2)$ and its positive factor is an exponential of a symmetric [traceless matrix](../../../linear-algebra.md#traceless-matrix). Thus the image is contained in $SO_0(2,2)$.

If the action is trivial, $X=I$ gives $A=B$, and fixing every $X$ makes $A$ a scalar [matrix](../../../vector-space.md#matrix). [Determinant](../../../linear-algebra.md#determinant) one gives $A=B=\pm I$. The kernel is therefore the diagonal $\mathbb Z_2$. Its discreteness makes the differential injective; domain and target both have dimension six. An open subgroup of connected $SO_0(2,2)$ is the whole group, so

$$
\boxed{SO_0(2,2)\cong\bigl(SL(2,\mathbb R)\times SL(2,\mathbb R)\bigr)/\mathbb Z_2.}
$$

Again the kernel is diagonal, and the target is the [identity component](../../../geometry-and-topology.md#identity-component).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

The imaginary [quaternions](../../../algebra.md#quaternion) form Euclidean $\mathbb R^3$. Conjugation by a [unit quaternion](../../../algebra.md#unit-quaternion) acts by

$$
v\longmapsto qvq^{-1}.
$$

It preserves the imaginary subspace and its [norm](../../../functional-analysis.md#norm), and continuity from $q=1$ gives [determinant](../../../linear-algebra.md#determinant) $+1$. The kernel consists of [quaternions](../../../algebra.md#quaternion) commuting with all imaginary [quaternions](../../../algebra.md#quaternion), hence is $\{\pm1\}$.

For a unit imaginary [quaternion](../../../algebra.md#quaternion) $n$, take $q=\cos(\theta/2)+n\sin(\theta/2)$. If $v$ is perpendicular to $n$, [quaternion](../../../algebra.md#quaternion) multiplication gives

$$
qvq^{-1}=v\cos\theta+(n\times v)\sin\theta,
$$

while the component parallel to $n$ is unchanged. This produces the rotation through angle $\theta$ about axis $n$, and every element of $SO(3)$ has such an axis-angle description. The map is surjective, yielding

$$
\boxed{SO(3)\cong SU(2)/\{\pm I\}.}
$$

The half-angle also explains why $q$ and $-q$ give the same rotation.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Use the real three-dimensional space of traceless [matrices](../../../vector-space.md#matrix)

$$
X=\begin{pmatrix}x&t+y\\-t+y&-x\end{pmatrix},
\qquad \det X=t^2-x^2-y^2.
$$

Thus $-\det X$ is a quadratic form of signature $(2,1)$. The adjoint action $X\mapsto AXA^{-1}$ of $SL(2,\mathbb R)$ preserves trace and [determinant](../../../linear-algebra.md#determinant). Connectedness puts its image in $SO_0(2,1)$.

A kernel element commutes with every [traceless matrix](../../../linear-algebra.md#traceless-matrix) and with the identity, hence with every real [matrix](../../../vector-space.md#matrix); it is therefore scalar. [Determinant](../../../linear-algebra.md#determinant) one leaves $\pm I$. The derivative is injective and both groups have dimension three, so the image is open and equals the [identity component](../../../geometry-and-topology.md#identity-component). Consequently

$$
\boxed{SO_0(2,1)\cong SL(2,\mathbb R)/\{\pm I\}.}
$$

## 6

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

The [Marsden-Weinstein theorem](../../../symplectic-geometry.md#marsden-weinstein-theorem) needs a [Hamiltonian action](../../../symplectic-geometry.md#hamiltonian-group-action), not merely an action by [symplectomorphisms](../../../symplectic-geometry.md#symplectomorphism). Assume an equivariant [moment map](../../../symplectic-geometry.md#moment-map) $\mu:P\to\mathfrak g^*$ exists, choose a coadjoint-fixed [regular value](../../../differential-geometry.md#regular-value) $a$ (zero is the usual choice), and assume the action on $C=\mu^{-1}(a)$ is free and proper. Regularity makes $C$ a [submanifold](../../../differential-geometry.md#submanifold) of codimension $g=\dim G$. Equivariance and invariance of $a$ make $C$ invariant under $G$, and freeness and properness give a smooth quotient $P'=C/G$. Thus

$$
\boxed{\dim P'=(2n-g)-g=2n-2g.}
$$

Let $\iota:C\hookrightarrow P$ and $\pi:C\to P'$. For $v\in T_pC$ and $\xi\in\mathfrak g$,

$$
\omega(\xi_P,v)=d\mu_\xi(v)=0.
$$

Moreover the conormal of $C$ is spanned by the independent $d\mu_\xi$, so nondegeneracy of $\omega$ gives $(T_pC)^\omega=\{\xi_P(p)\}$. The coadjoint-fixed value makes these orbit directions tangent to $C$. Hence the kernel of $\iota^*\omega$ is exactly the orbit tangent space. The restricted form is invariant and horizontal, so descends uniquely to a [two-form](../../../differential-form.md#2-form) $\omega'$ with

$$
\boxed{\pi^*\omega'=\iota^*\omega.}
$$

It is closed because $\omega$ is closed. If a quotient tangent vector annihilates $\omega'$, any lift lies in the kernel just identified and is vertical; the quotient vector is therefore zero. This proves nondegeneracy and completes [symplectic reduction](../../../symplectic-geometry.md#symplectic-reduction).

If the action is not free, singular strata or orbifold phenomena may occur. At a general noncentral [regular value](../../../differential-geometry.md#regular-value) one quotients by its coadjoint stabilizer $G_a$, not by all of $G$; the regular dimension is $2n-g-\dim G_a$. These are genuine hypotheses behind the stated dimension formula.

Both proposed examples can be given explicitly. For [symplectic reduction of an isotropic oscillator](../../../symplectic-geometry.md#symplectic-reduction-of-an-isotropic-oscillator), take two modes with

$$
\omega=\sum_{j=1}^2dq_j\wedge dp_j,\qquad
H=\frac12\sum_{j=1}^2(q_j^2+p_j^2),\qquad z_j=q_j+ip_j.
$$

Its [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) is $z_j\mapsto e^{-it}z_j$, a circle action with [moment map](../../../symplectic-geometry.md#moment-map) $H$. For $E>0$, $H^{-1}(E)$ is the sphere $S^3$ of radius $\sqrt{2E}$, and the action is free. The [Hopf fibration](../../../algebraic-topology.md#hopf-fibration) identifies its quotient with $\mathbb{CP}^1\cong S^2$. On the chart $z_1\ne0$, use $w=z_2/z_1$ and choose a section with $z_1=\sqrt{2E/(1+|w|^2)}$ real positive. Pulling back $\omega$ to this section gives

$$
\boxed{\omega'=\frac{iE\,dw\wedge d\bar w}{(1+|w|^2)^2}.}
$$

Writing $w=x+iy$ gives $2E\,dx\wedge dy/(1+x^2+y^2)^2$, whose integral is $2\pi E$. This is the [Fubini-Study form](../../../complex-geometry.md#fubini-study-form) scaled by $E$ in the convention of area $2\pi$ at unit scale. The reduced dimension is $4-2=2$. At $E=0$, the circle fixes the origin and the smooth regular-level hypotheses fail.

For a unit-mass free particle in the plane, use the rotation circle action with angular-momentum [moment map](../../../symplectic-geometry.md#moment-map) $\ell=xp_y-yp_x$. Choose $\ell_0\ne0$ so the entire level avoids $r=0$ and the action is free. Polar canonical coordinates have

$$
p_x\,dx+p_y\,dy=p_r\,dr+\ell\,d\theta,\qquad
\omega=dr\wedge dp_r+d\theta\wedge d\ell.
$$

Fixing $\ell=\ell_0$ and quotienting the rotation angle leaves

$$
\boxed{P'=T^*\mathbb R_{>0},\qquad\omega'=dr\wedge dp_r,\qquad
H'=\frac12p_r^2+\frac{\ell_0^2}{2r^2}.}
$$

This [planar rotational symplectic reduction](../../../symplectic-geometry.md#planar-rotational-symplectic-reduction) replaces a planar free trajectory by radial motion with the centrifugal potential. A nonzero moment value is allowed because the circle is abelian and every value is coadjoint-fixed.

## 7

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

[Geometric quantization](../../../symplectic-geometry.md#geometric-quantization) starts from a classical [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) $(P,\omega)$ and seeks a [Hilbert space](../../../hilbert-space.md) and quantum observables that reflect its geometry. It has two distinct stages: [prequantization](../../../symplectic-geometry.md#prequantization), which represents the full [Poisson algebra](../../../algebra.md#poisson-algebra) on sections of a [line bundle](../../../ringed-space.md#line-bundle), and a choice of [polarization in geometric quantization](../../../symplectic-geometry.md#polarization-in-geometric-quantization), which reduces the excessive phase-space dependence of those sections.

Use the conventions $\iota_{X_f}\omega=df$ and $\{f,g\}=\omega(X_f,X_g)$. A [prequantum line bundle](../../../symplectic-geometry.md#prequantum-line-bundle) is a Hermitian [line bundle](../../../ringed-space.md#line-bundle) $L\to P$ with unitary connection of curvature

$$
F_\nabla=\frac{i}{\hbar}\omega.
$$

Existence requires

$$
\boxed{\frac1{2\pi\hbar}\int_\Sigma\omega\in\mathbb Z}
$$

for every closed integral two-cycle $\Sigma$, equivalently integrality of the symplectic [cohomology class](../../../cohomology.md#cohomology-class). Necessity follows from the integral curvature periods of a unitary [line bundle](../../../ringed-space.md#line-bundle); conversely an integral class defines such a bundle, and one adjusts its connection to give the specified curvature. This is a restriction on the classical system, not a choice of local coordinates. For an exact cotangent [symplectic form](../../../symplectic-geometry.md#symplectic-form) $\omega=-d\theta$, with $\theta=p_jdq_j$, the bundle can be trivial and a connection is $\nabla=d-i\theta/\hbar$. On a sphere with [symplectic area](../../../symplectic-geometry.md#symplectic-area) $4\pi s$, the condition becomes $2s/\hbar\in\mathbb Z$. The sign of the curvature convention changes if one changes the Hamiltonian-vector-field convention or uses the dual bundle; the integrality condition is unaffected.

The [Kostant-Souriau prequantum operator](../../../symplectic-geometry.md#kostant-souriau-prequantum-operator) for a real observable is

$$
\widehat f=-i\hbar\nabla_{X_f}+f.
$$

Its derivative part describes the classical [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) and the multiplication term corrects the bracket. Indeed,

$$
[X_f,X_g]=-X_{\{f,g\}},\qquad
[\nabla_{X_f},\nabla_{X_g}]
=-\nabla_{X_{\{f,g\}}}+\frac{i}{\hbar}\{f,g\}.
$$

Since $X_f(g)=-\{f,g\}$, expanding the operator [commutator](../../../lie-algebra.md#commutator) gives

$$
\boxed{[\widehat f,\widehat g]=i\hbar\,\widehat{\{f,g\}},\qquad \widehat1=I.}
$$

With the Hermitian bundle metric and [Liouville measure](../../../symplectic-geometry.md#symplectic-volume-form), these operators are formally symmetric for real $f$ because [Hamiltonian flows](../../../classical-mechanics.md#hamiltonian-flow) preserve [symplectic volume](../../../symplectic-geometry.md#symplectic-volume). On noncompact spaces, domains and self-adjointness still require attention; the algebraic identity initially holds on an appropriate common smooth domain.

[Prequantization](../../../symplectic-geometry.md#prequantization) alone is too large. Sections depend on $2n$ phase-space variables, and the [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation) are represented reducibly. A polarization is an involutive maximal isotropic distribution $\mathcal F\subset T_{\mathbb C}P$ of complex rank $n$. Polarized sections satisfy

$$
\nabla_Ys=0\qquad(Y\in\mathcal F).
$$

The curvature vanishes on pairs of polarization vectors because $\omega|_{\mathcal F}=0$, and involutivity makes the equations locally compatible. A real polarization is tangent to a [Lagrangian foliation](../../../symplectic-geometry.md#lagrangian-foliation). A complex polarization in a [Kähler manifold](../../../complex-geometry.md#kahler-manifold) chooses one complex tangent type. With the curvature sign used here, choose the holomorphic tangent distribution, giving antiholomorphic wavefunctions. The conjugate line-bundle and sign convention gives the more usual holomorphic description.

For $T^*Q$, the vertical real polarization is spanned locally by $\partial_{p_j}$. Since the canonical [one-form](../../../differential-form.md#one-form) has no vertical component, its polarized sections are functions of $q$ alone. In the above trivialization,

$$
\widehat f=-i\hbar X_f+f-\theta(X_f),\qquad
\boxed{\widehat q_j=q_j,\qquad \widehat p_j=-i\hbar\partial_{q_j}.}
$$

One does not simply integrate these states over every momentum to retain the prequantum [norm](../../../functional-analysis.md#norm): they are constant along noncompact polarization leaves and that integral would diverge. The polarized inner product instead uses the configuration-space measure or an intrinsic [half-density](../../../ringed-space.md#half-density) description. This recovers the Schrödinger realization.

Only observables whose [Hamiltonian flows](../../../classical-mechanics.md#hamiltonian-flow) preserve $\mathcal F$ act directly on the polarized space. For example, the free-particle flow generated by $p^2/2$ sends vertical tangent vectors into directions with a configuration-space component, so its raw prequantum operator does not preserve the vertical polarization. To obtain the usual kinetic operator one needs an additional procedure, such as transporting the polarization and pairing back, rather than pretending every classical observable restricts automatically. The [Blattner-Kostant-Sternberg pairing](../../../symplectic-geometry.md#blattner-kostant-sternberg-pairing) and related projection methods address this problem. The impossibility of quantizing all classical observables with every desired algebraic property is another reason to specify the admissible observable algebra.

A [metaplectic correction](../../../symplectic-geometry.md#metaplectic-correction) tensors $L$ with a square root of the polarization's canonical [determinant](../../../linear-algebra.md#determinant) bundle when such a square root exists. These half-forms make the pairing more intrinsic and supply corrections to operator transport. They account for familiar Maslov and zero-point shifts; their existence is an extra topological condition. For a flat phase plane, take $z=q+ip$ and replace $\theta=p\,dq$ by the gauge-equivalent $\theta_s=(p\,dq-q\,dp)/2$. Then

$$
\nabla=d+\frac{\bar z\,dz-z\,d\bar z}{4\hbar},\qquad
\nabla_{\partial_z}s=0
\quad\Longrightarrow\quad
s=e^{-|z|^2/(4\hbar)}f(\bar z).
$$

The antiholomorphic function therefore has Gaussian [norm](../../../functional-analysis.md#norm), the complex-conjugate [Bargmann-Fock space](../../../hilbert-space.md#bargmann-fock-space). This explicit calculation fixes which polarization matches our curvature sign. Choosing the opposite tangent type with the same sign would give growing Gaussian sections, not the desired [Hilbert space](../../../hilbert-space.md). On compact positive [Kähler](../../../complex-geometry.md#kahler-manifold) examples, the corresponding holomorphic description (or its conjugate in these conventions) gives finite-dimensional state spaces.

Finding a suitable polarization is therefore a substantial part of the construction. A globally smooth real [Lagrangian foliation](../../../symplectic-geometry.md#lagrangian-foliation) may fail to exist; for example a regular real polarization on $S^2$ would require a line field that its tangent topology forbids. Singular foliations and noncompact leaves complicate both states and inner products. Although the restricted prequantum connection is locally flat on a Lagrangian leaf, a global nonzero parallel section requires trivial [holonomy](../../../fiber-bundle.md#holonomy). In an integrable system this selects the [Bohr-Sommerfeld quantization](../../../quantum-mechanics.md#bohr-sommerfeld-quantization) leaves; including the [half-form correction](../../../symplectic-geometry.md#metaplectic-correction) gives the familiar action condition

$$
\oint\theta=2\pi\hbar\left(n+\frac{\mu_{\mathrm{Maslov}}}{4}\right)
$$

in the usual Maslov-index convention. Complex polarizations require compatible global complex geometry and positivity. Different choices can lead to quite different realizations, and a natural unitary comparison is not automatic. Thus **integral curvature provides [prequantization](../../../symplectic-geometry.md#prequantization); polarization and its global compatibility determine the actual quantum state space**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
