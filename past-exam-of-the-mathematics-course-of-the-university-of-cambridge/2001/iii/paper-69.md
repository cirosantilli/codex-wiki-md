# Paper 69

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper69.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper69.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use $G=\hbar=c_{\rm light}=k_B=1$ and normalize the stationary time at infinity. For a regular stationary, asymptotically flat electrovacuum [black hole](../../../general-relativity.md#black-hole), the [Kerr-Newman metric](../../../general-relativity.md#kerr-newman-metric) has

$$
a=\frac JM,\qquad d=\sqrt{M^2-Q^2-a^2},\qquad
r_\pm=M\pm d,\qquad
D_H=r_+^2+a^2=2M^2-Q^2+2Md.
$$

Initially assume $M>0$ and $d>0$, so the outer [Killing horizon](../../../general-relativity.md#killing-horizon) is nondegenerate. Its [surface gravity](../../../general-relativity.md#surface-gravity), angular velocity, electric potential and area are

$$
\kappa=\frac{r_+-r_-}{2D_H}=\frac d{D_H},\qquad
\Omega_H=\frac a{D_H},\qquad
\Phi_H=\frac{Qr_+}{D_H},\qquad
A_H=4\pi D_H.
$$

These are horizon quantities for the generator $\chi=\partial_t+\Omega_H\partial_\phi$.

The [laws of black-hole mechanics](../../../general-relativity.md#laws-of-black-hole-mechanics) provide the first reason to regard $\kappa$ and area as thermodynamic variables. The [Zeroth law of black-hole mechanics](../../../general-relativity.md#zeroth-law-of-black-hole-mechanics) makes $\kappa$ constant on an equilibrium horizon. The [first law for the Kerr-Newman family](../../../general-relativity.md#first-law-for-the-kerr-newman-family) reads

$$
dM=\frac{\kappa}{8\pi}\,dA_H+\Omega_H\,dJ+\Phi_H\,dQ.
$$

For example, write the horizon relation as $M=(r_+^2+a^2+Q^2)/(2r_+)$ and use $J=Ma$; differentiating eliminates $dr_+$ and $da$ to give this law. The last two terms are rotational and electric work. The classical [second law of black-hole mechanics](../../../general-relativity.md#second-law-of-black-hole-mechanics) says that area cannot decrease under the [null energy condition](../../../general-relativity.md#null-energy-condition) and appropriate global horizon assumptions. The [third law of black-hole mechanics](../../../general-relativity.md#third-law-of-black-hole-mechanics) concerns unattainability of a zero-surface-gravity regular horizon by a finite physical process.

This analogy alone does not determine the [temperature](../../../thermodynamics.md#temperature) scale: if entropy were $\eta A_H$, the first law would only give $T=\kappa/(8\pi\eta)$. The decisive input is [quantum field theory](../../../quantum-field-theory.md) in the collapsing or stationary background. In a collapse vacuum that is regular for freely falling observers, the late outgoing retarded time $u$ and a regular affine null coordinate $U$ satisfy the [Hawking exponential ray map](../../../general-relativity.md#hawking-exponential-ray-map)

$$
U=-C e^{-\kappa u},\qquad C>0.
$$

An outgoing mode $e^{-i\omega u}$ therefore behaves as $(-U/C)^{i\omega/\kappa}$. Continuing this power through the horizon changes its amplitude by the factor $e^{-\pi\omega/\kappa}$. Its positive- and negative-frequency decomposition consequently has the [thermal ratio of Hawking Bogoliubov coefficients](../../../general-relativity.md#thermal-ratio-of-hawking-bogoliubov-coefficients)

$$
\frac{|\beta_\omega|^2}{|\alpha_\omega|^2}=e^{-2\pi\omega/\kappa}.
$$

Combining that ratio with bosonic normalization $|\alpha|^2-|\beta|^2=1$ gives a Planck occupation $1/(e^{2\pi\omega/\kappa}-1)$. The fermionic normalization instead gives the corresponding Fermi factor. Thus [Hawking radiation](../../../general-relativity.md#hawking-radiation) fixes

$$
T_H=\frac{\kappa}{2\pi}.
$$

For rotating charged modes, the horizon energy is $\widetilde\omega=\omega-m_\phi\Omega_H-q\Phi_H$, so the emission spectrum contains the same [temperature](../../../thermodynamics.md#temperature) with angular-momentum and charge chemical potentials. Exterior scattering supplies [greybody factors](../../../general-relativity.md#greybody-factor); it changes the received flux, not the horizon [temperature](../../../thermodynamics.md#temperature). Superradiant bosonic modes require the usual signed absorption factor, and a globally regular thermal bath need not exist throughout an asymptotically flat rotating exterior. The collapse-state emission argument is the relevant one.

A complementary check is the [Euclidean black-hole regularity condition](../../../general-relativity.md#euclidean-black-hole-regularity-condition). The local corotating nondegenerate horizon geometry is Rindler-like:

$$
ds_E^2\simeq d\rho^2+\kappa^2\rho^2d\tau^2+\text{horizon metric}.
$$

Smoothness at $\rho=0$ requires $\tau$ to have period $2\pi/\kappa$. Imaginary-time periodicity is precisely inverse [temperature](../../../thermodynamics.md#temperature), agreeing with the radiation calculation. Matching the resulting [temperature](../../../thermodynamics.md#temperature) to the first law fixes the [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy) to $S=A_H/4$. The [generalized second law](../../../general-relativity.md#generalized-second-law) then uses $S_{\rm outside}+A_H/4$: the classical area theorem alone does not apply to the negative-energy quantum flux responsible for evaporation.

Substitution gives the [Kerr-Newman horizon temperature](../../../general-relativity.md#kerr-newman-horizon-temperature)

$$
\boxed{T_H=\frac{\sqrt{M^2-Q^2-J^2/M^2}}
{2\pi\left(2M^2-Q^2+2M\sqrt{M^2-Q^2-J^2/M^2}\right)}.}
$$

It reduces to $1/(8\pi M)$ for a [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime). The nonextremal limit towards $d=0$ gives zero [temperature](../../../thermodynamics.md#temperature). At exact extremality the Euclidean horizon is degenerate, so the elementary conical-period argument does not itself fix a period; zero [temperature](../../../thermodynamics.md#temperature) here is the limiting semiclassical result. The reasoning assumes ordinary Einstein–Maxwell dynamics, a regular horizon, the stated normalization at infinity and a regime where quantum fields on a slowly evolving classical geometry are a useful approximation. The mechanical laws, radiation spectrum and Euclidean regularity agree under these assumptions, which is substantially stronger evidence than the classical analogy alone.

## 2

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [mass](../../../classical-mechanics.md#mass) statement needs a nonzero [parallel spinor](../../../connection-1-form.md#parallel-spinor) and an isolated [asymptotically flat spacetime](../../../general-relativity.md#asymptotically-flat-spacetime); the zero [spinor](../../../algebra.md#spinor) solves the equation on every geometry and cannot imply anything about [mass](../../../classical-mechanics.md#mass). Assume the usual complete regular spin initial data and [dominant energy condition](../../../general-relativity.md#dominant-energy-condition) used by the [positive energy theorem](../../../general-relativity.md#positive-energy-theorem), with the [spinor](../../../algebra.md#spinor) tending to a nonzero constant $\epsilon_\infty$ at infinity. Let $V^a=\bar\epsilon\gamma^a\epsilon$ be its future causal [Dirac current](../../../quantum-field-theory.md#dirac-current).

The [Nester two-form](../../../general-relativity.md#nester-two-form) can be written, up to normalization, as

$$
B^{ab}=\bar\epsilon\gamma^{abc}\nabla_c\epsilon
-\overline{\nabla_c\epsilon}\,\gamma^{abc}\epsilon.
$$

It is bilinear in $\epsilon$ and $\nabla\epsilon$. For a spacetime-parallel [spinor](../../../algebra.md#spinor) it vanishes identically, and hence so does its asymptotic flux. The [ADM boundary term of the Nester two-form](../../../general-relativity.md#adm-boundary-term-of-the-nester-two-form) identifies that flux, up to a fixed positive normalization, as

$$
E V_\infty^0-P_iV_\infty^i=0.
$$

The [positive energy theorem](../../../general-relativity.md#positive-energy-theorem) gives $E\geq|P|$. Since $V_\infty$ is nonzero future causal, a future timelike ADM momentum would have strictly positive contraction with it. Consequently the ADM momentum is zero or null:

$$
\boxed{M_{\rm ADM}=\sqrt{E^2-|P|^2}=0.}
$$

In a rest frame, when one exists, this immediately says $E=0$. The usual regular asymptotically flat rigidity conclusion also excludes a nontrivial null-momentum configuration and gives flat initial data. This is the spinorial boundary-charge proof, not an inference that every Lorentzian manifold with a [parallel spinor](../../../connection-1-form.md#parallel-spinor) is flat. Without the asymptotic and global hypotheses the local [spinor](../../../algebra.md#spinor) equation alone does not define, let alone determine, an ADM [mass](../../../classical-mechanics.md#mass).

For the modified connection, it is important to fix the [Clifford algebra](../../../algebra.md#clifford-algebra) normalization. Write

$$
\{\gamma_a,\gamma_b\}=2s\,g_{ab}I,\qquad
\gamma_{ab}=\frac12[\gamma_a,\gamma_b],\qquad s>0.
$$

The compatible [spinor curvature identity](../../../connection-1-form.md#spinor-curvature-identity) is

$$
[\nabla_a,\nabla_b]=\frac1{4s}R_{abcd}\gamma^{cd}.
$$

Indeed, rescaling conventional [gamma matrices](../../../algebra.md#gamma-matrices) by $\sqrt s$ rescales $\gamma_{ab}$ by $s$, while leaving the geometric spin connection unchanged. Since the connection is torsion-free and $\nabla\gamma=0$, the cross terms cancel in the modified commutator:

$$
[D_a,D_b]\epsilon=
\left(\frac1{4s}R_{abcd}\gamma^{cd}+c^2[\gamma_a,\gamma_b]\right)\epsilon.
$$

Thus the [Killing-spinor integrability with rescaled gamma matrices](../../../connection-1-form.md#killing-spinor-integrability-with-rescaled-gamma-matrices) equation is

$$
\boxed{(R_{abcd}\gamma^{cd}+8s c^2\gamma_{ab})\epsilon=0.}
$$

A factor of two in the convention for antisymmetrization multiplies the whole zero equation and cannot change this relative coefficient.

The two printed coefficients are consistent with $s=2$, namely $\{\gamma_a,\gamma_b\}=4g_{ab}I$. In that convention the displayed integrability equation becomes $R_{abcd}\gamma^{cd}+16c^2\gamma_{ab}=0$ on each solution. With the customary convention $s=1$, the coefficient is instead $8c^2$, and the final Ricci coefficient below is $-12c^2$. The PDF does not state its Clifford normalization, so these alternatives must be distinguished rather than mixing them.

In four spacetime dimensions the complex Dirac [spinor](../../../algebra.md#spinor) fibre has dimension four. Four independent solutions of $D\epsilon=0$ span that fibre at every point: a solution vanishing at one point vanishes everywhere by [parallel transport](../../../fiber-bundle.md#parallel-transport). Therefore the integrability matrix annihilates every [spinor](../../../algebra.md#spinor) and is the zero matrix. The six bivector matrices $\gamma^{cd}$ are linearly independent, as is seen by taking traces against them; their trace pairing is a nondegenerate multiple of the metric on two-forms. Expressing $\gamma_{ab}=g_{ac}g_{bd}\gamma^{cd}$ therefore gives

$$
R_{abcd}=-4s c^2(g_{ac}g_{bd}-g_{ad}g_{bc}).
$$

This proves that [maximal Killing spinors force constant negative curvature](../../../connection-1-form.md#maximal-killing-spinors-force-constant-negative-curvature), not merely an Einstein [Ricci tensor](../../../general-relativity.md#ricci-tensor). Contracting in four dimensions gives

$$
\boxed{R_{ab}=-12s c^2g_{ab}
=\begin{cases}-24c^2g_{ab},&s=2,\\-12c^2g_{ab},&s=1.\end{cases}}
$$

For $s=2$ this is the requested Einstein equation. Since $c>0$, its [Ricci tensor](../../../general-relativity.md#ricci-tensor) automatically has rank four; under the maximal-spinor hypothesis the additional rank assumption is redundant. If the stated four-dimensional solution space is interpreted directly as the pointwise kernel of the algebraic integrability equation, the same spanning and trace argument applies.

## 3

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Take $M>0$, set $b=Q^2/M$, and denote the squared areal radius by $C(r)=r(r-b)$. The positive-area exterior has $r>b$. The stationary norm is $-f(r)$, where $f(r)=1-2M/r$, so its candidate [Killing horizon](../../../general-relativity.md#killing-horizon) is at $r=2M$. There it has area

$$
A_H=4\pi C(2M)=8\pi(2M^2-Q^2).
$$

A regular horizon must have $b<2M$. The [curvature singularity](../../../general-relativity.md#curvature-singularity) then lies strictly inside the horizon, and ingoing coordinates extend smoothly across it because $C(2M)>0$. In the future interior $f<0$, the gradient of $r$ is timelike and future causal curves move to decreasing $r$, rather than back to infinity. Thus the regular [black hole](../../../general-relativity.md#black-hole) condition is

$$
\boxed{M>0,\qquad Q^2<2M^2.}
$$

The equality case has zero horizon area and a curvature-singular null limiting surface. It is often included in the family as a singular extremal solution, but it is not a regular [black hole](../../../general-relativity.md#black-hole). If that limiting nomenclature is used, the family condition is $Q^2\leq2M^2$ with this essential qualification. This geometry has the same spherical form as the [magnetically charged dilaton black hole](../../../general-relativity.md#magnetically-charged-dilaton-black-hole); no unprinted field equation is needed for the horizon comparison.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For $M>0$ and $Q^2>2M^2$, the physical exterior starts at $r=b>2M$. Throughout it, $f>0$, so the putative zero of $f$ is not in the exterior and no regular horizon shields the [curvature singularity](../../../general-relativity.md#curvature-singularity). The normal to $r=b$ has positive limiting squared norm $g^{rr}=f(b)>0$, identifying a timelike singular boundary. Outgoing radial [null geodesics](../../../special-relativity.md#null-geodesic) obey $dr/dt=f(r)>0$ and escape from arbitrarily close to that boundary. Hence

$$
\boxed{Q^2>2M^2\quad\text{gives a timelike naked singularity}.}
$$

At $Q^2=2M^2$, the singular boundary coincides with $f=0$ and is null. There is no regular shielding horizon of positive area; this marginal singular extremal case must be separated from both the regular [black hole](../../../general-relativity.md#black-hole) and the supercritical timelike naked singularity. If “naked” is used simply to mean unshielded by a regular horizon, equality belongs on that side of the distinction, but its causal boundary is different.

The usual positive-mass restriction matters. For $M<0$, $f(r)>0$ at every positive radius and there is no positive-radius horizon; the central zero-area boundary at $r=0$ is singular and naked. For $Q=0$ its angular sectional curvature is $2M/r^3$, which diverges there. For $Q\ne0$, $C=r(r-b)$ with $b<0$, and the angular sectional curvature $[1-f(C')^2/(4C)]/C$ also diverges as $r\downarrow0$. The displayed family is undefined at $M=0$ with nonzero $Q$; its uncharged zero-mass limit is flat.

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The absorption question concerns the geometric-optics capture cross-section, assuming rays reaching the central singular boundary are absorbed. [Null geodesic](../../../special-relativity.md#null-geodesic) motion alone does not specify a wave boundary condition at a singularity.

By spherical symmetry choose an equatorial ray. Conservation of energy and [angular momentum](../../../classical-mechanics.md#angular-momentum) gives $E=f\dot t$, $L=C\dot\phi$, and null normalization gives

$$
\dot r^2=E^2-\frac{fL^2}{C}
=E^2\{1-B^2H(r)\},\qquad
B=\frac LE,\qquad
H(r)=\frac{f}{C}=\frac{r-2M}{r^2(r-b)}.
$$

Here $B$ is the [impact parameter](../../../classical-mechanics.md#impact-parameter) measured at infinity. A returning ray has an exterior turning point; capture occurs when none exists. The critical impact parameter obeys $B_c^2=1/\sup H$, and the cross-section is the area $\pi B_c^2$ in the incident impact-parameter plane.

For $Q=0$, $H=(r-2M)/r^3$ and

$$
H'(r)=-\frac{2(r-3M)}{r^4}.
$$

The maximum is at the unstable [photon sphere](../../../general-relativity.md#photon-sphere) $r=3M$, with $H=1/(27M^2)$. Therefore

$$
\boxed{B_c=3\sqrt3\,M,\qquad \sigma_{\rm abs}=27\pi M^2\quad(Q=0).}
$$

For $Q^2=2M^2$, cancellation for $r>2M$ gives $H=1/r^2$. There is no regular exterior circular photon orbit: the supremum occurs at the singular limiting surface, with $\sup H=1/(4M^2)$. Rays with $B>2M$ turn at $r=B$; those with $B<2M$ reach the central boundary. Thus the [extremal dilaton metric photon capture](../../../general-relativity.md#extremal-dilaton-metric-photon-capture) result is

$$
\boxed{B_c=2M,\qquad \sigma_{\rm abs}=4\pi M^2\quad(Q^2=2M^2).}
$$

The critical ray is a measure-zero boundary of the capture set. The finite capture cross-section is not the horizon area, which vanishes in this limit. Nor is it a claim about a low-frequency quantum absorption cross-section or an unspecified reflection law at the singularity.

## 4

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Assume an asymptotically flat [Reissner-Nordstrom spacetime](../../../general-relativity.md#reissner-nordstrom-spacetime), with $M>|Q|$, time normalized at infinity, and $G=\hbar=c_{\rm light}=k_B=1$. Put

$$
q=|Q|,\qquad r_\pm=M\pm\sqrt{M^2-q^2},\qquad
f(r)=\frac{(r-r_+)(r-r_-)}{r^2}.
$$

Near $r_+$, the Euclidean radial-time metric is $f'(r_+)(r-r_+)\,d\tau^2+dr^2/[f'(r_+)(r-r_+)]$. With $\rho=2\sqrt{(r-r_+)/f'(r_+)}$, it becomes

$$
d\rho^2+\left(\frac{f'(r_+)}2\right)^2\rho^2d\tau^2.
$$

The [Euclidean black-hole regularity condition](../../../general-relativity.md#euclidean-black-hole-regularity-condition) removes a conical defect only if $\tau$ has period $4\pi/f'(r_+)$. Therefore the [Reissner-Nordstrom Hawking temperature](../../../general-relativity.md#reissner-nordstrom-hawking-temperature) is

$$
\boxed{T=\frac{f'(r_+)}{4\pi}
=\frac{r_+-r_-}{4\pi r_+^2}
=\frac{\sqrt{M^2-q^2}}{2\pi(M+\sqrt{M^2-q^2})^2}.}
$$

Equivalently this is the [Reissner-Nordstrom horizon surface gravity](../../../general-relativity.md#reissner-nordstrom-horizon-surface-gravity) divided by $2\pi$. The derivation assumes a nondegenerate horizon; the value zero at $M=q$ is obtained by the nonextremal limit, not by imposing conical regularity directly on the degenerate geometry.

For fixed nonzero $q$, write $y=r_+/q\geq1$. The horizon equation gives

$$
\frac Mq=\frac12(y+y^{-1}),\qquad
qT=\frac1{4\pi}(y^{-1}-y^{-3}).
$$

The [mass](../../../classical-mechanics.md#mass) is increasing with $y>1$, and

$$
\frac{d(qT)}{dy}=\frac{3-y^2}{4\pi y^4}.
$$

Thus the [fixed-charge Reissner-Nordstrom temperature maximum](../../../general-relativity.md#fixed-charge-reissner-nordstrom-temperature-maximum) occurs at

$$
\boxed{r_+=\sqrt3\,q,\qquad
M_{\max}=\frac{2q}{\sqrt3},\qquad
T_{\max}=\frac1{6\sqrt3\,\pi q}.}
$$

The curve starts at zero at $M=q$, rises to this maximum, then falls as $1/(8\pi M)$ for large [mass](../../../classical-mechanics.md#mass). During evaporation from $M_0\gg q$, the [mass](../../../classical-mechanics.md#mass) moves from right to left: the [temperature](../../../thermodynamics.md#temperature) initially increases, reaches its maximum, and then decreases towards zero.

<a id="4/image-reissner-nordstrom-temperature-at-fixed-charge-its-maximum-and-the-evaporation-direction"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-69-temperature.png)

**[Figure 1](#4/image-reissner-nordstrom-temperature-at-fixed-charge-its-maximum-and-the-evaporation-direction). Reissner-Nordstrom temperature at fixed charge, its maximum and the evaporation direction**.

Under the printed thermal-emission cutoff, charged emission is absent throughout precisely when the entire [mass](../../../classical-mechanics.md#mass) path remains at or below the threshold:

$$
\boxed{m\geq T_{\max}\quad\Longleftrightarrow\quad
m|Q|\geq\frac1{6\sqrt3\,\pi}.}
$$

Equality is allowed because emission is assumed to require $T>m$, not merely $T=m$. The initial large [mass](../../../classical-mechanics.md#mass) ensures that the path includes the maximum.

With charge then conserved, neutral [Hawking radiation](../../../general-relativity.md#hawking-radiation) lowers the [mass](../../../classical-mechanics.md#mass) until the system approaches the [charge-preserving Reissner-Nordstrom evaporation endpoint](../../../general-relativity.md#charge-preserving-reissner-nordstrom-evaporation-endpoint):

$$
\boxed{M_{\rm final}=|Q|,\qquad T_{\rm final}=0,\qquad
A_{\rm final}=4\pi Q^2.}
$$

The limiting state is an [extremal black hole](../../../general-relativity.md#extremal-black-hole), rather than a neutral zero-mass endpoint. Exact attainment in finite time is not established: near extremality $T\sim\sqrt{M-q}/(\sqrt2\pi q^{3/2})$, and the ideal radiation rate tends to zero. The conclusion is within the assumed thermal cutoff model, which omits nonthermal charge creation and other quantum corrections. For $Q=0$, the Schwarzschild [temperature](../../../thermodynamics.md#temperature) instead grows without bound in the extrapolated model, so no finite $m$ satisfies the stated all-the-way [temperature](../../../thermodynamics.md#temperature) bound.

## 5

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Interpret $A$ first as an infinitesimal screen area transported along generators of a future [event horizon](../../../general-relativity.md#event-horizon), not as the total area of an arbitrary trapped surface. Horizon generators form an affinely parametrized, hypersurface-orthogonal [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence). The two-dimensional screen metric is positive definite. Its optical tensor has zero twist and decomposes as

$$
B_{AB}=\frac12\theta h_{AB}+\widehat\sigma_{AB},\qquad
\theta=\frac{A'}A,\qquad
\sigma^2=\frac12\widehat\sigma_{AB}\widehat\sigma^{AB}\geq0.
$$

The scalar here agrees with the supplied derivative definition: nullness and the affine geodesic equation remove the longitudinal terms in the contracted norm, leaving $B_{AB}B^{AB}-\theta^2/2$.

To derive the focusing equation, vary neighbouring geodesics and let $J$ be their screen Jacobi map. The [geodesic deviation](../../../general-relativity.md#geodesic-deviation) equation is $J''=-\mathcal R J$, where $\mathcal R_{AB}=R_{AcBd}p^cp^d$. Hence $B=J'J^{-1}$ satisfies $B'=-B^2-\mathcal R$. Taking its screen trace yields the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation)

$$
\theta'=-\frac12\theta^2-2\sigma^2-R_{ab}p^ap^b.
$$

Set $a=A^{1/2}$. Since $a'/a=\theta/2$, the [area-square-root optical focusing equation](../../../geodesic-congruence.md#area-square-root-optical-focusing-equation) is

$$
\boxed{\frac{a''}a=\frac12\theta'+\frac14\theta^2
=-\frac12R_{ab}p^ap^b-\sigma^2.}
$$

The PDF's plus sign before $\sigma^2$ is inconsistent with its own positive shear definition. This is an actual source error, not an antisymmetrization or curvature-sign convention.

For an explicit check, take a flat-space twist-free beam with screen Jacobi factors $1+\lambda$ and $1-\lambda$, for $|\lambda|<1$. Then

$$
A=1-\lambda^2,\qquad
\sigma^2=(1-\lambda^2)^{-2},\qquad
(A^{1/2})''=-(1-\lambda^2)^{-3/2}.
$$

Its Ricci term is zero, so the result equals $-\sigma^2A^{1/2}$ and has the opposite sign to the printed equation. This is [flat-space anisotropic beam shear focusing](../../../geodesic-congruence.md#flat-space-anisotropic-beam-shear-focusing).

Under the [null convergence condition](../../../general-relativity.md#null-convergence-condition) $R_{ab}p^ap^b\geq0$, the correct equation gives concavity of each local area square root. Equivalently $\theta'\leq-\theta^2/2$. If a horizon generator had $\theta(\lambda_0)=\theta_0<0$, integration gives a focal point within affine distance at most $2/|\theta_0|$. Such a generator could not remain on an [achronal boundary](../../../general-relativity.md#achronal-boundary) beyond the focal point. Under the usual global hypotheses that horizon generators remain regular and future complete, this contradicts their being generators of the [event horizon](../../../general-relativity.md#event-horizon). Hence $\theta\geq0$ and $A'=\theta A\geq0$. Integrating over the horizon patches, and including newly joining generators which can add area, proves [Hawking's area theorem](../../../general-relativity.md#hawking-s-area-theorem). Global predictability/completeness assumptions are essential; the local differential inequality alone is not a theorem about arbitrary trapped-surface areas.

For the [perfect fluid](../../../general-relativity.md#perfect-fluid) stress tensor, null contraction eliminates the pressure-metric term:

$$
T_{ab}p^ap^b=(\rho+p_{\rm fluid})(u_ap^a)^2.
$$

A nonzero null vector cannot be orthogonal to a timelike fluid velocity. Thus the [perfect-fluid null energy condition](../../../general-relativity.md#perfect-fluid-null-energy-condition) is precisely

$$
\boxed{\rho+p_{\rm fluid}\geq0.}
$$

Separate requirements $\rho\geq0$ or $p_{\rm fluid}\geq0$ are not needed for this null focusing argument. With the Einstein equation, $R_{ab}p^ap^b=8\pi T_{ab}p^ap^b$.

A [cosmological constant](../../../cosmology.md#cosmological-constant) contributes only a term proportional to $g_{ab}$, whose null contraction is zero:

$$
(G_{ab}+\Lambda g_{ab})p^ap^b=R_{ab}p^ap^b.
$$

Therefore **a nonzero [cosmological constant](../../../cosmology.md#cosmological-constant) does not change the fluid condition or the local area-focusing argument**, though it can change the global asymptotics and which horizons and completeness hypotheses are appropriate.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
