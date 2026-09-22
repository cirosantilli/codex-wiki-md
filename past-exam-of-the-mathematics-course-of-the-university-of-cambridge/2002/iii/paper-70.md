# Paper 70

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper70.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper70.pdf)

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

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) signature $(+,-)$ and put $\kappa=|\lambda|>0$. The [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation) for the real [scalar field](../../../quantum-field-theory.md#scalar-field) is

$$
\boxed{\phi_{tt}-\phi_{xx}+2\kappa^2\phi(\phi^2-1)=0.}
$$

Indeed, differentiating the potential $U(\phi)=\kappa^2(\phi^2-1)^2/2$ gives $U'=2\kappa^2\phi(\phi^2-1)$, while the kinetic term contributes $\partial_\mu\partial^\mu\phi$.

Translation invariance gives the symmetric [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor)

$$
T^{\mu\nu}=\partial^\mu\phi\,\partial^\nu\phi
-\eta^{\mu\nu}\mathcal L.
$$

Its divergence is $(\partial_\mu\partial^\mu\phi+U')\partial^\nu\phi$, which vanishes by the [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation). Consequently the conserved [energy](../../../classical-mechanics.md#energy) and physical spatial [momentum](../../../classical-mechanics.md#momentum) are

$$
\boxed{E=\int_{\mathbb R}\left[\frac12\phi_t^2+\frac12\phi_x^2+
\frac{\kappa^2}{2}(\phi^2-1)^2\right]dx,\qquad
P=-\int_{\mathbb R}\phi_t\phi_x\,dx.}
$$

The minus sign in $P=\int T^{01}dx$ follows from $\partial^1=-\partial_x$. Conservation assumes the associated stress-energy fluxes vanish at spatial infinity, as they do for the localized fields below.

A static [finite-energy field configuration](../../../classical-field-theory-soliton.md#finite-energy-field-configuration) approaches vacua $\phi=\pm1$. Multiplying $\phi''=U'(\phi)$ by $\phi'$ gives

$$
\frac12\phi'^2-U(\phi)=\text{constant}=0,
$$

where the vacuum limits fix the constant. For a [kink](../../../classical-field-theory-soliton.md#scalar-field-kink) increasing from $-1$ to $1$, $\phi'=\kappa(1-\phi^2)$. Integration gives $\operatorname{artanh}\phi=\kappa(x-X)$ and hence

$$
\boxed{\phi_{\mathrm K}(x)=\tanh[\kappa(x-X)].}
$$

Its negative is the [antikink](../../../classical-field-theory-soliton.md#antikink). The arbitrary center $X$ is a translational [collective coordinate](../../../classical-field-theory-soliton.md#collective-coordinate-of-a-soliton). The static [kink](../../../classical-field-theory-soliton.md#scalar-field-kink) mass is its rest [energy](../../../classical-mechanics.md#energy); using $\phi'^2=2U$ and $y=\kappa(x-X)$ gives

$$
M=\int_{\mathbb R}\phi'^2dx
=\kappa\int_{-\infty}^{\infty}\operatorname{sech}^4y\,dy
=\kappa\int_{-1}^{1}(1-z^2)\,dz
=\boxed{\frac{4\kappa}{3}}.
$$

Equivalently, completing the static [energy](../../../classical-mechanics.md#energy) into a square gives $E=\frac12\int[\phi'-\kappa(1-\phi^2)]^2dx+\kappa[\phi-\phi^3/3]_{-\infty}^{\infty}$, so this [kink](../../../classical-field-theory-soliton.md#scalar-field-kink) saturates its [Bogomolny bound](../../../quantum-field-theory.md#bogomolny-bound).

A [Lorentz boost](../../../special-relativity.md#lorentz-boost) with velocity $v$ gives

$$
\boxed{\phi(t,x)=\tanh[\kappa\gamma(x-X-vt)],
\qquad \gamma=(1-v^2)^{-1/2}.}
$$

Writing $z=\gamma(x-X-vt)$, the derivatives are $\phi_t=-\gamma v\phi_{\mathrm K}'(z)$ and $\phi_x=\gamma\phi_{\mathrm K}'(z)$. The [momentum](../../../classical-mechanics.md#momentum) integral therefore becomes

$$
P=\gamma^2v\int\phi_{\mathrm K}'(z)^2\,\frac{dz}{\gamma}
=\boxed{\gamma Mv}.
$$

The boosted [energy](../../../classical-mechanics.md#energy) is

$$
E=\frac12\left[\gamma(1+v^2)+\gamma^{-1}\right]
\int\phi_{\mathrm K}'(z)^2dz
=\boxed{\gamma M},
$$

because $\gamma^{-1}=\gamma(1-v^2)$. Thus $E^2-P^2=M^2$ and $P/E=v$, exactly the [energy–momentum relation](../../../special-relativity.md#energy-momentum-relation) of a relativistic particle of rest mass $4\kappa/3$. This is the [relativistic energy and momentum of a phi-four kink](../../../classical-field-theory-soliton.md#relativistic-energy-and-momentum-of-a-phi-four-kink). If $\lambda=0$, the double-well potential disappears and there is no localized static kink connecting these vacua.

## 2

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Bogomolny equations](../../../quantum-field-theory.md#bogomolny-equations) are first-order equations obtained by expressing a static [energy](../../../classical-mechanics.md#energy) as nonnegative squares plus a term fixed by the [topological charge](../../../classical-field-theory-soliton.md#topological-charge). Vanishing of the squares minimizes the [energy](../../../classical-mechanics.md#energy) in that [topological sector](../../../classical-field-theory-soliton.md#topological-sector). In particular, the solutions satisfy the full second-order field equations, since their first variation vanishes for compactly supported variations preserving the boundary data. Both monopole and vortex realizations illustrate this mechanism.

For a [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) with gauge group [SU(2)](../../../topological-group.md#su-2-group) and an adjoint [Higgs field](../../../standard-model.md#higgs-field) $\Phi^a$, take the static, purely magnetic [energy](../../../classical-mechanics.md#energy)

$$
E=\int_{\mathbb R^3}\left[\frac12 B_i^aB_i^a+
\frac12(D_i\Phi)^a(D_i\Phi)^a+
\frac{\lambda_H}{4}(\Phi^a\Phi^a-v_H^2)^2\right]d^3x.
$$

Here $B_i^a=\frac12\epsilon_{ijk}F_{jk}^a$, and $e$ is the gauge coupling. In the Bogomolny limit $\lambda_H=0$, retain the boundary condition $|\Phi|\to v_H>0$; it breaks [SU(2)](../../../topological-group.md#su-2-group) to [U(1)](../../../lie-theory.md#circle-group) at infinity even though the scalar potential has been removed. The normalized [Higgs field](../../../standard-model.md#higgs-field) on the sphere at infinity defines a map $S^2_\infty\to S^2$ of [topological degree](../../../geometry-and-topology.md#topological-degree) $n$. In a consistent magnetic orientation the asymptotic flux is $g_m=4\pi n/e$, and

$$
\int_{S^2_\infty}\Phi^a B_i^a\,dS_i=v_Hg_m.
$$

For example, this equality follows by projecting the asymptotic [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) on the Higgs direction: its flux is the integral of the target-sphere area form, divided by $e$.

The [gauge-theory Bianchi identity](../../../relativistic-quantum-field.md#gauge-theory-bianchi-identity) $D_iB_i=0$ makes the cross term a divergence:

$$
B_i^a(D_i\Phi)^a=\partial_i(\Phi^aB_i^a).
$$

For either sign $s=\pm1$, complete the square:

$$
E=\frac12\int_{\mathbb R^3}|B-sD\Phi|^2d^3x+
s\int_{S^2_\infty}\Phi\cdot B\,dS.
$$

Choosing $s=\operatorname{sgn}n$ gives

$$
\boxed{E\geq\frac{4\pi v_H}{e}|n|,
\qquad B_i=sD_i\Phi\ \text{at equality}.}
$$

These are the [Bogomolny-Prasad-Sommerfield monopole](../../../classical-field-theory-soliton.md#bogomolny-prasad-sommerfield-monopole) equations. A nonzero scalar potential would add a positive term; a nontrivial smooth monopole with a core cannot generally saturate this same bound at $\lambda_H>0$. The [Bogomolny monopole equations imply Yang-Mills-Higgs equations](../../../classical-field-theory-soliton.md#bogomolny-monopole-equations-imply-yang-mills-higgs-equations): the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity) already gives $D_iD_i\Phi=0$, and the square-completion argument gives stationarity with respect to the gauge field as well.

An explicit charge-one solution is furnished by the [hedgehog ansatz for a monopole](../../../classical-field-theory-soliton.md#hedgehog-ansatz-for-a-monopole). To fix its signs, use component conventions $D_i\Phi=\partial_i\Phi-eA_i\times\Phi$ and $F_{ij}=\partial_iA_j-\partial_jA_i-eA_i\times A_j$. With $\rho=ev_Hr$ and $\hat x=x/r$, put

$$
\Phi^a=v_HH(\rho)\hat x^a,\qquad
A_i^a=\frac{1-K(\rho)}{er}\epsilon_{iaj}\hat x^j.
$$

The radial and transverse parts of $D_i\Phi$ are $ev_H^2H'\hat x_i\hat x^a$ and $v_HHK(\delta_{ia}-\hat x_i\hat x^a)/r$. The corresponding parts of $B_i^a$ are $(1-K^2)\hat x_i\hat x^a/(er^2)$ and $-v_HK'(\delta_{ia}-\hat x_i\hat x^a)/r$. Therefore $B=D\Phi$ reduces to

$$
\frac{dK}{d\rho}=-KH,\qquad
\frac{dH}{d\rho}=\frac{1-K^2}{\rho^2}.
$$

The [Prasad-Sommerfield radial monopole solution](../../../classical-field-theory-soliton.md#prasad-sommerfield-radial-monopole-solution) is

$$
\boxed{K(\rho)=\frac{\rho}{\sinh\rho},\qquad
H(\rho)=\coth\rho-\frac1\rho.}
$$

Direct differentiation verifies both equations. Near $\rho=0$, $K=1-\rho^2/6+O(\rho^4)$ and $H=\rho/3+O(\rho^3)$, so the apparent angular singularities disappear and the fields are smooth. At infinity $K$ decays exponentially while $H=1-1/\rho+O(e^{-2\rho})$, leaving an Abelian $1/(er^2)$ magnetic field and mass $4\pi v_H/e$.

Translations of this [magnetic monopole](../../../physics.md#magnetic-monopole) give three [collective coordinates](../../../classical-field-theory-soliton.md#collective-coordinate-of-a-soliton); a residual [U(1)](../../../lie-theory.md#circle-group) phase provides another in the framed description, where gauge transformations are fixed at infinity. Multimonopole solutions of a common sign also saturate the linear bound. Their widely separated constituents have position and phase parameters, with no static force: the magnetic repulsion and massless-Higgs attraction cancel in this limit. Relative motion is described at low speeds by the [moduli-space approximation](../../../classical-field-theory-soliton.md#moduli-space-approximation-for-solitons). An opposite-sign monopole pair does not solve one common sign of the [Bogomolny equations](../../../quantum-field-theory.md#bogomolny-equations) and is not protected by that no-force argument.

For the [Abelian Higgs model](../../../classical-field-theory-soliton.md#abelian-higgs-model), a second realization occurs in the plane. Let $\psi$ be a complex [Higgs field](../../../standard-model.md#higgs-field), $D_i=\partial_i-ieA_i$, $B=\partial_1A_2-\partial_2A_1$, and choose the critically coupled static [energy](../../../classical-mechanics.md#energy)

$$
E=\int_{\mathbb R^2}\left[\frac12B^2+|D_i\psi|^2+
\frac{e^2}{2}(|\psi|^2-v_H^2)^2\right]d^2x.
$$

Different conventions for the scalar kinetic coefficient change the numerical coefficients of both the bound and the equations. This normalization gives scalar and gauge masses $\sqrt2ev_H$, explaining the critical balance of their long-distance forces. In three spatial dimensions the planar solutions describe straight strings with this [energy](../../../classical-mechanics.md#energy) per unit length.

Finite [energy](../../../classical-mechanics.md#energy) requires $|\psi|\to v_H$ and $D_i\psi\to0$. On a large circle the Higgs phase winds by $2\pi n$, so the [magnetic flux quantization of an Abelian Higgs vortex](../../../classical-field-theory-soliton.md#magnetic-flux-quantization-of-an-abelian-higgs-vortex) gives

$$
\Phi_B=\int B\,d^2x=\oint A_i\,dx^i=\frac{2\pi n}{e}.
$$

Writing $J_i=\operatorname{Im}(\bar\psi D_i\psi)$, expansion and integration by parts give

$$
|D_1\psi|^2+|D_2\psi|^2
=|(D_1+iD_2)\psi|^2+eB|\psi|^2+
\partial_1J_2-\partial_2J_1.
$$

The divergence integrates to zero for the usual localized vortex boundary conditions. Thus the [Bogomolny square completion for an Abelian Higgs vortex](../../../classical-field-theory-soliton.md#bogomolny-square-completion-for-an-abelian-higgs-vortex) is

$$
E=\int_{\mathbb R^2}\left[
|(D_1+iD_2)\psi|^2+
\frac12\{B-e(v_H^2-|\psi|^2)\}^2\right]d^2x
+ev_H^2\Phi_B.
$$

For $n\geq0$ the [Bogomolny vortex equations](../../../classical-field-theory-soliton.md#bogomolny-vortex-equation) and bound are

$$
\boxed{(D_1+iD_2)\psi=0,\quad
B=e(v_H^2-|\psi|^2),\quad E=2\pi v_H^2n.}
$$

For $n<0$, reverse the sign in both first-order equations and obtain $E=2\pi v_H^2|n|$.

For a rotationally symmetric positive [vortex number](../../../classical-field-theory-soliton.md#vortex-number), use $\psi=v_H f(r)e^{in\theta}$ and the physical angular component $A_\theta=na(r)/(er)$. The [Bogomolny vortex equations](../../../classical-field-theory-soliton.md#bogomolny-vortex-equation) become

$$
f'=\frac{n(1-a)}r f,\qquad
a'=\frac{e^2v_H^2r}{n}(1-f^2),
$$

with $f(0)=a(0)=0$ and $f(\infty)=a(\infty)=1$. The regular core behaves as $f\sim cr^n$ and $a\sim e^2v_H^2r^2/(2n)$. Linearization at infinity gives exponentially decaying massive tails. Unlike the radial monopole, these planar radial profiles have no elementary closed form in general.

The general multi-vortex solution can be encoded by the [Taubes equation](../../../classical-field-theory-soliton.md#taubes-equation). Away from zeros, write $\psi=v_He^{h/2+i\chi}$. The first equation gives

$$
A_1=\frac1e\left(\partial_1\chi+\frac12\partial_2h\right),\qquad
A_2=\frac1e\left(\partial_2\chi-\frac12\partial_1h\right).
$$

At zeros $z_a$ of multiplicity $m_a$, the phase contributes circulation $2\pi m_a$. The second equation becomes, including these [Dirac delta](../../../distribution-theory.md#dirac-delta-function) terms,

$$
\Delta h+2e^2v_H^2(1-e^h)
=4\pi\sum_a m_a\delta^{(2)}(x-z_a),\qquad h\to0\ \text{at infinity}.
$$

For prescribed zeros the planar existence result gives a solution; the [prescribed-zero construction of planar Abelian Higgs vortices](../../../classical-field-theory-soliton.md#prescribed-zero-construction-of-planar-abelian-higgs-vortices) reconstructs smooth fields, with $h=2m_a\log|x-z_a|+O(1)$ near each zero. Uniqueness is visible directly: for two solutions with the same zeros, their nonsingular difference $w$ satisfies $\Delta w=2e^2v_H^2(e^{h_1}-e^{h_2})$. Multiplying by $w$ and integrating gives

$$
-\int|\nabla w|^2d^2x
=2e^2v_H^2\int w(e^{h_1}-e^{h_2})\,d^2x\geq0,
$$

hence $w=0$. The [Abelian Higgs vortex moduli space](../../../classical-field-theory-soliton.md#abelian-higgs-vortex-moduli-space) has arbitrary unordered positions of the $n$ zeros, giving $2n$ real position parameters. The saturated [energy](../../../classical-mechanics.md#energy) is independent of their positions, so critically coupled vortices have no static interaction energy. Away from critical coupling this cancellation is lost.

## 3

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [topological degree](../../../geometry-and-topology.md#topological-degree) assigns an integer to a continuous map $f:M\to N$ between closed, connected, oriented manifolds of the same dimension $d$. Their top [homology groups](../../../homology.md#homology-group) are infinite cyclic, generated by their [fundamental classes](../../../cohomology.md#fundamental-class). The induced map defines

$$
\boxed{f_*[M]=(\deg f)[N],\qquad \deg f\in\mathbb Z.}
$$

For a smooth map and a [regular value](../../../differential-geometry.md#regular-value) $y$, its equivalent local description is

$$
\deg f=\sum_{x\in f^{-1}(y)}\operatorname{sgn}\det(df_x),
$$

where the sign records preservation or reversal of orientation. The preimage is a finite set because the manifolds are compact and $y$ is regular. This is a signed count; opposite-orientation preimages cancel. If $\omega$ is a normalized target [volume form](../../../differential-form.md#volume-form) with $\int_N\omega=1$, the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) gives the equivalent integral $\deg f=\int_Mf^*\omega$.

The [homotopy invariance of mapping degree](../../../homology.md#homotopy-invariance-of-mapping-degree) follows because homotopic maps induce the same homology map. In the smooth description, apply [Stokes theorem](../../../calculus.md#stokes-theorem) to a homotopy $F:M\times[0,1]\to N$:

$$
\int_Mf_1^*\omega-\int_Mf_0^*\omega
=\int_{M\times[0,1]}d(F^*\omega)=0,
$$

since a top-dimensional form on $N$ is closed. Thus degree cannot change during a smooth deformation preserving the relevant boundary conditions. Degrees multiply under composition, and a nonzero-degree map is surjective: a missed target point would give a regular value with an empty preimage and hence degree zero.

For maps $S^d\to S^d$, the [homotopy group](../../../algebraic-topology.md#homotopy-group) $\pi_d(S^d)=\mathbb Z$ is completely detected by degree. This supplies integer [topological sectors](../../../classical-field-theory-soliton.md#topological-sector) for many [classical field-theory solitons](../../../classical-field-theory-soliton.md). It is important to distinguish two ways spheres arise. In a [nonlinear sigma model](../../../quantum-field-theory.md#nonlinear-sigma-model) with the field approaching one fixed target value at infinity, compactify all of $\mathbb R^d$ to $S^d$ and classify the resulting map into the target. For a defect whose vacuum field varies with direction, retain the sphere $S^{d-1}_\infty$ surrounding the core and map it into the [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold). This is the [vacuum-boundary degree as a defect charge](../../../classical-field-theory-soliton.md#vacuum-boundary-degree-as-a-defect-charge). An asymptotic limit is a boundary hypothesis; finite energy alone in every possible model need not imply one.

For an [Abelian Higgs vortex](../../../classical-field-theory-soliton.md#nielsen-olesen-vortex), the phase at infinity defines $S^1\to U(1)\cong S^1$. Its degree is the [winding number](../../../complex-analysis.md#winding-number)

$$
n=\frac1{2\pi}\oint d\chi
=\frac e{2\pi}\int B\,d^2x.
$$

Nonzero $n$ forces a zero of the Higgs field inside: a nowhere-vanishing field would extend its normalized phase through the disk and make the boundary loop contractible. This is also the flux classification of the [Bogomolny vortex equations](../../../classical-field-theory-soliton.md#bogomolny-vortex-equation).

For a ['t Hooft-Polyakov monopole](../../../classical-field-theory-soliton.md#t-hooft-polyakov-monopole), the normalized adjoint [Higgs field](../../../standard-model.md#higgs-field) $\hat\Phi$ gives $S^2_\infty\to SU(2)/U(1)\cong S^2$. With outward orientation its degree is

$$
n=\frac1{8\pi}\int_{S^2_\infty}
\epsilon_{abc}\hat\Phi^a\,d\hat\Phi^b\wedge d\hat\Phi^c.
$$

The integrand is the normalized target area form, so the [hedgehog ansatz for a monopole](../../../classical-field-theory-soliton.md#hedgehog-ansatz-for-a-monopole) has degree one. Nonzero degree obstructs extending the normalized Higgs direction through the ball; the full Higgs field must leave the vacuum manifold, normally vanishing in its core. The asymptotic unbroken Abelian [magnetic flux](../../../electromagnetism.md#magnetic-flux) measures the same integer with a convention-dependent sign.

For the [Skyrme model](../../../classical-field-theory-soliton.md#skyrme-model), a field $U:\mathbb R^3\to SU(2)$ with $U\to1$ at infinity gives $S^3\to S^3$, because [SU(2) as the three-sphere](../../../topological-group.md#su-2-as-the-three-sphere) identifies the target. A choice of orientations gives its [topological baryon number in the Skyrme model](../../../classical-field-theory-soliton.md#topological-baryon-number-in-the-skyrme-model) as the winding integral $\pm(24\pi^2)^{-1}\int\operatorname{tr}(U^{-1}dU)^3$; specifying the orientation fixes the sign. Similarly, the transition map at infinity of a four-dimensional [Yang-Mills instanton](../../../classical-field-theory-soliton.md#yang-mills-instanton) has degree in $\pi_3(SU(2))$, measured by its Chern charge.

A [scalar-field kink](../../../classical-field-theory-soliton.md#scalar-field-kink) illustrates the discrete-vacuum case: its endpoint data lie in $\pi_0(\{\pm1\})$, rather than being a map between connected positive-dimensional spheres. For the double-well field its [topological charge](../../../classical-field-theory-soliton.md#topological-charge) is $Q=[\phi(+\infty)-\phi(-\infty)]/2$. A kink has $Q=1$, an antikink $Q=-1$; they cannot individually deform to vacuum while their endpoints are fixed.

Degree classifies topology, rather than every solution. Smooth motion or local perturbations with fixed boundary data preserve it, and a nonzero degree obstructs decay to the vacuum within that class. It does not guarantee existence of a smooth energy minimizer, a fixed size, uniqueness, or dynamical stability. The [degree and energetic stability of a field configuration](../../../classical-field-theory-soliton.md#degree-and-energetic-stability-of-a-field-configuration) are distinct: a field can shrink towards a singular limit at fixed degree, as [Derrick's theorem](../../../classical-field-theory-soliton.md#derrick-s-theorem) diagnoses in many two-derivative theories. Moreover degree need not classify all homotopy classes for an arbitrary target; other [homotopy groups](../../../algebraic-topology.md#homotopy-group) or invariants may be needed. Within one degree there can be continuous [moduli spaces](../../../geometry-and-topology.md#moduli-space) and several stationary solutions.

## 4

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use an [SU(2)](../../../topological-group.md#su-2-group) [connection one-form](../../../fiber-bundle.md#connection-one-form) $A=A_\mu dx^\mu$ with [Skew-Hermitian](../../../linear-operator-theory.md#skew-hermitian-matrix) generators $T_a=-i\sigma_a/2$, so $\operatorname{tr}(T_aT_b)=-\delta_{ab}/2$. Absorb the gauge coupling into $A$, and write its [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) as $F=dA+A\wedge A$. The [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation) convention is $A^h=h^{-1}Ah+h^{-1}dh$, giving $F^h=h^{-1}Fh$.

In four dimensions the [Second Chern form](../../../geometry-and-topology.md#second-chern-form) and [Second Chern number](../../../geometry-and-topology.md#second-chern-number) of the associated fundamental rank-two bundle are

$$
c_2(A)=\frac1{8\pi^2}\operatorname{tr}(F\wedge F),\qquad
k_C=\int_Mc_2(A)\in\mathbb Z.
$$

Here $M$ is a closed oriented four-manifold. This sign follows by expanding the total [Chern class](../../../algebraic-geometry.md#chern-class) $\det(1+iF/(2\pi))$ and using $\operatorname{tr}F=0$. The first Chern class vanishes for [SU(2)](../../../topological-group.md#su-2-group); the second is the degree-four characteristic class relevant here. With the same curvature convention the commonly positive self-dual [instanton number](../../../classical-field-theory-soliton.md#instanton-number) is

$$
Q=-\frac1{8\pi^2}\int_M\operatorname{tr}(F\wedge F)=-k_C.
$$

Both sign conventions occur; fixing them at the outset avoids identifying opposite-oriented integers.

The form is [gauge-invariant](../../../relativistic-quantum-field.md#gauge-invariance) by conjugation and cyclicity of the [matrix trace](../../../linear-algebra.md#matrix-trace). The [gauge-theory Bianchi identity](../../../relativistic-quantum-field.md#gauge-theory-bianchi-identity) $D_AF=0$ makes it closed. To see that its integral is independent of the connection, vary $A$:

$$
\delta F=D_A\delta A,\qquad
\delta\operatorname{tr}(F\wedge F)
=2d\,\operatorname{tr}(\delta A\wedge F).
$$

On a closed $M$ the integral of this exact form vanishes. This is [Chern-Weil connection transgression](../../../geometry-and-topology.md#chern-weil-connection-transgression), showing that $k_C$ depends on the bundle's topology rather than on a particular [gauge field](../../../relativistic-quantum-field.md#gauge-field).

Locally the same four-form is an exterior derivative. The [Chern-Simons 3-form](../../../geometry-and-topology.md#chern-simons-3-form)

$$
\omega_3(A)=\operatorname{tr}\left(A\wedge dA+
\frac23A\wedge A\wedge A\right)
$$

satisfies

$$
d\omega_3=\operatorname{tr}(F\wedge F).
$$

For verification, differentiating gives $\operatorname{tr}(dA\wedge dA+2dA\wedge A\wedge A)$; expansion of $F\wedge F$ gives these terms and $\operatorname{tr}A^4$. Graded cyclicity moves the first one-form through the other three, changing the sign, so $\operatorname{tr}A^4=0$. This local exactness does not make the [Second Chern number](../../../geometry-and-topology.md#second-chern-number) zero on every closed manifold: on a nontrivial bundle the gauge potentials and $\omega_3$ are only patchwise defined.

For the usual finite-action sector on $\mathbb R^4$, impose pure-gauge behavior $A\to h^{-1}dh$ at infinity. Compactification gives a bundle over $S^4$, with transition map $h:S^3\to SU(2)$. The [Maurer-Cartan equation](../../../lie-theory.md#maurer-cartan-equation) gives $d(h^{-1}dh)=-(h^{-1}dh)^2$, hence

$$
\omega_3(h^{-1}dh)=-\frac13\operatorname{tr}(h^{-1}dh)^3.
$$

With the outward boundary orientation, [Stokes theorem](../../../calculus.md#stokes-theorem) therefore gives

$$
k_C=-\frac1{24\pi^2}\int_{S^3_\infty}
\operatorname{tr}(h^{-1}dh)^3,\qquad
Q=\frac1{24\pi^2}\int_{S^3_\infty}
\operatorname{tr}(h^{-1}dh)^3.
$$

These are opposite choices of the [winding number](../../../complex-analysis.md#winding-number), and either becomes the [topological degree](../../../geometry-and-topology.md#topological-degree) of $h$ after specifying the orientation of the target [SU(2)](../../../topological-group.md#su-2-group) sphere. Thus integrality also follows from $\pi_3(SU(2))=\mathbb Z$. Smooth deformations preserving the asymptotic sector cannot change it.

The positive Euclidean [Yang-Mills action](../../../relativistic-quantum-field.md#yang-mills-action) is

$$
S=-\frac1{g^2}\int_M\operatorname{tr}(F\wedge *F)
=\frac1{4g^2}\int_MF_{\mu\nu}^aF_{\mu\nu}^a\,d^4x.
$$

Define $\|X\|^2=-\int\operatorname{tr}(X\wedge *X)$. Since the [Hodge star](../../../differential-form.md#hodge-star-operator) has square one on two-forms in Euclidean dimension four,

$$
S=\frac1{2g^2}\|F-s*F\|^2+\frac{8\pi^2s}{g^2}Q,
\qquad s=\pm1.
$$

Choosing $s=\operatorname{sgn}Q$ gives the [Yang-Mills instanton Bogomolny bound](../../../classical-field-theory-soliton.md#yang-mills-instanton-bogomolny-bound)

$$
\boxed{S\geq\frac{8\pi^2}{g^2}|Q|,\qquad
F=s*F\ \text{at equality}.}
$$

The [self-dual Yang-Mills equations](../../../classical-field-theory-soliton.md#self-dual-yang-mills-equations) and their anti-self-dual version imply the [Yang-Mills equations](../../../relativistic-quantum-field.md#yang-mills-equations) $D_A*F=0$ by the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity). Their finite-action solutions are [Yang-Mills instantons](../../../classical-field-theory-soliton.md#yang-mills-instanton).

For a concrete self-dual example, the [BPST instanton](../../../classical-field-theory-soliton.md#bpst-instanton) with center $a$ and size $\rho>0$ has

$$
A_\mu^a=\frac{2\eta^a_{\mu\nu}(x-a)^\nu}{|x-a|^2+\rho^2},
\qquad
F_{\mu\nu}^a=-\frac{4\rho^2\eta^a_{\mu\nu}}
{(|x-a|^2+\rho^2)^2},
$$

where $\eta^a_{\mu\nu}$ are self-dual ['t Hooft symbols](../../../differential-form.md#t-hooft-symbol). Their contraction is $\sum_{a,\mu,\nu}(\eta^a_{\mu\nu})^2=12$. Thus $F_{\mu\nu}^aF_{\mu\nu}^a=192\rho^4/(|x-a|^2+\rho^2)^4$, and

$$
\int_{\mathbb R^4}\frac{\rho^4\,d^4x}{(|x|^2+\rho^2)^4}
=2\pi^2\int_0^\infty\frac{\rho^4r^3\,dr}{(r^2+\rho^2)^4}
=\frac{\pi^2}{6}.
$$

This gives $S=8\pi^2/g^2$ and $Q=1$. Reversing duality gives $Q=-1$. The free center, size and framed gauge orientation illustrate the [instanton moduli space](../../../classical-field-theory-soliton.md#instanton-moduli-space).

On a three-dimensional slice $\Sigma$, there is no four-form Chern integral intrinsic to the slice. Its transgression is the [Chern-Simons number of a gauge field](../../../geometry-and-topology.md#chern-simons-number-of-a-gauge-field), in the instanton-charge convention

$$
N_{\mathrm{CS}}[A]=-\frac1{8\pi^2}\int_\Sigma\omega_3(A).
$$

It is a real number for a general connection, not necessarily an integer, and is not strictly gauge invariant. Set $\theta=h^{-1}dh$ and $\bar\theta=dh\,h^{-1}$. Substituting $A^h=h^{-1}Ah+\theta$, using $d\theta=-\theta^2$ and graded trace cyclicity, gives the [gauge change of the Chern-Simons three-form](../../../geometry-and-topology.md#gauge-change-of-the-chern-simons-three-form)

$$
\omega_3(A^h)=\omega_3(A)-d\operatorname{tr}(\bar\theta\wedge A)
-\frac13\operatorname{tr}\theta^3.
$$

The mixed terms collect into the displayed exact form; the last term is also fixed by the pure-gauge case $A=0$. Therefore on a closed $\Sigma$, or with boundary conditions making the exact-form integral vanish,

$$
\boxed{N_{\mathrm{CS}}[A^h]=N_{\mathrm{CS}}[A]+w(h),\qquad
w(h)=\frac1{24\pi^2}\int_\Sigma\operatorname{tr}(h^{-1}dh)^3\in\mathbb Z.}
$$

Thus $N_{\mathrm{CS}}\bmod\mathbb Z$, or $\exp(2\pi iN_{\mathrm{CS}})$, is gauge invariant. Gauge maps homotopic to the identity have $w=0$; maps of nonzero winding are large transformations even when they equal the identity at infinity.

For a [Yang-Mills vacuum](../../../relativistic-quantum-field.md#yang-mills-vacuum) on $\mathbb R^3$, zero magnetic [energy](../../../classical-mechanics.md#energy) requires $F_{ij}=0$. On simply connected space this is a pure gauge $A=h^{-1}dh$, and $N_{\mathrm{CS}}=w(h)$ is an integer after fixing the asymptotic trivialization. Quotienting only by transformations homotopic to the identity leaves integer-labelled vacuum representatives. Allowing all winding transformations identifies them classically; quantum states can instead transform by a phase, producing the [theta vacuum](../../../relativistic-quantum-field.md#theta-vacuum). A three-dimensional pure-gauge representative carries a winding number but is not a localized positive-energy monopole. In fact [no static finite-energy lump in three-dimensional pure Yang-Mills theory](../../../classical-field-theory-soliton.md#no-static-finite-energy-lump-in-three-dimensional-pure-yang-mills-theory) exists with the usual decay conditions: $A_i^{(s)}(x)=sA_i(sx)$ gives $E(s)=sE(1)$, and stationarity forces $E=0$.

Finally, on an oriented spacetime slab $[t_-,t_+]\times\Sigma$, with no side-boundary contribution, the transgression identity gives

$$
\boxed{Q=N_{\mathrm{CS}}(t_+)-N_{\mathrm{CS}}(t_-).}
$$

A [Yang-Mills instanton](../../../classical-field-theory-soliton.md#yang-mills-instanton) therefore interpolates between vacuum representatives whose [Chern-Simons numbers](../../../geometry-and-topology.md#chern-simons-number-of-a-gauge-field) differ by its integer charge. In a four-dimensional quantum theory a [Yang-Mills theta term](../../../relativistic-quantum-field.md#yang-mills-theta-term) weights such sectors by $e^{i\theta Q}$, making $\theta$ periodic modulo $2\pi$. In an intrinsically three-dimensional theory an action $2\pi\ell N_{\mathrm{CS}}$ has a gauge-invariant phase $e^{iS}$ only for integer level $\ell$ under all winding gauge maps. These statements distinguish the gauge-invariant integer four-dimensional Chern charge from the three-dimensional connection-dependent quantity defined modulo integers.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
