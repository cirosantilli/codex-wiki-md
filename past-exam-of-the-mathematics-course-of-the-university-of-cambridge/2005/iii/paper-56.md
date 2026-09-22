# Paper 56

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper56.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper56.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The nonexistence conclusion concerns nonconstant fields: a constant [scalar-field vacuum](../../../quantum-field-theory.md#scalar-field-vacuum) with $U=0$ is a zero-energy [critical point of an energy functional](../../../calculus-of-variations.md#critical-point-of-an-energy-functional) in every dimension. Assume the potential is smooth, so the classical [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is well defined. Write the two nonnegative [energy](../../../classical-mechanics.md#energy) terms as

$$
T=\frac12\int|\nabla\phi|^2\,d^Dx,\qquad
V=\int U(\phi)\,d^Dx.
$$

For the admissible [Derrick scaling](../../../classical-field-theory-soliton.md#derrick-scaling) $\phi_\lambda(x)=\phi(\lambda x)$,

$$
E(\phi_\lambda)=\lambda^{2-D}T+\lambda^{-D}V.
$$

Stationarity at $\lambda=1$ gives the [Derrick virial identity](../../../classical-field-theory-soliton.md#derrick-virial-identity)

$$
\boxed{(2-D)T-DV=0.}
$$

For $D>2$, both terms have nonpositive sign, forcing $T=V=0$ and hence a constant vacuum. For $D=2$, scaling alone only proves $V=0$; the gradient term is scale invariant, so it must not simply be declared zero.

The [two-dimensional flat-target Derrick obstruction](../../../classical-field-theory-soliton.md#two-dimensional-flat-target-derrick-obstruction) supplies that remaining step. Since $U\geq0$ and its integral is zero, continuity gives $U(\phi(x))=0$ everywhere; smooth nonnegative $U$ has $U'(\phi(x))=0$ at those values. The field equation $\Delta\phi=U'(\phi)$ therefore becomes $\Delta\phi=0$. Each $\partial_i\phi$ is an entire [harmonic function](../../../partial-differential-equation.md#harmonic-function) in $L^2(\mathbb R^2)$. Its [mean value property](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) give, for every radius $R$,

$$
|\partial_i\phi(x_0)|
\leq\frac{\|\partial_i\phi\|_{L^2(\mathbb R^2)}}{\sqrt{\pi R^2}}.
$$

Let $R\to\infty$ to get $\partial_i\phi=0$. Thus $D=2$ also has only constant [stationary field configurations](../../../calculus-of-variations.md#critical-point-of-an-energy-functional) of finite [energy](../../../classical-mechanics.md#energy). The unconstrained real scalar target is essential in this argument; the spherical target in Question 2 has different field equations.

In $D=1$ the field equation is $\phi''=U'(\phi)$. Multiplication by $\phi'$ gives the [first integral](../../../differential-equation.md#first-integral)

$$
\frac12(\phi')^2-U(\phi)=K.
$$

Finite [energy](../../../classical-mechanics.md#energy) makes $\frac12(\phi')^2+U(\phi)$ an [integrable](../../../measure-theory.md#integrability) nonnegative function, so along some sequence $x_n\to+\infty$ it tends to zero. Evaluating the constant [first integral](../../../differential-equation.md#first-integral) on that sequence gives $K=0$. Choose

$$
\boxed{W(u)=\int_{u_*}^{u}\sqrt{2U(s)}\,ds,\qquad U(u)=\frac12(W'(u))^2.}
$$

Consequently $(\phi')^2=2U(\phi)$ and

$$
\boxed{\frac{d\phi}{dx}=\pm\frac{dW}{d\phi}.}
$$

For a nonconstant entire solution the sign is fixed. Indeed a finite-$x$ zero of $\phi'$ would have $U(\phi)=U'(\phi)=0$; uniqueness of the smooth second-order equation with initial data $(\phi,\phi')=(v,0)$ would make the solution the constant vacuum. Thus $\phi'$ never vanishes in a nonconstant solution. Conversely a smooth solution of the displayed first-order equation satisfies $\phi''=U'(\phi)$ wherever it is nonconstant.

Under the usual soliton boundary conditions $\phi(x)\to v_\pm$ as $x\to\pm\infty$, with $v_\pm$ in the [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold) $\{U=0\}$, the two endpoint components label the [topological sector](../../../classical-field-theory-soliton.md#topological-sector). For isolated [scalar-field vacua](../../../quantum-field-theory.md#scalar-field-vacuum) this is an ordered pair of vacuum labels, not necessarily one universally normalized integer. More explicitly, for any smooth $F$, the [topological current](../../../classical-field-theory-soliton.md#topological-current)

$$
j_F^\mu=\epsilon^{\mu\nu}\partial_\nu F(\phi),\qquad
\partial_\mu j_F^\mu=0,\qquad
Q_F=\int j_F^0\,dx=F(v_+)-F(v_-)
$$

is identically conserved, taking $\epsilon^{01}=1$ and boundary conditions fixed during evolution. The choices $F(u)=u$ and $F(u)=W(u)$ give the field-difference charge and the kink [energy](../../../classical-mechanics.md#energy) charge. The [square completion for a one-dimensional kink](../../../quantum-field-theory.md#square-completion-for-a-one-dimensional-kink) gives

$$
E=\frac12\int(\phi'\mp W'(\phi))^2\,dx
\pm[W(v_+)-W(v_-)],
\qquad
\boxed{E\geq|W(v_+)-W(v_-)|.}
$$

The first-order critical solution saturates this [Bogomolny bound](../../../quantum-field-theory.md#bogomolny-bound). A nonzero difference between endpoint vacuum components prevents continuous deformation to a vacuum while those boundary conditions remain fixed. Finite [energy](../../../classical-mechanics.md#energy) alone need not give finite endpoint values for arbitrary potentials, so these topological labels use the stated vacuum boundary conditions.

To evade the scalar-only obstruction, introduce a [gauge field](../../../relativistic-quantum-field.md#gauge-field) and a charged, generally multicomponent [Higgs field](../../../standard-model.md#higgs-field). For a Yang-Mills-Higgs [energy](../../../classical-mechanics.md#energy) write $E=T_H+V+E_B$, where $T_H$ contains $|D_i\Phi|^2$ and $E_B$ contains $|F_{ij}|^2$. Rescale $\Phi_\lambda(x)=\Phi(\lambda x)$ and $A_{i,\lambda}(x)=\lambda A_i(\lambda x)$. Then $D_i\Phi$ scales by $\lambda$, while $F_{ij}$ scales by $\lambda^2$, so

$$
E_\lambda=\lambda^{2-D}T_H+\lambda^{-D}V+\lambda^{4-D}E_B,
\qquad
\boxed{(2-D)T_H-DV+(4-D)E_B=0.}
$$

The magnetic term supplies the missing opposing scaling power. In $D=2$ the relation is $E_B=V$, permitting [Abelian Higgs vortices](../../../classical-field-theory-soliton.md#nielsen-olesen-vortex); in $D=3$ it is $E_B=T_H+3V$, permitting ['t Hooft-Polyakov monopoles](../../../classical-field-theory-soliton.md#t-hooft-polyakov-monopole). In the monopole Bogomolny limit $V=0$, $B_i=\pm D_i\Phi$ achieves $E_B=T_H$. Also, asymptotic ordinary derivatives need not vanish when a Higgs phase winds: the relevant vanishing quantity is the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative). This allows nontrivial boundary winding with finite [energy](../../../classical-mechanics.md#energy). Merely appending a gauge potential to a neutral one-component real field would not by itself furnish that Higgs mechanism.

## 2

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Enforce the unit-vector constraint using a [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) $\Lambda(x)$:

$$
\widetilde E=\frac12\int\left[\partial_i\phi^a\partial_i\phi^a+
\Lambda(\phi^a\phi^a-1)\right]\,d^2x.
$$

Integration by parts in a compactly supported variation gives $-\Delta\phi^a+\Lambda\phi^a=0$. Contracting with $\phi^a$ gives $\Lambda=\phi^b\Delta\phi^b$, hence

$$
\boxed{\Delta\phi^a-(\phi^b\Delta\phi^b)\phi^a=0.}
$$

Differentiating $\phi^a\phi^a=1$ twice also gives $\phi\cdot\Delta\phi=-|\nabla\phi|^2$, so an equivalent equation is $\Delta\phi+|\nabla\phi|^2\phi=0$. These are the [harmonic map](../../../differential-geometry.md#harmonic-map) equations for the [O3 nonlinear sigma model](../../../quantum-field-theory.md#o3-nonlinear-sigma-model).

For arbitrary maps, the printed finite-energy compactification assertion is too strong. The following counterexample shows that [finite sigma-model energy need not give a limit at infinity](../../../classical-field-theory-soliton.md#finite-sigma-model-energy-need-not-give-a-limit-at-infinity). Outside a large disk, set

$$
\phi(r,\vartheta)=(\sin(\log\log r),0,\cos(\log\log r)).
$$

Interpolate smoothly to a constant inside the disk. There is no angular dependence, and the exterior [energy](../../../classical-mechanics.md#energy) is

$$
\frac12\int_{r\geq R}|\nabla\phi|^2\,d^2x
=\pi\int_R^\infty\frac{dr}{r\log^2r}
=\frac{\pi}{\log R}<\infty.
$$

Nevertheless the field keeps rotating and has no limit as $r\to\infty$. Thus [energy](../../../classical-mechanics.md#energy) integrability alone does not prove a continuous map on the [one-point compactification](../../../topology.md#alexandroff-extension).

The usual [sigma-model lump](../../../quantum-field-theory.md#sigma-model-lump) sector adds the boundary condition $\phi(x)\to\phi_\infty\in S^2$ uniformly as $|x|\to\infty$. Defining the value at the added point to be $\phi_\infty$ then gives a continuous map $S^2\to S^2$: neighborhoods of the point at infinity are precisely complements of compact subsets of the plane, and uniform convergence supplies continuity there. For the [topological degree](../../../geometry-and-topology.md#topological-degree) calculation using [differential forms](../../../differential-form.md) below, take a smooth compactified map, as in the regular lump sector. This boundary/regularity information is additional to finite [energy](../../../classical-mechanics.md#energy) for unrestricted fields.

Write $a_i=\partial_i\phi$ and $b_i=\epsilon_{ij}\phi\times\partial_j\phi$. Since $\phi\cdot\partial_i\phi=0$ and $|\phi|=1$,

$$
\sum_i|b_i|^2=\sum_i|a_i|^2,\qquad
\sum_i a_i\cdot b_i=-2\,\phi\cdot(\partial_1\phi\times\partial_2\phi).
$$

Also the given double-index charge reduces to

$$
Q=\frac1{4\pi}\int
\phi\cdot(\partial_1\phi\times\partial_2\phi)\,d^2x.
$$

For $s=\pm1$, expanding the nonnegative square gives

$$
\int\sum_i|a_i+s b_i|^2\,d^2x=4E-16\pi sQ.
$$

Therefore the [Bogomolny degree bound for the O3 sigma model](../../../quantum-field-theory.md#bogomolny-degree-bound-for-the-o3-sigma-model) is

$$
\boxed{E\geq4\pi|Q|.}
$$

The charge integral is absolutely convergent already for finite-energy fields, because $|\phi\cdot(\partial_1\phi\times\partial_2\phi)|\leq\frac12(|\partial_1\phi|^2+|\partial_2\phi|^2)$. The inequality itself consequently does not need the compactification hypothesis. Equality requires $\partial_i\phi+s\epsilon_{ij}\phi\times\partial_j\phi=0$ for $s$ chosen to have the sign of $Q$.

For the topological interpretation, the standard oriented area form on the target [sphere](../../../geometry-and-topology.md#sphere) is

$$
\omega=\frac12\epsilon_{abc}y^a\,dy^b\wedge dy^c,\qquad
\int_{S^2}\omega=4\pi.
$$

Its pullback is $\phi^*\omega=\phi\cdot(\partial_1\phi\times\partial_2\phi)\,dx^1\wedge dx^2$. The [topological degree](../../../geometry-and-topology.md#topological-degree) is defined by $\phi_*[S^2]=\deg(\phi)[S^2]$ in $H_2(S^2;\mathbb Z)\cong\mathbb Z$. Pairing with $\omega$ gives

$$
\int_{S^2}\phi^*\omega=\deg(\phi)\int_{S^2}\omega,
\qquad
\boxed{Q=\deg(\phi)\in\mathbb Z.}
$$

Equivalently, the integer is the signed number of preimages of a regular value. It is invariant under smooth [homotopy](../../../algebraic-topology.md#homotopy): if $\Phi:S^2\times[0,1]\to S^2$ is that [homotopy](../../../algebraic-topology.md#homotopy), then [Stokes theorem](../../../calculus.md#stokes-theorem) and $d\omega=0$ make the difference between the two charge integrals equal to $\int_{S^2\times[0,1]}d(\Phi^*\omega)=0$. This identifies the charge as the [degree charge of an O3 sigma-model lump](../../../quantum-field-theory.md#degree-charge-of-an-o3-sigma-model-lump), rather than merely an arbitrary [energy](../../../classical-mechanics.md#energy) integral.

## 3

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use Euclidean coordinates $(x^1,x^2,x^3,x^4)$ and orientation $dx^1\wedge dx^2\wedge dx^3\wedge dx^4$. For $D_\mu=\partial_\mu+A_\mu$, the [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) is $F_{\mu\nu}=[D_\mu,D_\nu]$. The [ASDYM equations](../../../classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations) are $F=-*F$, equivalently

$$
F_{12}+F_{34}=0,\qquad F_{13}-F_{24}=0,\qquad F_{14}+F_{23}=0.
$$

Put $w=x^1+ix^2$, $z=x^3+ix^4$, with $\partial_w=(\partial_1-i\partial_2)/2$ and similarly for $z$. The bars label the complex conjugate coordinates on the Euclidean real slice; after complexification they can be treated as independent coordinates. A [Lax pair for the anti-self-dual Yang-Mills equations](../../../integrable-systems.md#lax-pair-for-the-anti-self-dual-yang-mills-equations) is

$$
\boxed{(D_w-\lambda D_{\bar z})\Psi=0,\qquad
(D_z+\lambda D_{\bar w})\Psi=0,\qquad \lambda\in\mathbb{CP}^1.}
$$

At infinity rescale the operators and use the other affine coordinate. Their [commutator](../../../lie-algebra.md#commutator) is

$$
[D_w-\lambda D_{\bar z},D_z+\lambda D_{\bar w}]
=F_{wz}+\lambda(F_{w\bar w}+F_{z\bar z})+\lambda^2F_{\bar w\bar z}.
$$

Compatibility for every $\lambda$ is therefore precisely $F_{wz}=F_{\bar w\bar z}=0$ and $F_{w\bar w}+F_{z\bar z}=0$. To verify the real component signs,

$$
F_{wz}=\frac14\{F_{13}-F_{24}-i(F_{14}+F_{23})\},\qquad
F_{w\bar w}+F_{z\bar z}=\frac i2(F_{12}+F_{34}).
$$

The conjugate equation supplies the remaining real components. This is compatibility of an overdetermined system, not an additional field equation on $\Psi$ for only one value of the [spectral parameter](../../../integrable-systems.md#spectral-parameter).

Impose invariance under translations in $x^1,x^2,x^3$, writing $t=x^4$. In a symmetry-adapted gauge the potentials depend only on $t$. A further $t$-dependent [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation) sets $A_4=0$ locally, by solving the usual [parallel transport](../../../fiber-bundle.md#parallel-transport) ordinary differential equation; it does not reintroduce spatial dependence. Then

$$
F_{ab}=[A_a,A_b],\qquad F_{a4}=-\dot A_a.
$$

The three real equations above become $\dot A_1=[A_2,A_3]$, $\dot A_2=[A_3,A_1]$ and $\dot A_3=[A_1,A_2]$, namely

$$
\boxed{\dot A_a=\frac12\epsilon_{abc}[A_b,A_c].}
$$

These are the [Nahm equations](../../../classical-field-theory-soliton.md#nahm-equations). The orientation chosen above gives the requested plus sign; reversing orientation exchanges [self-duality of gauge curvature](../../../classical-field-theory-soliton.md#self-duality-of-gauge-curvature) and [anti-self-duality of gauge curvature](../../../classical-field-theory-soliton.md#anti-self-duality-of-gauge-curvature). Translation invariance here is a local dimensional reduction and is not a claim of finite four-dimensional action over all three translation directions.

To prove conservation, abbreviate $P=A_1+iA_2$, $Q=A_1-iA_2$ and $R=A_3$, so $A(\lambda)=P+2R\lambda-Q\lambda^2$ and $B(\lambda)=-iR+iQ\lambda$. Expanding the [commutator](../../../lie-algebra.md#commutator), including the cancellation of the cubic term, gives

$$
[A(\lambda),B(\lambda)]
=-i[P,R]+i[P,Q]\lambda+i[R,Q]\lambda^2.
$$

The [Nahm equations](../../../classical-field-theory-soliton.md#nahm-equations) give

$$
\dot P=-i[P,R],\qquad
2\dot R=i[P,Q],\qquad
-\dot Q=i[R,Q].
$$

Thus the [polynomial Lax representation of the Nahm equations](../../../classical-field-theory-soliton.md#polynomial-lax-representation-of-the-nahm-equations) is

$$
\boxed{\dot A(\lambda)=[A(\lambda),B(\lambda)].}
$$

Take a finite-dimensional [matrix](../../../vector-space.md#matrix) representation of the [Lie algebra](../../../lie-algebra.md) and its complexification. For every positive integer $p$, differentiating the product and using cyclicity of the [matrix trace](../../../linear-algebra.md#matrix-trace) gives

$$
\frac d{dt}\operatorname{Tr}(A(\lambda)^p)
=p\operatorname{Tr}(A(\lambda)^{p-1}[A(\lambda),B(\lambda)])
=p\{\operatorname{Tr}(A^pB)-\operatorname{Tr}(BA^p)\}=0.
$$

This proves the [trace invariants of a Lax equation](../../../integrable-systems.md#trace-invariants-of-a-lax-equation) directly. Since $\operatorname{Tr}(A(\lambda)^p)$ is a polynomial of degree at most $2p$ in the affine coordinate $\lambda$, its derivative vanishes identically only if the derivative of every coefficient vanishes. Therefore **every trace-polynomial coefficient is independent of $t$**. At projective infinity these polynomials are sections of $\mathcal O(2p)$; they need not be constant functions of $\lambda$ on the whole projective [sphere](../../../geometry-and-topology.md#sphere).

## 4

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Represent affine [complexified Minkowski space](../../../special-relativity.md#complexified-minkowski-spacetime) by complex $2\times2$ [matrices](../../../vector-space.md#matrix) $x^{AA'}$, with the conformal metric characterized by $\det(dx)$. Let an element of [twistor space](../../../general-relativity.md#twistor-space) be $Z=(\omega^A,\pi_{A'})\in\mathbb C^4$, and identify nonzero twistors under $Z\sim cZ$, $c\ne0$. The compact [projective twistor space](../../../general-relativity.md#projective-twistor-space) is $\mathbb{CP}^3$. For affine space-time the corresponding open domain is the [affine projective twistor space](../../../general-relativity.md#affine-projective-twistor-space)

$$
\boxed{PT_{\rm aff}=\{[\omega,\pi]:\pi\ne0\}
=\mathbb{CP}^3\setminus\mathbb{CP}^1_\infty
\cong\operatorname{Tot}(\mathcal O(1)\oplus\mathcal O(1)).}
$$

Use the [twistor incidence relation](../../../general-relativity.md#twistor-incidence-relation) in the convention $\omega^A=x^{AA'}\pi_{A'}$; the more usual factor $i$ can be absorbed into the complex coordinate $x$. A point $x$ determines a [twistor line](../../../general-relativity.md#twistor-line)

$$
L_x=\{[x\pi,\pi]:[\pi]\in\mathbb{CP}^1\}\cong\mathbb{CP}^1.
$$

In the two projective charts, fibre coordinates $\omega/\pi_{0'}$ and $\omega/\pi_{1'}$ differ by division by $\lambda=\pi_{1'}/\pi_{0'}$, giving the two $\mathcal O(1)$ summands. Two distinct space-time points have intersecting lines precisely when $(x-y)\pi=0$ for some nonzero $\pi$, equivalently $\det(x-y)=0$; this recovers conformal null separation.

The [twistor correspondence](../../../general-relativity.md#twistor-correspondence) is the double fibration

$$
M_{\mathbb C}\,\xleftarrow{p}\,
\mathcal F=M_{\mathbb C}\times\mathbb{CP}^1
\ \xrightarrow{\ q\ }\ PT_{\rm aff},
\qquad q(x,[\pi])=[x\pi,\pi].
$$

For a fixed twistor, the incidence solutions form an affine [alpha-plane](../../../general-relativity.md#alpha-plane), a two-dimensional totally null plane. Its tangent distribution on $\mathcal F$ is generated by

$$
V_A=\pi^{A'}\partial_{AA'},\qquad
\pi^{A'}=\epsilon^{A'B'}\pi_{B'}.
$$

These [vector fields](../../../calculus.md#vector-field) annihilate the incidence coordinates, since $\pi^{A'}\pi_{A'}=0$, and commute. This distribution is the geometric source of the linear system in the [Penrose-Ward correspondence](../../../general-relativity.md#penrose-ward-correspondence).

For the inverse construction, take a rank-$r$ [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle) $E$ on the twistor domain corresponding to a space-time open set $U$. The crucial hypothesis is

$$
\boxed{E|_{L_x}\cong\mathcal O^{\oplus r}\quad\text{for every }x\in U.}
$$

These are [line-trivial bundles in the Ward correspondence](../../../general-relativity.md#line-trivial-bundles-in-the-ward-correspondence). It is not enough to specify an arbitrary [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle), nor just zero [First Chern class](../../../complex-geometry.md#first-chern-class) on its lines: $\mathcal O(1)\oplus\mathcal O(-1)$ has degree zero but is nontrivial. A line with a nontrivial splitting is a jumping line and does not support the regular linewise construction there. Thus a globally nonsingular field on all affine complexified space-time requires triviality on all its relevant lines; a local construction uses only the lines over $U$.

Choose [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle) [bundle frames](../../../fiber-bundle.md#frame-of-a-vector-bundle) on two twistor patches, and let $P$ be the invertible transition [matrix](../../../vector-space.md#matrix) on their overlap. Pull it back to $\mathcal F$. Because it comes from [affine projective twistor space](../../../general-relativity.md#affine-projective-twistor-space), it is constant along the $q$-fibres:

$$
V_A P(x,\pi)=0.
$$

Triviality on $L_x$ supplies a global [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) [bundle frame](../../../fiber-bundle.md#frame-of-a-vector-bundle) on that line. Comparing this global [bundle frame](../../../fiber-bundle.md#frame-of-a-vector-bundle) with the two local [bundle frames](../../../fiber-bundle.md#frame-of-a-vector-bundle) produces a [holomorphic splitting of a twistor patching matrix](../../../general-relativity.md#holomorphic-splitting-of-a-twistor-patching-matrix),

$$
P(x,\lambda)=\Psi_-(x,\lambda)^{-1}\Psi_+(x,\lambda),
$$

where $\Psi_+$ and $\Psi_-$ are [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) and invertible near the two affine patches of the [complex projective line](../../../algebraic-topology.md#complex-projective-line). The splitting can be chosen holomorphically in $x$ locally: the restrictions have $r$ independent global sections and $H^1(\mathbb{CP}^1,\mathcal O^{\oplus r})=0$, so these [bundle frames](../../../fiber-bundle.md#frame-of-a-vector-bundle) extend through a neighborhood of the given line. This explains where regularity and linewise triviality enter the construction.

Differentiate the factorization using $V_AP=0$. Multiplication by the invertible factors gives

$$
(V_A\Psi_+)\Psi_+^{-1}
=(V_A\Psi_-)\Psi_-^{-1}.
$$

Define their common negative to be $\mathcal A_A$. It is regular on both projective patches and homogeneous of degree one in $\pi$, because $V_A$ has that degree while the [bundle frames](../../../fiber-bundle.md#frame-of-a-vector-bundle) have degree zero. Consequently

$$
\mathcal A_A(x,\pi)=\pi^{A'}A_{AA'}(x).
$$

This last conclusion is elementary: on one affine chart its entries are entire in $\lambda$; regularity at infinity after dividing by the transition factor $\lambda$ allows at most linear growth, so each entry is affine in $\lambda$. Equivalently, a global section of $\mathcal O(1)$ is a linear homogeneous polynomial. We have thereby recovered a [gauge connection](../../../fiber-bundle.md#connection-vector-bundle) $D_{AA'}=\partial_{AA'}+A_{AA'}$ on the space-time bundle whose fibre is $H^0(L_x,E|_{L_x})$.

The splitting factors now obey

$$
\boxed{\pi^{A'}D_{AA'}\Psi_\pm=0.}
$$

Their invertibility implies the compatibility conditions

$$
\pi^{A'}\pi^{B'}F_{AA'BB'}=0\quad\text{for every }[\pi].
$$

In the [spinor decomposition of gauge curvature](../../../relativistic-quantum-field.md#spinor-decomposition-of-gauge-curvature),

$$
F_{AA'BB'}=\epsilon_{AB}\Phi_{A'B'}+\epsilon_{A'B'}\Phi_{AB},
$$

the two spinors are symmetric. The antisymmetric primed factor vanishes when contracted with $\pi^{A'}\pi^{B'}$, leaving $\epsilon_{AB}\pi^{A'}\pi^{B'}\Phi_{A'B'}=0$. A quadratic polynomial that vanishes for every spinor has every coefficient zero, so $\Phi_{A'B'}=0$. With the orientation convention used here, this is exactly [anti-self-duality of gauge curvature](../../../classical-field-theory-soliton.md#anti-self-duality-of-gauge-curvature), hence the [ASDYM equations](../../../classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations). This establishes the field equation from the [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) data, rather than assuming it as an extra input.

The construction naturally gives a gauge class. If another linewise splitting is chosen, $\Psi'_\pm\Psi_\pm^{-1}$ agrees on the overlap and is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on the entire compact [complex projective line](../../../algebraic-topology.md#complex-projective-line); its entries are therefore independent of $\lambda$. Write this common [matrix](../../../vector-space.md#matrix) as $g(x)^{-1}$. Then

$$
A'_{AA'}=g^{-1}A_{AA'}g+g^{-1}\partial_{AA'}g,
$$

the ordinary [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation). Changing the original [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle) [bundle frames](../../../fiber-bundle.md#frame-of-a-vector-bundle) or replacing $E$ by an isomorphic bundle produces the same space-time gauge class. A determinant trivialization or another [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) structure-group reduction gives the corresponding restriction from $GL(r,\mathbb C)$ to $SL(r,\mathbb C)$ or another complex [gauge group](../../../relativistic-quantum-field.md#gauge-group).

For perspective, the forward direction starts from an ASD [gauge connection](../../../fiber-bundle.md#connection-vector-bundle) and uses its flat [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) along each [alpha-plane](../../../general-relativity.md#alpha-plane) to descend parallel sections to [affine projective twistor space](../../../general-relativity.md#affine-projective-twistor-space). The reconstructed linear system is exactly that parallel-section system. Going back through it recovers the original line-trivial bundle, while changing space-time [bundle frames](../../../fiber-bundle.md#frame-of-a-vector-bundle) amounts to [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation). Thus, locally and with the stated regularity and triviality conditions, **[holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) line-trivial bundles determine solutions of the [ASDYM equations](../../../classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations) uniquely up to gauge**.

No unitary reality condition is imposed on [complexified Minkowski space](../../../special-relativity.md#complexified-minkowski-spacetime) in this question. Obtaining real Euclidean [gauge fields](../../../relativistic-quantum-field.md#gauge-field) requires the compatible antiholomorphic twistor involution and a bundle reality structure; obtaining finite-action instantons requires further global and boundary conditions. Those are additional restrictions on the complex correspondence, not automatic consequences of having any [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle) on [projective twistor space](../../../general-relativity.md#projective-twistor-space).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
