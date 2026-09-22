# Paper 49

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_49.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_49.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
    - [iv](#3/b/iv)
      - [Solution](#3/b/iv/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $\phi_s$ be the [local flow](../../../differential-geometry.md#local-flow) of the smooth [vector field](../../../calculus.md#vector-field) $X$, with $\phi_0=\mathrm{id}$ and $\frac{d}{ds}\phi_s(p)=X_{\phi_s(p)}$. The [flow definition of the Lie derivative of a tensor field](../../../fiber-bundle.md#flow-definition-of-the-lie-derivative-of-a-tensor-field) is

$$
\boxed{(\mathcal L_XT)_p=\left.\frac{d}{ds}\right|_{s=0}(\phi_s^*T)_p.}
$$

For a [tensor field](../../../fiber-bundle.md#tensor-field) of type $(r,s)$, the [mixed tensor pullback](../../../geometry-and-topology.md#pullback-of-a-mixed-tensor-by-a-diffeomorphism) transports the tensor at $\phi_s(p)$ back to $p$: it applies $(d\phi_s)_p^{-1}$ to every contravariant factor and $(d\phi_s)_p^*$ to every covariant factor. Thus every difference quotient belongs to the same tensor space at $p$. This definition gives another tensor field of the same type and uses no choice of [affine connection](../../../fiber-bundle.md#affine-connection). The [tensor Lie derivative](../../../fiber-bundle.md#lie-derivative-of-a-tensor-field) is defined wherever the [local flow](../../../differential-geometry.md#local-flow) exists, including points where $X$ vanishes.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), the differential and its inverse preserve the natural pairing of a [vector](../../../vector-space.md#vector) with a [covector](../../../linear-algebra.md#covector). Consequently the [mixed tensor pullback](../../../geometry-and-topology.md#pullback-of-a-mixed-tensor-by-a-diffeomorphism) commutes with every [tensor contraction](../../../linear-algebra.md#tensor-contraction) $C$:

$$
\phi_s^*(CT)=C(\phi_s^*T).
$$

Differentiating at zero gives $\mathcal L_X(CT)=C(\mathcal L_XT)$. The [mixed tensor pullback](../../../geometry-and-topology.md#pullback-of-a-mixed-tensor-by-a-diffeomorphism) also preserves [tensor products](../../../linear-algebra.md#tensor-product), so

$$
\phi_s^*(S\otimes T)=\phi_s^*S\otimes\phi_s^*T.
$$

The ordinary [product rule](../../../calculus.md#product-rule) for differentiation therefore yields

$$
\boxed{\mathcal L_X(S\otimes T)=(\mathcal L_XS)\otimes T+S\otimes(\mathcal L_XT).}
$$

This proves the contraction and [Leibniz rule](../../../calculus.md#leibniz-rule) properties for all smooth generators, without needing straightening coordinates.

The suggested [flow-box theorem](../../../differential-geometry.md#straightening-theorem) applies locally only where $X\ne0$. For example $X=x\partial_x$ vanishes at $x=0$, so it cannot equal a coordinate basis vector there. Its local flow is nevertheless $\phi_s(x)=e^sx$ and $\phi_s^*dx=e^s dx$, giving $\mathcal L_Xdx=dx$ even at that zero. This [Lie derivative at a zero of its generator](../../../fiber-bundle.md#lie-derivative-at-a-zero-of-its-generator) illustrates why the general flow proof is needed to cover every point.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For a smooth [function](../../../function.md), [pullback of a smooth function](../../../differential-geometry.md#pullback-of-a-smooth-function) is composition. The [chain rule](../../../calculus.md#chain-rule) gives

$$
\boxed{\mathcal L_Xf=\left.\frac{d}{ds}\right|_0f(\phi_s(p))=X(f).}
$$

For a [vector field](../../../calculus.md#vector-field) $Y$, use any local coordinates. To first order,

$$
\phi_s^\mu(x)=x^\mu+sX^\mu(x)+O(s^2),\qquad
(d\phi_s)^{-1\mu}{}_{\nu}=\delta^\mu{}_{\nu}-s\partial_\nu X^\mu+O(s^2).
$$

Multiplying this inverse differential by $Y(\phi_s(x))$ gives

$$
(\phi_s^*Y)^\mu=Y^\mu+s\bigl(X^\nu\partial_\nu Y^\mu-Y^\nu\partial_\nu X^\mu\bigr)+O(s^2).
$$

Thus

$$
\boxed{\mathcal L_XY=[X,Y],\qquad
[X,Y]^\mu=X^\nu\partial_\nu Y^\mu-Y^\nu\partial_\nu X^\mu.}
$$

This is the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields), whose action on a function is $X(Yf)-Y(Xf)$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Write the [covector field](../../../differential-form.md#one-form) as $\omega=\omega_\mu dx^\mu$. From the contraction and [product rule](../../../calculus.md#product-rule) properties,

$$
(\mathcal L_X\omega)(Y)=X(\omega(Y))-\omega([X,Y]).
$$

Take $Y=\partial_\mu$. The [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) is $[X,\partial_\mu]=-(\partial_\mu X^\nu)\partial_\nu$, so

$$
\boxed{(\mathcal L_X\omega)_\mu
=X^\nu\partial_\nu\omega_\mu+\omega_\nu\partial_\mu X^\nu.}
$$

Equivalently, the covariant-factor contribution comes from $\mathcal L_Xdx^\mu=dX^\mu=(\partial_\nu X^\mu)dx^\nu$. The formula holds in any [coordinate basis](../../../differential-geometry.md#coordinate-basis) and is the one-form case of the [coordinate tensor Lie derivative](../../../fiber-bundle.md#coordinate-tensor-lie-derivative).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Expand $T=T^\mu{}_{\nu}\,\partial_\mu\otimes dx^\nu$. Using the [tensor Lie derivative](../../../fiber-bundle.md#lie-derivative-of-a-tensor-field) of functions, vectors and covectors and its [Leibniz rule](../../../calculus.md#leibniz-rule) gives

$$
\boxed{(\mathcal L_XT)^\mu{}_{\nu}
=X^\rho\partial_\rho T^\mu{}_{\nu}
-T^\rho{}_{\nu}\partial_\rho X^\mu
+T^\mu{}_{\rho}\partial_\nu X^\rho.}
$$

The contravariant slot has a minus sign and the covariant slot a plus sign.

For the [commutator identity for Lie derivatives](../../../fiber-bundle.md#commutator-identity-for-lie-derivatives), put $D=[\mathcal L_X,\mathcal L_Y]-\mathcal L_{[X,Y]}$. The commutator of two [tensor derivations](../../../fiber-bundle.md#tensor-derivation) is itself a [tensor derivation](../../../fiber-bundle.md#tensor-derivation), and $D$ commutes with [tensor contractions](../../../linear-algebra.md#tensor-contraction). On a function, $Df=XYf-YXf-[X,Y]f=0$. On a [vector field](../../../calculus.md#vector-field) $Z$,

$$
DZ=[X,[Y,Z]]-[Y,[X,Z]]-[[X,Y],Z]=0
$$

by the [Jacobi identity](../../../lie-algebra.md#jacobi-identity), which follows here by expanding the commutators of the operators $X,Y,Z$ acting on functions. For a type $(1,1)$ tensor, $T(Z)$ is a [vector field](../../../calculus.md#vector-field), and contraction compatibility gives

$$
0=D(T(Z))=(DT)(Z)+T(DZ)=(DT)(Z).
$$

As this holds for every $Z$, $DT=0$. Therefore

$$
\boxed{\mathcal L_X\mathcal L_YT-\mathcal L_Y\mathcal L_XT=\mathcal L_{[X,Y]}T.}
$$

The derivation argument also establishes the identity for arbitrary tensor types by applying it to covector–vector pairings and then to [tensor products](../../../linear-algebra.md#tensor-product).

## 2

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use $G=c=1$, select the retarded source field with no added homogeneous radiation, and work to leading order in the [weak-field approximation](../../../general-relativity.md#weak-field-approximation) and [long-wavelength source approximation](../../../general-relativity.md#long-wavelength-source-approximation). The [retarded fundamental solution](../../../distribution-theory.md#retarded-fundamental-solution) of the [Linearized Einstein equations](../../../general-relativity.md#linearized-einstein-equations) in [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity) is

$$
\bar h_{ij}(t,\mathbf x)=4\int\frac{T_{ij}(t-|\mathbf x-\mathbf x'|,\mathbf x')}{|\mathbf x-\mathbf x'|}\,d^3x'.
$$

For $r\gg d$, the denominator is $r$ to leading order. The delay is $t-r+\mathbf n\cdot\mathbf x'+O(d^2/r)$, where $\mathbf n=\mathbf x/r$. In the usual slowly evolving source regime, its characteristic time $\tau$ obeys $d/\tau\ll1$, so the source-size part of the delay is negligible:

$$
\bar h_{ij}(t,\mathbf x)\simeq\frac4r\int T_{ij}(t-r,\mathbf x')\,d^3x'.
$$

The [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation) equation $\partial_\mu T^{\mu\nu}=0$ is required at the approximation order used; it follows from the divergence of the gauge-fixed field equation. [Compact support](../../../function.md#compact-support) removes the [integration by parts](../../../calculus.md#integration-by-parts) surface terms. Since $T^{00}=T_{00}$ and $T^{ij}=T_{ij}$ in this signature,

$$
\dot I_{ij}=\int(T^{0i}x^j+T^{0j}x^i)\,d^3x,
\qquad
\ddot I_{ij}=\int(T^{ji}+T^{ij})\,d^3x=2\int T_{ij}\,d^3x.
$$

Combining these identities gives the [retarded quadrupole field](../../../general-relativity.md#retarded-quadrupole-field)

$$
\boxed{\bar h_{ij}(t,\mathbf x)\simeq\frac2r\ddot I_{ij}(t-r).}
$$

For an ordinary nonrelativistic bound source, $\tau\sim d/v$ makes $d/\tau\sim v\ll1$. More generally the size relative to the variation timescale must also be small; speed alone does not exclude a rapidly varying small-amplitude motion.

The [radiation boundary condition for linearized gravity](../../../general-relativity.md#radiation-boundary-condition-for-linearized-gravity) is essential for a statement about the full field. Without it, the displayed implication is false: take $T_{\mu\nu}=0$ and add $\bar h_{11}=A\cos(k(t-z))$, $\bar h_{22}=-\bar h_{11}$, all other components zero. This weak plane [gravitational wave](../../../general-relativity.md#gravitational-wave) satisfies both the homogeneous wave equation and [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity), while every $I_{ij}$ is zero. The proved formula is for the retarded source contribution, with the standard slow-source qualification. Its transverse–traceless projection gives the physical radiative strain.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The separation of the stars is $2R$. [Newton's law of universal gravitation](../../../classical-mechanics.md#newton-s-law-of-universal-gravitation) and circular acceleration give

$$
M\Omega^2R=\frac{M^2}{(2R)^2},\qquad
\boxed{\Omega^2=\frac{M}{4R^3}.}
$$

To leading nonrelativistic order, the [mass density](../../../fluid-mechanics.md#density) is the sum of the two translated point-mass [Dirac delta distributions](../../../distribution-theory.md#dirac-delta-function). Thus

$$
I_{xx}=MR^2(1+\cos2\Omega t),\qquad
I_{yy}=MR^2(1-\cos2\Omega t),\qquad
I_{xy}=I_{yx}=MR^2\sin2\Omega t,
$$

with all components involving $z$ zero. The trace is $2MR^2$, a constant. Define the trace-free [mass quadrupole moment](../../../general-relativity.md#mass-quadrupole-moment) $Q_{ij}=I_{ij}-\delta_{ij}I_{kk}/3$; its third derivatives equal those of $I_{ij}$. If $K=8MR^2\Omega^3$, then

$$
\dddot Q_{xx}=K\sin2\Omega t,\qquad
\dddot Q_{yy}=-K\sin2\Omega t,\qquad
\dddot Q_{xy}=\dddot Q_{yx}=-K\cos2\Omega t.
$$

Both off-diagonal entries count in the contraction. Therefore $\dddot Q_{ij}\dddot Q_{ij}=2K^2=128M^2R^4\Omega^6$, independent of phase. The [quadrupole formula](../../../general-relativity.md#quadrupole-formula) gives the [equal-mass circular-binary quadrupole luminosity](../../../general-relativity.md#equal-mass-circular-binary-quadrupole-luminosity)

$$
\boxed{\langle P\rangle=\frac{128}{5}M^2R^4\Omega^6=\frac{2M^5}{5R^5}.}
$$

Restoring units, $\Omega^2=GM/(4R^3)$ and

$$
\boxed{\langle P\rangle=\frac{2G^4M^5}{5c^5R^5}.}
$$

Here $R$ is each star's radius about the centre of mass, not the separation. The rest-frame prescription supplies the leading [mass density](../../../fluid-mechanics.md#density); a moving star does not still have zero momentum density and spatial stress. The calculation uses the assumed [quadrupole formula](../../../general-relativity.md#quadrupole-formula) and the Newtonian orbit rather than imposing those rest-frame zeros on the moving binary.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

At fixed masses, the [equal-mass circular-binary quadrupole luminosity](../../../general-relativity.md#equal-mass-circular-binary-quadrupole-luminosity) grows as $R^{-5}$. The binary's Newtonian binding energy is $-GM^2/(4R)$, so reducing the separation increases both the binding and the radiated power. Equivalently, its luminosity scaling is

$$
P=\frac25\frac{c^5}{G}\left(\frac{GM}{Rc^2}\right)^5,
$$

which makes the importance of [orbital compactness](../../../general-relativity.md#orbital-compactness) explicit.

Ordinary extended stars cannot remain separate at very small orbital radii: contact, mass transfer and [tidal disruption](../../../classical-mechanics.md#tidal-disruption) intervene. A [neutron star](../../../stellar-astrophysics.md#neutron-star) or [black hole](../../../general-relativity.md#black-hole) can remain a compact orbiting object down to separations of order a few gravitational radii, allowing high orbital speeds, rapidly changing [mass quadrupole moments](../../../general-relativity.md#mass-quadrupole-moment) and strong [gravitational waves](../../../general-relativity.md#gravitational-wave). Thus compact, tightly bound binaries are especially efficient emitters. The Newtonian [quadrupole formula](../../../general-relativity.md#quadrupole-formula) explains the scaling; precision predictions near merger require relativistic dynamics, where that approximation itself ceases to be reliable.

## 3

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Write $h_{ab}=\delta g_{ab}$ and $C^a{}_{bc}=\delta\Gamma^a{}_{bc}$. The difference between two [affine connections](../../../fiber-bundle.md#affine-connection) is a tensor, so its infinitesimal change $C$ is a type $(1,2)$ [tensor field](../../../fiber-bundle.md#tensor-field). Both [affine connections](../../../fiber-bundle.md#affine-connection) are [torsion-free](../../../fiber-bundle.md#torsion-free-connection), giving $C^a{}_{bc}=C^a{}_{cb}$. Varying [metric compatibility](../../../fiber-bundle.md#metric-compatibility) gives

$$
\nabla_c h_{ab}=g_{db}C^d{}_{ca}+g_{ad}C^d{}_{cb}.
$$

Lower the first index of $C$. Add the versions with derivatives $b,c$ and subtract the one with derivative $d$; the lower-slot symmetry cancels the unwanted terms, leaving

$$
\nabla_bh_{dc}+\nabla_ch_{db}-\nabla_dh_{bc}=2g_{da}C^a{}_{bc}.
$$

Therefore

$$
\boxed{\delta\Gamma^a{}_{bc}=\frac12g^{ad}
(\nabla_ch_{db}+\nabla_bh_{dc}-\nabla_dh_{bc}).}
$$

All [covariant derivatives](../../../general-relativity.md#covariant-derivative) use the original [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). The PDF has $\nabla_bh_{dc}$ as its second term; the converted TeX's $\nabla_dh_{dc}$ is a transcription error.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Adopt the printed [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) convention and contract $R_{ab}=R^c{}_{acb}$. At an arbitrary point choose [normal coordinates](../../../general-relativity.md#normal-coordinates) for the original [metric tensor](../../../general-relativity.md#metric-tensor). There the original connection coefficients vanish. Varying the coordinate curvature formula leaves

$$
\delta R^a{}_{bcd}=\partial_c C^a{}_{bd}-\partial_d C^a{}_{bc}.
$$

At that point these partial derivatives equal the [covariant derivatives](../../../general-relativity.md#covariant-derivative) of the tensor $C$. Both sides are tensors, so the result is valid in every coordinate system:

$$
\delta R^a{}_{bcd}=\nabla_c C^a{}_{bd}-\nabla_d C^a{}_{bc}.
$$

Contracting its first and third indices proves the [Palatini identity](../../../general-relativity.md#palatini-identity)

$$
\boxed{\delta R_{ab}=\nabla_c\delta\Gamma^c{}_{ab}-\nabla_b\delta\Gamma^c{}_{ac}.}
$$

The normal-coordinate argument is applied independently at every point; it does not assume a flat background or set derivatives of the original connection to zero.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

Variation of the [inverse metric](../../../general-relativity.md#inverse-metric) relation $g^{ac}g_{cb}=\delta^a{}_b$ gives $\delta g^{ab}=-h^{ab}$. Hence the [metric variation of scalar curvature](../../../general-relativity.md#metric-variation-of-scalar-curvature) is

$$
\delta R=-R^{ab}h_{ab}+g^{ab}\delta R_{ab}.
$$

Put $h=g^{ab}h_{ab}$. The connection variation gives the contractions

$$
g^{ab}C^c{}_{ab}=\nabla_a h^{ca}-\frac12\nabla^c h,
\qquad C^c{}_{ac}=\frac12\nabla_a h.
$$

Using [metric compatibility](../../../fiber-bundle.md#metric-compatibility) and the [Palatini identity](../../../general-relativity.md#palatini-identity),

$$
g^{ab}\delta R_{ab}=\nabla_c\nabla_a h^{ca}-\nabla_c\nabla^c h.
$$

Renaming dummy indices gives

$$
\boxed{\delta R=-R^{ab}h_{ab}+\nabla^a\nabla^b h_{ab}
-\nabla^c\nabla_c(g^{ab}h_{ab}).}
$$

No interchange of covariant derivatives on a tensor is needed in this derivation, so no hidden curvature-commutator term is discarded.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Take compactly supported [metric variations](../../../general-relativity.md#metric-variation), or impose [boundary conditions](../../../differential-equation.md#boundary-condition) that remove the [integration by parts](../../../calculus.md#integration-by-parts) terms. Let $F=f'(R)$ and $\Box=\nabla^a\nabla_a$. Since $\delta\sqrt{-g}=\frac12\sqrt{-g}\,g^{ab}h_{ab}$, the gravitational action varies as

$$
\delta S_g=\int\sqrt{-g}\left[
\left(\frac12f g^{ab}-F R^{ab}\right)h_{ab}
+F\left(\nabla^a\nabla^b h_{ab}-\Box h\right)\right]d^4x.
$$

Applying [integration by parts](../../../calculus.md#integration-by-parts) twice to the derivative terms gives

$$
\delta S_g=-\int\sqrt{-g}\,E^{ab}h_{ab}\,d^4x,\qquad
\boxed{E_{ab}=F R_{ab}-\frac12f g_{ab}-\nabla_a\nabla_bF+g_{ab}\Box F.}
$$

For the usual [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) definition $T_{ab}=-2(-g)^{-1/2}\delta S_m/\delta g^{ab}$, varying the covariant [metric tensor](../../../general-relativity.md#metric-tensor) gives $\delta S_m=\frac12\int\sqrt{-g}\,T^{ab}h_{ab}\,d^4x$. Thus the action's stated normalization implies

$$
\boxed{E_{ab}=\frac12T_{ab}.}
$$

There is no implicit $1/(16\pi)$ in this gravitational action. This is the [normalization of the metric f(R) field equation](../../../general-relativity.md#normalization-of-the-metric-f-r-field-equation), rather than the commonly normalized version with $8\pi T_{ab}$ on the right.

Finally, the [chain rule](../../../calculus.md#chain-rule) gives $\nabla_a\nabla_bF=f''\nabla_a\nabla_bR+f^{(3)}\nabla_aR\nabla_bR$ and $\Box F=f''\Box R+f^{(3)}(\nabla R)^2$. Substitution yields

$$
\boxed{E_{ab}=f'R_{ab}-f''\nabla_a\nabla_bR-f^{(3)}\nabla_aR\nabla_bR
+\left(-\frac12f+f''\Box R+f^{(3)}\nabla_cR\nabla^cR\right)g_{ab}.}
$$

This is a metric [f(R) gravity](../../../general-relativity.md#f-r-gravity) variation: the connection is always the Levi-Civita connection of the varied [metric tensor](../../../general-relativity.md#metric-tensor), not an independent variable.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The pure gravitational action is invariant under [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism). An infinitesimal diffeomorphism generated by a compactly supported [vector field](../../../calculus.md#vector-field) $\xi$ changes the metric by its [tensor Lie derivative](../../../fiber-bundle.md#lie-derivative-of-a-tensor-field),

$$
\delta g_{ab}=\mathcal L_\xi g_{ab}=\nabla_a\xi_b+\nabla_b\xi_a.
$$

Using symmetry of $E^{ab}$ and the variational expression already derived,

$$
0=\delta_\xi S_g=-2\int\sqrt{-g}\,E^{ab}\nabla_a\xi_b\,d^4x
=2\int\sqrt{-g}\,(\nabla_aE^{ab})\xi_b\,d^4x.
$$

As $\xi_b$ is arbitrary, the [off-shell metric divergence identity](../../../general-relativity.md#diffeomorphism-identity-for-a-metric-action) is

$$
\boxed{\nabla^aE_{ab}=0.}
$$

This [Noether identity](../../../general-relativity.md#noether-identity) follows for every [metric tensor](../../../general-relativity.md#metric-tensor) without imposing either the gravitational field equation or the matter equations. It is a consequence of the metric action's diffeomorphism invariance, not a conclusion requiring a long component calculation.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

In four dimensions, [Lovelock's theorem](../../../general-relativity.md#lovelock-s-theorem) restricts a local natural symmetric divergence-free metric tensor with at most second derivatives of the metric to a constant linear combination of the [Einstein tensor](../../../general-relativity.md#einstein-tensor) and the metric. A generic nonlinear [f(R) gravity](../../../general-relativity.md#f-r-gravity) equation contains $\nabla_a\nabla_bf'(R)$: the [Ricci scalar](../../../general-relativity.md#ricci-scalar) already has second metric derivatives, so this term generally introduces fourth metric derivatives. It therefore violates the second-order hypothesis, although it remains covariant, symmetric and divergence-free.

The exception must be stated. For $f(R)=aR+b$, the same tensor reduces to

$$
E_{ab}=aG_{ab}-\frac b2g_{ab},
$$

which is precisely of Lovelock form. In particular, **$f(R)=R$ is a counterexample to a blanket claim that the theorem never applies**. The intended exclusion concerns generic nonlinear $f$, with $f''$ not identically zero. Restricting attention to a special constant-curvature solution of a nonlinear theory does not turn its off-shell equations into a universally second-order metric tensor.

<h4 id="3/b/iv">iv</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/b/iv)

A four-dimensional vacuum Einstein solution with the fixed [cosmological constant](../../../cosmology.md#cosmological-constant) $\Lambda$ has $R_{ab}=\Lambda g_{ab}$ and $R=4\Lambda$, constant. Thus every derivative of $f'(R)$ vanishes and

$$
E_{ab}=\left(\Lambda f'(4\Lambda)-\frac12f(4\Lambda)\right)g_{ab}.
$$

The [metric tensor](../../../general-relativity.md#metric-tensor) is nondegenerate, so this is zero precisely when

$$
\boxed{f(4\Lambda)=2\Lambda f'(4\Lambda).}
$$

This is the necessary and sufficient [Einstein metric condition in f(R) gravity](../../../general-relativity.md#einstein-metric-condition-in-f-r-gravity) for the specified $\Lambda$, and works for every such Einstein metric, even when its [Weyl tensor](../../../general-relativity.md#weyl-tensor) is nonzero. There is no need to divide by $f'(4\Lambda)$; the degenerate case where both $f$ and $f'$ vanish at that curvature is included. At $\Lambda=0$, the condition is simply $f(0)=0$.

If the intention is to demand the inclusion for every real $\Lambda$ simultaneously, the stronger functional condition is $Rf'(R)=2f(R)$ for all $R$. On each nonzero half-line it integrates to $f(R)=CR^2$; smoothness across zero makes the constants equal. Thus the all-$\Lambda$ version gives **$f(R)=CR^2$**, including $C=0$. This stronger reading is distinct from fixing one cosmological constant.

## 4

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Treat the printed $e^\mu$ as an [orthonormal coframe](../../../general-relativity.md#orthonormal-coframe-in-spacetime), with frame metric $\eta=\operatorname{diag}(-1,1,1,1)$. Work on a patch $z\ne0$ and $F=1-\alpha z^3>0$, so the given real coframe exists. Define $f=\sqrt F$ and $A=zf'-f$. The [exterior derivatives](../../../differential-form.md#exterior-derivative) are

$$
de^0=A e^3\wedge e^0,\qquad
de^1=-f e^3\wedge e^1,\qquad
de^2=-f e^3\wedge e^2,\qquad de^3=0.
$$

The [connection 1-forms](../../../connection-1-form.md) satisfying [Cartan's first structure equation](../../../connection-1-form.md#cartan-s-first-structure-equation) and [metric compatibility](../../../fiber-bundle.md#metric-compatibility) are

$$
\boxed{\omega^0{}_3=\omega^3{}_0=Ae^0,\qquad
\omega^1{}_3=-fe^1,\quad\omega^3{}_1=fe^1,\qquad
\omega^2{}_3=-fe^2,\quad\omega^3{}_2=fe^2.}
$$

All other forms vanish. With a Lorentzian frame, it is the lowered forms $\omega_{ab}=\eta_{ac}\omega^c{}_b$ that are antisymmetric; the two mixed time–space forms are equal. These displayed forms solve the torsion-free structure equation, and uniqueness of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) identifies them as the required connection.

Apply [Cartan's second structure equation](../../../connection-1-form.md#cartan-s-second-structure-equation). For example,

$$
\Theta^0{}_3=d(Ae^0)=-(zfA'+A^2)e^0\wedge e^3,
\qquad
\Theta^0{}_1=\omega^0{}_3\wedge\omega^3{}_1=Af e^0\wedge e^1.
$$

The remaining derivatives give $\Theta^1{}_3=Af e^1\wedge e^3$ and $\Theta^1{}_2=-f^2e^1\wedge e^2$, with analogous forms for index 2. Put $q=\alpha z^3$ and $B=1+q/2$. From $f^2=1-q$,

$$
Af=zf f'-f^2=-B,\qquad zfA'+A^2=F.
$$

Therefore all six independent [curvature 2-forms](../../../connection-1-form.md#curvature-2-form) are

$$
\boxed{\begin{aligned}
\Theta^0{}_1&=-B e^0\wedge e^1,&\Theta^0{}_2&=-B e^0\wedge e^2,\\
\Theta^0{}_3&=-F e^0\wedge e^3,&\Theta^1{}_2&=-F e^1\wedge e^2,\\
\Theta^1{}_3&=-B e^1\wedge e^3,&\Theta^2{}_3&=-B e^2\wedge e^3.
\end{aligned}}
$$

The other six are fixed by $\Theta^b{}_a=-\eta_{aa}\eta_{bb}\Theta^a{}_b$ for $a\ne b$, with no sum: equal for time–space pairs and opposite for spatial pairs. All diagonal forms are zero. The [Lorentzian connection-form antisymmetry](../../../connection-1-form.md#lorentzian-connection-form-antisymmetry) is essential to these signs.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use the convention $\Theta^a{}_b=\frac12R^a{}_{bcd}e^c\wedge e^d$ and $R_{ab}=R^c{}_{acb}$. Each independent two-form has only one coordinate-plane wedge, so the [Ricci tensor](../../../general-relativity.md#ricci-tensor) is diagonal. Contracting the six coefficients gives

$$
R_{00}=2B+F,\qquad R_{11}=R_{22}=R_{33}=-(2B+F).
$$

But $2B+F=2(1+q/2)+(1-q)=3$, so

$$
\boxed{R_{ab}=-3\eta_{ab},\qquad R=-12,\qquad G_{ab}=3\eta_{ab}.}
$$

In coordinate-independent form, $R_{\mu\nu}=-3g_{\mu\nu}$. Thus the vacuum [Einstein field equations](../../../general-relativity.md#einstein-field-equations) $G_{\mu\nu}+\Lambda g_{\mu\nu}=0$ hold with

$$
\boxed{\Lambda=-3.}
$$

The curvature radius is one in the metric's normalization. The parameter $\alpha$ changes the individual [curvature 2-forms](../../../connection-1-form.md#curvature-2-form) but cancels from their Ricci contraction. For $\alpha=0$ this is [Anti-de Sitter spacetime](../../../general-relativity.md#anti-de-sitter-spacetime); for nonzero $\alpha$ it is the [planar Einstein metric with cubic radial function](../../../general-relativity.md#planar-einstein-metric-with-cubic-radial-function), with a nontrivial [Weyl tensor](../../../general-relativity.md#weyl-tensor) rather than universally constant sectional curvature. The result is local on regular coordinate patches; a zero of $F$ invalidates this particular static coframe, not the tensor equation in a suitable regular extension.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
