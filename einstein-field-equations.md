# Einstein field equations

↑ **Parent:** [General relativity](general-relativity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Einstein_field_equations)

With signature $(-,+,+,+)$ and vanishing cosmological constant, the Einstein field equations are

$$
R_{\mu\nu}-\frac12 g_{\mu\nu}R=\kappa T_{\mu\nu}.
$$

In four spacetime dimensions, contraction with $g^{\mu\nu}$ gives the useful trace relation $R=-\kappa T$.

In the usual commutator convention for the [Riemann curvature tensor](riemann-curvature-tensor.md), $\kappa=8\pi G/c^4$: $G$ is the [gravitational constant](newton-s-law-of-universal-gravitation.md#gravitational-constant), whereas $G_{\mu\nu}$ is the [Einstein tensor](riemann-curvature-tensor.md#einstein-tensor). The [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor) $R_{\mu\nu}$ and [scalar curvature](second-fundamental-form.md#scalar-curvature) $R$ encode contractions of [curvature](differential-geometry.md#curvature). The [stress-energy tensor](stress-energy-tensor.md) $T_{\mu\nu}$ includes [energy density](statistical-physics.md#energy-density), [momentum](momentum.md) flow and [stresses](continuum-mechanics.md#stress), so [pressure](pressure.md) also gravitates. A [cosmological constant](cosmology.md#cosmological-constant) adds $\Lambda g_{\mu\nu}$ to the left-hand side. See [Tong's Einstein equations and matter coupling](https://www.damtp.cam.ac.uk/user/tong/gr/grhtml/S4.html).

For a concrete consequence, set $T_{\mu\nu}=0$ and $\Lambda=0$. The trace gives $R=0$, and substitution gives $R_{\mu\nu}=0$. Yet the exterior [Schwarzschild spacetime](schwarzschild-spacetime.md) still has the [tidal forces](newton-s-law-of-universal-gravitation.md#tidal-force) computed under [geodesic deviation](riemann-curvature-tensor.md#geodesic-deviation): vanishing [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor) does not imply vanishing [Riemann curvature tensor](riemann-curvature-tensor.md). Geometry carries gravitational effects through empty space. Einstein presented the final matter equations on 25 November 1915, including the essential trace correction, in [Die Feldgleichungen der Gravitation, pages 844-847, especially equation (2a)](https://d-nb.info/1379427029/34). His symbols and sign conventions differ from modern ones; the displayed formula uses modern notation.

**Table of contents**

- [Trace coefficient fixed by stress-energy conservation](#trace-coefficient-fixed-by-stress-energy-conservation)
- [Einstein equation in the sequential-derivative curvature convention](#einstein-equation-in-the-sequential-derivative-curvature-convention)
- [Newtonian normalization of the Einstein field equations](#newtonian-normalization-of-the-einstein-field-equations)
- [Einstein-equation coupling under reversed curvature](#einstein-equation-coupling-under-reversed-curvature)
- [Planar Einstein metric with cubic radial function](#planar-einstein-metric-with-cubic-radial-function)
- [Lovelock's theorem](#lovelock-s-theorem)
- [Vacuum Einstein equations](#vacuum-einstein-equations)
  - [Vacuum spacetime](#vacuum-spacetime)
- [Einstein-Hilbert action](#einstein-hilbert-action)
  - [Einstein-Cartan theory](#einstein-cartan-theory)
    - [1.5-order formalism](#1-5-order-formalism)
    - [Algebraic torsion of a Dirac field](#algebraic-torsion-of-a-dirac-field)
  - [First-order three-dimensional gravity](#first-order-three-dimensional-gravity)
  - [Einstein-Proca theory](#einstein-proca-theory)
    - [Proca stress-energy tensor](#proca-stress-energy-tensor)
  - [Einstein-Maxwell-dilaton theory](#einstein-maxwell-dilaton-theory)
    - [Magnetically charged dilaton black hole](#magnetically-charged-dilaton-black-hole)
      - [Causal structure of the magnetic dilaton black hole](#causal-structure-of-the-magnetic-dilaton-black-hole)
      - [Geodesic potential of the magnetic dilaton black hole](#geodesic-potential-of-the-magnetic-dilaton-black-hole)
        - [Extremal dilaton metric photon capture](#extremal-dilaton-metric-photon-capture)
      - [Komar mass of the magnetic dilaton black hole](#komar-mass-of-the-magnetic-dilaton-black-hole)
- [Trace-reversed Einstein field equations in D dimensions](#trace-reversed-einstein-field-equations-in-d-dimensions)
  - [Ricci curvature sourced by a Klein-Gordon scalar field](#ricci-curvature-sourced-by-a-klein-gordon-scalar-field)
- [Metric variation](#metric-variation)
  - [Palatini identity](#palatini-identity)
  - [Metric variation of scalar curvature](#metric-variation-of-scalar-curvature)
- [Modified gravity](#modified-gravity)
  - [Tensor-vector-scalar gravity](#tensor-vector-scalar-gravity)
  - [Modified Newtonian dynamics](#modified-newtonian-dynamics)
  - [Scalar-tensor theory](#scalar-tensor-theory)
    - [Metric variation of a scalar-curvature coupling](#metric-variation-of-a-scalar-curvature-coupling)
    - [Brans-Dicke theory](#brans-dicke-theory)
      - [Scalar equation of Brans-Dicke theory](#scalar-equation-of-brans-dicke-theory)
        - [Degenerate coupling of Brans-Dicke theory](#degenerate-coupling-of-brans-dicke-theory)
  - [f(R) gravity](#f-r-gravity)
    - [Einstein-frame representation of metric f(R) gravity](#einstein-frame-representation-of-metric-f-r-gravity)
    - [Einstein metric condition in f(R) gravity](#einstein-metric-condition-in-f-r-gravity)
    - [Normalization of the metric f(R) field equation](#normalization-of-the-metric-f-r-field-equation)
    - [Linearized f(R) gravity about Minkowski spacetime](#linearized-f-r-gravity-about-minkowski-spacetime)

## Trace coefficient fixed by stress-energy conservation

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)

In four dimensions, the [contracted Bianchi identity](riemann-curvature-tensor.md#contracted-bianchi-identity) gives $(1/2-\alpha)\partial_\mu R=-\kappa\nabla^\nu T_{\mu\nu}$ for the displayed equation. Its trace is $(1-4\alpha)R=-\kappa T$. For $\alpha\ne1/4$,

$$
\nabla^\nu T_{\mu\nu}=\frac{1/2-\alpha}{1-4\alpha}\partial_\mu T.
$$

Compatibility with covariant [stress-energy conservation](stress-energy-tensor.md#stress-energy-conservation) for unrestricted conventional matter therefore requires $\alpha=1/2$, yielding the [Einstein tensor](riemann-curvature-tensor.md#einstein-tensor). Other coefficients impose constant trace on conserved sources. The exceptional $\alpha=1/4$ equation instead requires $T=0$; conservation additionally makes $R$ constant. A trace-free equation sourced by $T_{\mu\nu}-g_{\mu\nu}T/4$ is a different system and does not impose vanishing matter trace.

## Einstein equation in the sequential-derivative curvature convention

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)

With signature $(+---)$, let $R^a{}_{bcd}=\partial_d\Gamma^a{}_{bc}-\partial_c\Gamma^a{}_{bd}-\Gamma^a{}_{pc}\Gamma^p{}_{bd}+\Gamma^a{}_{pd}\Gamma^p{}_{bc}$ and $R_{ab}=R^c{}_{acb}$. This curvature is the negative of the convention in which $[\nabla_c,\nabla_d]X^a=R^a{}_{bcd}X^b$. The physical [Einstein field equations](einstein-field-equations.md) are $G_{ab}+\Lambda g_{ab}=-8\pi G T_{ab}/c^4$. In a static weak field $R_{00}=-\nabla^2\Phi/c^2$; the trace-reversed equation then reproduces the [Poisson equation](partial-differential-equation.md#poisson-s-equation) $\nabla^2\Phi=4\pi G\rho_{\rm mass}$. Metric variation of $\int\sqrt{-g}(R-2\Lambda)/(2\kappa)+S_m$ gives the same sign when $\delta S_m=\int\sqrt{-g}T_{ab}\delta g^{ab}/2$.

## Newtonian normalization of the Einstein field equations

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)

Assume a metric theory in four dimensions, a [Levi-Civita connection](general-relativity.md#levi-civita-connection), covariant [stress-energy conservation](stress-energy-tensor.md#stress-energy-conservation) and field equations linear in second metric derivatives. The [contracted Bianchi identity](riemann-curvature-tensor.md#contracted-bianchi-identity) selects $G_{ab}=R_{ab}-g_{ab}R/2$. Its trace-reversed equation is $R_{ab}=\kappa(T_{ab}-g_{ab}T/2)+\Lambda g_{ab}$. In the convention $R_{00}\simeq-\nabla^2\varphi$ and signature $(+---)$, nonrelativistic matter gives $R_{00}\simeq\kappa\rho/2$. The [Poisson equation](partial-differential-equation.md#poisson-s-equation) $\nabla^2\varphi=4\pi G\rho$ fixes $\kappa=-8\pi G$. Reversing the curvature convention reverses this displayed coupling sign without changing the physical theory. The [strong equivalence principle](general-relativity.md#strong-equivalence-principle) alone does not establish uniqueness without the stated additional assumptions.

## Einstein-equation coupling under reversed curvature

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)

With the metric and [stress-energy tensor](stress-energy-tensor.md) fixed and zero [cosmological constant](cosmology.md#cosmological-constant), changing the sign convention for the [Riemann curvature tensor](riemann-curvature-tensor.md) changes the signs of the [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor), [scalar curvature](second-fundamental-form.md#scalar-curvature) and [Einstein tensor](riemann-curvature-tensor.md#einstein-tensor). The same physical field equation is therefore written with the opposite coupling sign. For signature $(+---)$, the convention $R^a{}_{bcd}=\partial_d\Gamma^a_{bc}-\partial_c\Gamma^a_{bd}-\Gamma^a_{ec}\Gamma^e_{bd}+\Gamma^a_{ed}\Gamma^e_{bc}$ and $R_{ab}=R^c{}_{acb}$ gives $R_{00}\simeq-\Delta\Phi$ in a static [Newtonian limit](linearized-gravity.md#newtonian-limit). The trace-reversed equation and $\Delta\Phi=4\pi G\rho$ then require $G_{ab}=-8\pi GT_{ab}$.

## Planar Einstein metric with cubic radial function

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)

This metric has $R_{ab}=-3g_{ab}$ and [cosmological constant](cosmology.md#cosmological-constant) $\Lambda=-3$ in unit curvature-radius normalization. Its regular static coframe is real when $F>0$ and $z\ne0$. Setting $q=\alpha z^3$, its six independent [curvature 2-form](connection-1-form.md#curvature-2-form) coefficients are $-(1-q)$ in the $03$ and $12$ planes and $-(1+q/2)$ in the other four planes. Their Ricci contractions cancel $q$. The [Weyl tensor](riemann-curvature-tensor.md#weyl-tensor) squared invariant is $12\alpha^2z^6$, so nonzero $\alpha$ does not give constant sectional curvature despite the Einstein equation.

<h2 id="lovelock-s-theorem">Lovelock's theorem</h2>

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)

In four dimensions, a local natural symmetric divergence-free metric tensor involving the metric and its derivatives of at most second order has the Lovelock form $aG_{ab}+bg_{ab}$ with constant coefficients. Generic nonlinear metric [f(R) gravity](#f-r-gravity) instead has fourth-order terms and does not meet that derivative-order hypothesis. For affine $f$, the metric field equation is precisely of Lovelock form.

## Vacuum Einstein equations

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)

In a region with vanishing [stress-energy tensor](stress-energy-tensor.md), the [Einstein field equations](einstein-field-equations.md) reduce to $R_{\mu\nu}=0$ when the [cosmological constant](cosmology.md#cosmological-constant) vanishes.

### Vacuum spacetime

↑ **Parent:** [Vacuum Einstein equations](#vacuum-einstein-equations)

A [vacuum spacetime](#vacuum-spacetime) has vanishing matter [stress-energy tensor](stress-energy-tensor.md). In $D>2$ dimensions, tracing the [Vacuum Einstein equations](#vacuum-einstein-equations) gives $R=2D\Lambda/(D-2)$ and hence $R_{ab}=2\Lambda g_{ab}/(D-2)$; in four dimensions this reduces to $R_{ab}=\Lambda g_{ab}$. With zero [cosmological constant](cosmology.md#cosmological-constant) it is [Ricci flat](differential-geometry.md#ricci-flat-manifold), although its full [Riemann curvature tensor](riemann-curvature-tensor.md) can be nonzero: a vacuum [Kerr black hole](black-hole.md#kerr-black-hole) and vacuum [gravitational waves](gravitational-wave.md) illustrate that distinction.

## Einstein-Hilbert action

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Einstein-Hilbert_action)

The Einstein-Hilbert action is the integral of the [Ricci scalar](general-relativity.md#ricci-scalar) against the metric volume form. Varying it with respect to the metric gives the vacuum [Einstein field equations](einstein-field-equations.md), up to a boundary term.

### Einstein-Cartan theory

↑ **Parent:** [Einstein-Hilbert action](#einstein-hilbert-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Einstein-Cartan_theory)

An independent [vierbein](general-relativity.md#orthonormal-coframe-in-spacetime) and metric-compatible [spin connection](connection-1-form.md#spin-connection) allow [spin](angular-momentum-operator.md#spin) density to source a [torsion tensor](vector-bundle.md#torsion-tensor). The connection equation from the [Einstein-Hilbert action](#einstein-hilbert-action) is algebraic in torsion. In the absence of connection-dependent matter it fixes the [Levi-Civita connection](general-relativity.md#levi-civita-connection). For a minimally coupled [Dirac field](relativistic-quantum-field.md#dirac-field), eliminating the connection generates a local four-fermion interaction. Thus its equivalent torsion-free second-order [action](lagrangian-mechanics.md#action) includes this contact term; simply dropping it defines a different matter theory.

<h4 id="1-5-order-formalism">1.5-order formalism</h4>

↑ **Parent:** [Einstein-Cartan theory](#einstein-cartan-theory)

Solve the algebraic connection equation for $\widehat\omega(e,\chi)$, but perform the remaining variations as though the connection were independent. The chain-rule contribution $(\delta S/\delta\omega)\delta\widehat\omega$ vanishes on that solution. The resulting equations are those of the connection-eliminated second-order [action](lagrangian-mechanics.md#action). This is especially useful for local [supersymmetry](supersymmetry.md) calculations, where the gravitino-induced contorsion is quadratic in [fermions](tensor-product-of-quantum-systems.md#fermion) and the omitted induced connection variation would otherwise be lengthy.

#### Algebraic torsion of a Dirac field

↑ **Parent:** [Einstein-Cartan theory](#einstein-cartan-theory)

Use $K_{abc}=e_a{}^\mu(\omega-\omega(e))_{\mu bc}$ and $T_{abc}=K_{bac}-K_{cab}$. For the symmetrized Dirac [action](lagrangian-mechanics.md#action) $-e\bar\chi\gamma^\mu\overleftrightarrow\nabla_\mu\chi/2-em\bar\chi\chi$, varying the [spin connection](connection-1-form.md#spin-connection) gives $-e\bar\chi\gamma^{\mu ab}\chi\,\delta\omega_{\mu ab}/4$. Only totally antisymmetric contorsion is sourced. Its [action](lagrangian-mechanics.md#action) is $-eK^2/(2\kappa^2)-eK_{abc}\bar\chi\gamma^{abc}\chi/4$, hence the stated solution. Substitution generates $e\kappa^2(\bar\chi\gamma^{abc}\chi)(\bar\chi\gamma_{abc}\chi)/32$. The torsion is an [auxiliary field](supersymmetry.md#auxiliary-field), not an independent propagating degree of freedom.

### First-order three-dimensional gravity

↑ **Parent:** [Einstein-Hilbert action](#einstein-hilbert-action)

For a nondegenerate [orthonormal coframe in spacetime](general-relativity.md#orthonormal-coframe-in-spacetime) $E^a$ and independent antisymmetric Lorentz [connection 1-form](connection-1-form.md), the action $\int\epsilon_{abc}(R^{ab}\wedge E^c+\lambda E^a\wedge E^b\wedge E^c)$ has independent coframe and connection variations. Since $\delta R^{ab}=D\delta\omega^{ab}$, integration by parts yields a connection equation $\epsilon_{abc}T^c=0$. The three variations of the cubic coframe term give the coframe equation $\epsilon_{abc}(R^{ab}+3\lambda E^a\wedge E^b)=0$. In three dimensions these are exactly the equations displayed above. The solution has [constant sectional curvature](riemann-curvature-tensor.md#constant-sectional-curvature) $K=-3\lambda$. Omitting the factor of three changes the cosmological normalization.

### Einstein-Proca theory

↑ **Parent:** [Einstein-Hilbert action](#einstein-hilbert-action)

Einstein-Proca theory couples [general relativity](general-relativity.md) to a massive vector field governed by the [Proca action](electromagnetism.md#proca-action). Its matter stress-energy tensor is

$$
T_{ab}=F_{ac}F_b{}^c-\frac14g_{ab}F_{cd}F^{cd}
+m^2\left(A_aA_b-\frac12g_{ab}A_cA^c\right).
$$

The [contracted Bianchi identity](riemann-curvature-tensor.md#contracted-bianchi-identity) makes the Einstein equation compatible with the covariant [Proca equation](electromagnetism.md#proca-equation).

#### Proca stress-energy tensor

↑ **Parent:** [Einstein-Proca theory](#einstein-proca-theory)

The Proca stress-energy tensor is the metric variation of the matter part of the [Proca action](electromagnetism.md#proca-action). It consists of the [electromagnetic stress-energy tensor](relativistic-electromagnetism.md#electromagnetic-stress-energy-tensor) plus the quadratic mass contribution $m^2(A_aA_b-g_{ab}A^2/2)$.

### Einstein-Maxwell-dilaton theory

↑ **Parent:** [Einstein-Hilbert action](#einstein-hilbert-action)

Einstein-Maxwell-dilaton theory couples the metric to a scalar field and a Maxwell field with scalar-dependent gauge coupling, typically through $e^{\alpha\Phi}F_{ab}F^{ab}$. Its Maxwell equation is $\nabla_a(e^{\alpha\Phi}F^{ab})=0$.

#### Magnetically charged dilaton black hole

↑ **Parent:** [Einstein-Maxwell-dilaton theory](#einstein-maxwell-dilaton-theory)

The unit-coupling magnetic solution of [Einstein-Maxwell-dilaton theory](#einstein-maxwell-dilaton-theory) has $ds^2=-Vdt^2+V^{-1}dr^2+R^2d\Omega_2^2$, magnetic potential $A=P\cos\theta\,d\phi$, and dilaton $\phi=-\tfrac12\log(1-r_-/r)$, where $r_-=2P^2/r_+$ and $r_+>0$. Its physical asymptotic component has $r>r_-$. For $0\le r_-<r_+$ it has a regular [Killing horizon](general-relativity.md#killing-horizon) at $r_+$, area $4\pi r_+(r_+-r_-)$ and [surface gravity](general-relativity.md#surface-gravity) $1/(2r_+)$. Its asymptotic mass is $r_+/2$. For $r_->r_+$ the zero-area singularity is naked. The limiting case $r_-=r_+$ is singular and must not be treated as a regular nondegenerate horizon.

##### Causal structure of the magnetic dilaton black hole

↑ **Parent:** [Magnetically charged dilaton black hole](#magnetically-charged-dilaton-black-hole)

For $r_-<r_+$, an ingoing chart with $v=t+r_*$ has metric $-Vdv^2+2dv\,dr+R^2d\Omega_2^2$. In its future interior, $\nabla r=\partial_v+V\partial_r$ is future timelike, so every future causal curve decreases $r$ and cannot reach [future null infinity](general-relativity.md#future-null-infinity). The singularity $r=r_-$ is spacelike. A [Kruskal–Szekeres coordinates](schwarzschild-spacetime.md#kruskal-szekeres-coordinates) extension has the same qualitative [Penrose diagram](black-hole.md#penrose-diagram) as [Schwarzschild spacetime](schwarzschild-spacetime.md), with two exterior regions, a future black-hole interior and a past [white hole](black-hole.md#white-hole) interior. The past interior has the same radial interval but is not a [black hole](black-hole.md) region; specifying the radial interval alone does not identify the future component. For $r_->r_+$, the physical exterior $r>r_-$ has $V>0$ everywhere and outgoing null rays escape from arbitrarily near a timelike [naked singularity](black-hole.md#naked-singularity).

##### Geodesic potential of the magnetic dilaton black hole

↑ **Parent:** [Magnetically charged dilaton black hole](#magnetically-charged-dilaton-black-hole)

Rotate any [geodesic](riemannian-geometry.md#geodesic) into an equatorial plane of the [magnetically charged dilaton black hole](#magnetically-charged-dilaton-black-hole). Conserved energy and angular momentum are $E=V\dot t$ and $L=R^2\dot\phi$. Normalizing its tangent to $g(\dot x,\dot x)=-\epsilon$, with $\epsilon=1,0,-1$ for timelike, null and spacelike geodesics, gives $\dot r^2=E^2-V(\epsilon+L^2/R^2)$. Thus its radial equation is $\dot r^2/2+\widetilde V=0$. Radial null rays have $\dot r=\pm E$ and use the same [Schwarzschild tortoise coordinate](schwarzschild-spacetime.md#schwarzschild-tortoise-coordinate) with $2M$ replaced by $r_+$.

###### Extremal dilaton metric photon capture

↑ **Parent:** [Geodesic potential of the magnetic dilaton black hole](#geodesic-potential-of-the-magnetic-dilaton-black-hole)

For $f=1-2M/r$ and squared areal radius $C=r(r-b)$, an equatorial [null geodesic](special-relativity.md#null-geodesic) obeys $\dot r^2=E^2[1-B^2f/C]$, with [impact parameter](classical-mechanics.md#impact-parameter) $B=L/E$. At $b=2M$, $f/C=1/r^2$ in the exterior. Its supremum is $1/(4M^2)$ at the null singular boundary, rather than at a regular exterior [photon sphere](schwarzschild-spacetime.md#photon-sphere). Rays with $B>2M$ turn at $r=B$; rays with $B<2M$ reach the boundary. Assuming those rays are absorbed gives the displayed geometric-optics cross-section despite zero limiting horizon area.

##### Komar mass of the magnetic dilaton black hole

↑ **Parent:** [Magnetically charged dilaton black hole](#magnetically-charged-dilaton-black-hole)

For the [magnetically charged dilaton black hole](#magnetically-charged-dilaton-black-hole), the metric-dual one-form of $k=\partial_t$ is $k^\flat=-Vdt$. With orientation $dt\wedge dr\wedge d\theta\wedge d\phi$, its [Hodge star operator](differential-form.md#hodge-star-operator) gives $\star dk^\flat=-V'R^2\sin\theta\,d\theta\wedge d\phi$. Therefore the [Komar mass](killing-vector-field.md#komar-mass) is $R^2V'/2=r_+/2-P^2/r$. Its radial dependence is allowed because the [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor) is nonzero; the divergence of $dk^\flat$ is sourced by $R_{ab}k^b$. At the horizon $M_K(r_+)=(r_+-r_-)/2=\kappa A_H/(4\pi)$.

## Trace-reversed Einstein field equations in D dimensions

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)

For $D>2$, tracing and substituting back gives

$$
R_{\mu\nu}
=\kappa\left(T_{\mu\nu}-\frac1{D-2}g_{\mu\nu}T\right).
$$

### Ricci curvature sourced by a Klein-Gordon scalar field

↑ **Parent:** [Trace-reversed Einstein field equations in D dimensions](#trace-reversed-einstein-field-equations-in-d-dimensions)

For the conserved scalar stress tensor above,

$$
R_{\mu\nu}
=\frac\kappa2\left[
\nabla_\mu\phi\nabla_\nu\phi
+\frac{m^2}{D-2}g_{\mu\nu}\phi^2
\right].
$$

## Metric variation

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)

For $h_{ab}=\delta g_{ab}$, variation of the inverse metric and metric volume form gives

$$
\delta g^{ab}=-h^{ab},
\qquad
\delta(d\operatorname{vol}_g)=\frac12g^{ab}h_{ab}\,d\operatorname{vol}_g.
$$

The [Levi-Civita connection](general-relativity.md#levi-civita-connection) varies by

$$
\delta\Gamma^a{}_{bc}=\frac12g^{ad}
(\nabla_bh_{cd}+\nabla_ch_{bd}-\nabla_dh_{bc}).
$$

### Palatini identity

↑ **Parent:** [Metric variation](#metric-variation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Palatini_identity)

For the [Levi-Civita connection](general-relativity.md#levi-civita-connection), the difference of two connections is a tensor. Varying the coordinate expression for the [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor) then gives the displayed covariant identity. It is the starting point for the [metric variation of scalar curvature](#metric-variation-of-scalar-curvature).

### Metric variation of scalar curvature

↑ **Parent:** [Metric variation](#metric-variation)

For $h_{ab}=\delta g_{ab}$, the [Ricci scalar](general-relativity.md#ricci-scalar) varies as

$$
\delta R=-R^{ab}h_{ab}+\nabla_a\nabla_bh^{ab}-\nabla^a\nabla_ah,
\qquad h=g^{ab}h_{ab}.
$$

The last two terms form a [covariant divergence](general-relativity.md#covariant-divergence) and hence contribute only a boundary term to a compactly supported variation of the [Einstein-Hilbert action](#einstein-hilbert-action).

## Modified gravity

↑ **Parent:** [Einstein field equations](einstein-field-equations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modified_gravity)

Modified gravity changes the Einstein-Hilbert action or its field equations in order to produce gravitational dynamics different from general relativity.

### Tensor-vector-scalar gravity

↑ **Parent:** [Modified gravity](#modified-gravity)

A relativistic gravitational theory constructed by [Jacob Bekenstein](physicist.md#jacob-bekenstein) using tensor, vector and [scalar fields](classical-field-theory.md#scalar-field), together with a specified physical [metric](topological-analysis.md#metric) for matter. It illustrates how the low-acceleration phenomenology of [MOND](#modified-newtonian-dynamics) can be embedded in a theory with calculable light deflection. Matching rotation curves is not sufficient to establish its lensing or cosmological predictions.[Relativistic action and physical metric](physics-bibliography.md#relativistic-gravitation-theory-for-the-mond-paradigm-by-jacob-bekenstein)

### Modified Newtonian dynamics

↑ **Parent:** [Modified gravity](#modified-gravity)

A low-acceleration modification associated with [Mordehai Milgrom](physicist.md#mordehai-milgrom). For an isolated spherical system, $g\mu(g/a_0)=g_N$, with $\mu(x)\to1$ at high $x$ and $\mu(x)\to x$ at low $x$. An isolated point-like baryonic distribution then gives $v_c^4=GM_ba_0$ and a flat asymptotic [galaxy rotation curve](galaxy.md#galaxy-rotation-curve). The algebraic spherical relation is not a complete relativistic field theory and should not be assumed to hold vectorially for arbitrary [mass](classical-mechanics.md#mass) distributions.[Pages 365–370](physics-bibliography.md#a-modification-of-the-newtonian-dynamics-as-a-possible-alternative-to-the-hidden-mass-hypothesis-by-mordehai-milgrom)

### Scalar-tensor theory

↑ **Parent:** [Modified gravity](#modified-gravity)

A [scalar-tensor theory](#scalar-tensor-theory) uses a [metric tensor](general-relativity.md#metric-tensor) and an additional [scalar field](classical-field-theory.md#scalar-field) to mediate gravity. A [scalar](vector-space.md#scalar) multiplier of the [Ricci scalar](general-relativity.md#ricci-scalar) makes the [curvature](differential-geometry.md#curvature) coupling depend on that field. The [Brans-Dicke theory](#brans-dicke-theory) is a standard example; the choice of [scalar](vector-space.md#scalar) potential and kinetic coupling distinguishes different members of the class.

#### Metric variation of a scalar-curvature coupling

↑ **Parent:** [Scalar-tensor theory](#scalar-tensor-theory)

With the [curvature sign convention](riemann-curvature-tensor.md#curvature-sign-convention) in which $\delta R_{bc}=\nabla_c\delta\Gamma^a{}_{ba}-\nabla_a\delta\Gamma^a{}_{bc}$, the inverse-metric [variation](calculus-of-variations.md#variation) of $\int\sqrt{-g}\,\Phi R$ is $\int\sqrt{-g}\,E_{ab}\delta g^{ab}$ plus a [boundary term](calculus.md#boundary-term), for a [scalar](vector-space.md#scalar) multiplier held fixed in that variation. The [Palatini identity](#palatini-identity) expresses the [curvature](differential-geometry.md#curvature) variation as divergences of $\delta\Gamma$. Two [integrations by parts](calculus.md#integration-by-parts) move the [derivatives](calculus.md#derivative) onto $\Phi$, yielding the displayed terms. For constant $\Phi$ they vanish. The opposite [curvature](differential-geometry.md#curvature) convention instead has $E_{ab}=\Phi G_{ab}+g_{ab}\Box\Phi-\nabla_a\nabla_b\Phi$.

#### Brans-Dicke theory

↑ **Parent:** [Scalar-tensor theory](#scalar-tensor-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brans–Dicke_theory)

The [Brans-Dicke theory](#brans-dicke-theory) adds a dynamical [scalar field](classical-field-theory.md#scalar-field) $\Phi$ to a [metric tensor](general-relativity.md#metric-tensor) theory of gravity, with constant dimensionless coupling $\omega$. In a $(+---)$ signature and the reversed-curvature convention used here, the displayed Lagrangian is supplemented by matter and integrated against the [metric tensor](general-relativity.md#metric-tensor) volume density with prefactor $1/(16\pi G)$. Its [scalar](vector-space.md#scalar) multiplier of the [Ricci scalar](general-relativity.md#ricci-scalar) lets the [curvature](differential-geometry.md#curvature) coupling vary in spacetime. Both the [metric tensor](general-relativity.md#metric-tensor) and [scalar](vector-space.md#scalar) are varied; the [scalar equation of Brans-Dicke theory](#scalar-equation-of-brans-dicke-theory) follows by eliminating [curvature](differential-geometry.md#curvature) between the [scalar](vector-space.md#scalar) equation and the [trace](linear-algebra.md#matrix-trace) of the [metric tensor](general-relativity.md#metric-tensor) equation. The original construction is described in [Brans and Dicke's 1961 article](https://doi.org/10.1103/PhysRev.124.925).

##### Scalar equation of Brans-Dicke theory

↑ **Parent:** [Brans-Dicke theory](#brans-dicke-theory)

Assume four spacetime dimensions, $\Phi\ne0$, constant $\omega$, no [scalar](vector-space.md#scalar) potential and matter independent of $\Phi$. In the stated action convention, [scalar](vector-space.md#scalar) [variation](calculus-of-variations.md#variation) gives $\Phi R+\omega\Phi^{-1}(\nabla\Phi)^2-2\omega\Box\Phi=0$. The [trace](linear-algebra.md#matrix-trace) of the [metric tensor](general-relativity.md#metric-tensor) equation gives $\Phi R+\omega\Phi^{-1}(\nabla\Phi)^2+3\Box\Phi=8\pi G T$. Their subtraction proves the displayed [wave equation](wave-equation.md) with $T=g^{ab}T_{ab}$. The [degenerate coupling of Brans-Dicke theory](#degenerate-coupling-of-brans-dicke-theory) needs separate treatment before dividing by its coefficient.

###### Degenerate coupling of Brans-Dicke theory

↑ **Parent:** [Scalar equation of Brans-Dicke theory](#scalar-equation-of-brans-dicke-theory)

At $\omega=-3/2$, the combined [scalar equation of Brans-Dicke theory](#scalar-equation-of-brans-dicke-theory) becomes the matter consistency condition $T=0$. It does not determine $\Box\Phi$ by division, since the wave coefficient has vanished. The original [metric tensor](general-relativity.md#metric-tensor) and [scalar](vector-space.md#scalar) [Euler-Lagrange equations](analysis.md#euler-lagrange-equation) must be retained. Introducing scalar-dependent matter or a [scalar](vector-space.md#scalar) potential changes the consistency condition.

<h3 id="f-r-gravity">f(R) gravity</h3>

↑ **Parent:** [Modified gravity](#modified-gravity)

An f(R) theory replaces the Ricci scalar in the gravitational action by a smooth function $f(R)$. Its metric field equation is

$$
f'(R)R_{ab}-\frac12f(R)g_{ab}
+(g_{ab}\Box-\nabla_a\nabla_b)f'(R)=8\pi T_{ab}.
$$

<h4 id="einstein-frame-representation-of-metric-f-r-gravity">Einstein-frame representation of metric f(R) gravity</h4>

↑ **Parent:** [f(R) gravity](#f-r-gravity)

In the mostly-minus convention with vacuum gravitational action proportional to $\int\sqrt{-g}f(R)$ and $f'<0$, the displayed [conformal transformation](geometry-and-topology.md#conformal-map) turns its vacuum equation into $\widetilde G_{\mu\nu}=T_{\mu\nu}(\phi)$, with potential $V=(Rf'-f)/(2f'^2)$ and the [stress-energy tensor of a canonical scalar field](stress-energy-tensor.md#stress-energy-tensor-of-a-canonical-scalar-field). The conformal Ricci formula cancels the second derivatives of $f'$ against the original field equation. Its remaining derivative tensor is $\partial_\mu\phi\partial_\nu\phi-\widetilde g_{\mu\nu}(\widetilde\nabla\phi)^2/2$. Expressing $V$ as a function of $\phi$ requires a locally invertible $R\mapsto f'(R)$. When $f''=0$, this scalar-tensor parametrization degenerates and introduces no new propagating scalar degree of freedom.

<h4 id="einstein-metric-condition-in-f-r-gravity">Einstein metric condition in f(R) gravity</h4>

↑ **Parent:** [f(R) gravity](#f-r-gravity)

Every four-dimensional Einstein metric with $R_{ab}=\Lambda g_{ab}$ has constant [Ricci scalar](general-relativity.md#ricci-scalar) $R=4\Lambda$. The vacuum metric [f(R) gravity](#f-r-gravity) tensor reduces to $(\Lambda f'(4\Lambda)-f(4\Lambda)/2)g_{ab}$, giving the displayed necessary and sufficient condition for a fixed [cosmological constant](cosmology.md#cosmological-constant). Both function and derivative may vanish, so division by $f'$ is unnecessary. Requiring this for all real $\Lambda$ and a smooth $f$ instead yields $f(R)=CR^2$.

<h4 id="normalization-of-the-metric-f-r-field-equation">Normalization of the metric f(R) field equation</h4>

↑ **Parent:** [f(R) gravity](#f-r-gravity)

For a metric action $S_g=A\int\sqrt{-g}f(R)\,d^4x$ and the usual [stress-energy tensor](stress-energy-tensor.md) convention, covariant metric variation gives $A E_{ab}=T_{ab}/2$, where $E_{ab}=f'R_{ab}-fg_{ab}/2+(g_{ab}\Box-\nabla_a\nabla_b)f'$. With $A=1/(16\pi G)$ this becomes $E_{ab}=8\pi G T_{ab}$; with $A=1$ it becomes $E_{ab}=T_{ab}/2$. The chosen normalization does not alter the vacuum equation.

<h4 id="linearized-f-r-gravity-about-minkowski-spacetime">Linearized f(R) gravity about Minkowski spacetime</h4>

↑ **Parent:** [f(R) gravity](#f-r-gravity)

If $f(0)=0$, $f'(0)=1$, and $f''(0)=0$, then $f(R)=R+O(R^3)$ near zero. The field equations linearized about [Minkowski spacetime](special-relativity.md#minkowski-spacetime) are therefore the [Linearized Einstein equations](linearized-gravity.md#linearized-einstein-equations); deviations first appear beyond linear order.

## ↑ Ancestors (4)

1. [General relativity](general-relativity.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (115)

- [Affine focusing model for the Penrose theorem](general-relativity.md#affine-focusing-model-for-the-penrose-theorem)
- [Albert Einstein](physicist.md#albert-einstein)
- [Cartan curvature forms for a static spherical metric](connection-1-form.md#cartan-curvature-forms-for-a-static-spherical-metric)
- [CDM density equation in a matter-radiation universe](linear-cosmological-density-perturbation.md#cdm-density-equation-in-a-matter-radiation-universe)
- [Closed slicing of de Sitter spacetime](general-relativity.md#closed-slicing-of-de-sitter-spacetime)
- [Copernican principle](cosmology.md#copernican-principle)
- [Cosmological constant](cosmology.md#cosmological-constant)
- [Cosmological constant preserves null convergence](stress-energy-tensor.md#cosmological-constant-preserves-null-convergence)
- [Diffeomorphism invariance of general relativity](general-relativity.md#diffeomorphism-invariance-of-general-relativity)
- [Double-null focusing identity](geodesic-congruence.md#double-null-focusing-identity)
- [Einstein equation in the sequential-derivative curvature convention](#einstein-equation-in-the-sequential-derivative-curvature-convention)
- [Einstein-Hilbert action](#einstein-hilbert-action)
- [Equivalence principle does not uniquely fix field equations](general-relativity.md#equivalence-principle-does-not-uniquely-fix-field-equations)
- [Euclidean de Sitter action and entropy](general-relativity.md#euclidean-de-sitter-action-and-entropy)
- [General relativity](general-relativity.md)
- [Gravitational potential evolution of a barotropic fluid](linear-cosmological-perturbation-theory.md#gravitational-potential-evolution-of-a-barotropic-fluid)
- [Gravity](physics.md#gravity)
- [Hamiltonian constraint](numerical-relativity.md#hamiltonian-constraint)
- [Harmonic reduction of the vacuum Einstein equations](numerical-relativity.md#harmonic-reduction-of-the-vacuum-einstein-equations)
- [Komar angular momentum](killing-vector-field.md#komar-angular-momentum)
- [Komar angular momentum with inner boundaries](killing-vector-field.md#komar-angular-momentum-with-inner-boundaries)
- [Komar current from trace-reversed stress-energy](killing-vector-field.md#komar-current-from-trace-reversed-stress-energy)
- [Momentum constraint](numerical-relativity.md#momentum-constraint)
- [Null convergence condition](stress-energy-tensor.md#null-convergence-condition)
- [Null energy condition for a planar warped spacetime](stress-energy-tensor.md#null-energy-condition-for-a-planar-warped-spacetime)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-67.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-72.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-50.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-56.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-56.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-58.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-58.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-54.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-62.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-63.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-72.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#35a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-61.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-61.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-63.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-63.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-65.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-66.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-66.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1.md#15d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-54.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-54.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-55.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-57.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-52.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-56.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-57.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-58.md#section-i/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-58.md#section-i/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-49.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-48.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-49.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52.md#2/b/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-48.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-52.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-52.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-54.md#2/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-54.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-311.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-311.md#4/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-311.md#4/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-312.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-309.md#4/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-310.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-311.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-312.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-312.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-309.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-310.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-311.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#37d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-4.md#37c/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-311.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-311.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-312.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#38d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#38b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#37b/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-309.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-311.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-312.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-357.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4.md#37e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-309.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-311.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-309.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-311.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-311.md#1/d/ii/solution)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2014/paper-1.md#3/d/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2012/paper-1.md#3/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2016/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2016/paper-1.md#3/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2017.md#1/b/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2017.md#4/solution)
- [Penrose singularity theorem](general-relativity.md#penrose-singularity-theorem)
- [Perfect-fluid alignment in a static spacetime](stress-energy-tensor.md#perfect-fluid-alignment-in-a-static-spacetime)
- [Radiation-era adiabatic potentials with free-streaming neutrinos](linear-cosmological-perturbation-theory.md#radiation-era-adiabatic-potentials-with-free-streaming-neutrinos)
- [Riemannian Penrose inequality](black-hole.md#riemannian-penrose-inequality)
- [Stress-energy tensor](stress-energy-tensor.md)
- [Strong energy condition](stress-energy-tensor.md#strong-energy-condition)
- [Superhorizon radiation-era entropy integration constants](linear-cosmological-density-perturbation.md#superhorizon-radiation-era-entropy-integration-constants)
- [Two-dimensional general relativity](riemann-curvature-tensor.md#two-dimensional-general-relativity)
- [Vacuum Einstein equations](#vacuum-einstein-equations)
