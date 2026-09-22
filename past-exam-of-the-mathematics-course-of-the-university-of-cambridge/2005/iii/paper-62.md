# Paper 62

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper62.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper62.pdf)

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

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use [geometrized units](../../../general-relativity.md#geometrized-units) $G=c=1$ and positive [mass](../../../classical-mechanics.md#mass) $M$. The [Schwarzschild metric](../../../general-relativity.md#schwarzschild-spacetime) initially describes an exterior region, not the whole [black hole](../../../general-relativity.md#black-hole):

$$
ds^2=-f(r)dt^2+f(r)^{-1}dr^2+r^2d\Omega^2,\qquad f(r)=1-\frac{2M}{r},\qquad r>2M.
$$

Here $r$ is the [areal radius](../../../general-relativity.md#areal-radius) and $t$ is [Schwarzschild time](../../../general-relativity.md#schwarzschild-time), normalized at infinity. We must distinguish a removable [coordinate singularity](../../../general-relativity.md#coordinate-singularity) from a genuine [curvature singularity](../../../general-relativity.md#curvature-singularity). The [Kretschmann scalar](../../../general-relativity.md#kretschmann-scalar) is

$$
R_{abcd}R^{abcd}=\frac{48M^2}{r^6}.
$$

It is finite at $r=2M$ and diverges at $r=0$. Thus $r=2M$ can be crossed in a better chart, whereas $r=0$ cannot be made a regular point by changing the [coordinate chart](../../../differential-geometry.md#manifold-chart).

First integrate the [Schwarzschild tortoise coordinate](../../../general-relativity.md#schwarzschild-tortoise-coordinate):

$$
\frac{dr_*}{dr}=\frac1f,\qquad r_*=r+2M\log\left|\frac r{2M}-1\right|.
$$

The radial metric becomes $f(-dt^2+dr_*^2)$. Set $v=t+r_*$; the [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates) give

$$
ds^2=-f\,dv^2+2\,dv\,dr+r^2d\Omega^2.
$$

The radial block has determinant minus one and smooth coefficients at $r=2M$, so it extends through the future [Schwarzschild event horizon](../../../general-relativity.md#schwarzschild-event-horizon). Its ingoing radial [null geodesics](../../../special-relativity.md#null-geodesic) have constant $v$, while the outgoing radial [null geodesics](../../../special-relativity.md#null-geodesic) obey $dr/dv=f/2$. In the future interior both future-directed radial null families decrease $r$; $r=0$ is therefore an unavoidable future boundary for causal motion there. The outgoing chart $u=t-r_*$ similarly gives $ds^2=-f\,du^2-2\,du\,dr+r^2d\Omega^2$, extending through the past horizon. A single one of these null charts does not display both horizons or the entire extension.

To regularize both horizons together, introduce [Kruskal–Szekeres coordinates](../../../general-relativity.md#kruskal-szekeres-coordinates) in the original exterior:

$$
u=t-r_*,\quad v=t+r_*,\qquad U=-e^{-u/(4M)},\quad V=e^{v/(4M)}.
$$

Then

$$
UV=\left(1-\frac r{2M}\right)e^{r/(2M)},\qquad
\boxed{ds^2=-\frac{32M^3}{r}e^{-r/(2M)}dU\,dV+r^2d\Omega^2.}
$$

For $r>0$ the right side defining $UV$ decreases monotonically from one to minus infinity. In fact its derivative is $-re^{r/(2M)}/(4M^2)$. Thus it determines a unique smooth $r=r(UV)$ wherever $UV<1$, including $UV=0$. At $r=2M$ the radial metric coefficient is finite and nonzero, proving actual regularity of both horizons and their intersection, rather than merely relabelling the old coordinate divergence. Allowing all real $U,V$ with $UV<1$ produces the simply connected [maximal analytic extension](../../../special-relativity.md#maximal-analytic-extension), the [Kruskal spacetime](../../../general-relativity.md#kruskal-spacetime).

There are four regions of the [Kruskal spacetime](../../../general-relativity.md#kruskal-spacetime). The original exterior is $U<0,V>0$; a second asymptotically flat exterior is $U>0,V<0$. The future [black hole](../../../general-relativity.md#black-hole) has $U>0,V>0$ and $0<r<2M$; the past [white hole](../../../general-relativity.md#white-hole) has $U<0,V<0$ and the same range of [areal radius](../../../general-relativity.md#areal-radius). The horizon branches are $U=0$ and $V=0$. Their intersection $U=V=0$ is a regular [bifurcation surface](../../../general-relativity.md#bifurcation-surface), a two-sphere of radius $2M$, not the centre of the spacetime. Each point of the radial diagram represents a symmetry two-sphere.

Put $T_K=(V+U)/2$ and $X_K=(V-U)/2$. Radial [null geodesics](../../../special-relativity.md#null-geodesic) have slopes $dT_K=\pm dX_K$, and the [curvature singularities](../../../general-relativity.md#curvature-singularity) have

$$
T_K^2-X_K^2=1.
$$

The upper branch is the future spacelike [Schwarzschild singularity](../../../general-relativity.md#schwarzschild-singularity); the lower branch is the [white hole](../../../general-relativity.md#white-hole) past singularity. The [Killing vector field](../../../general-relativity.md#killing-vector-field) extends as $\partial_t=(V\partial_V-U\partial_U)/(4M)$. It is future directed in the original exterior and past directed in the other exterior for the chosen global [time orientation](../../../general-relativity.md#time-orientation); inside, this stationary vector is spacelike. In the future interior, $r$ is a time coordinate decreasing toward the singularity. For example, a radial infaller of unit specific [Killing energy](../../../general-relativity.md#killing-energy) obeys $dr/d\tau=-\sqrt{2M/r}$ and reaches $r=0$ from the horizon in finite [proper time](../../../special-relativity.md#proper-time) $4M/3$. The curvature divergence and this geodesic endpoint show why the extension stops there.

For the global causal picture, compactify the null coordinates using $p=\arctan U$, $q=\arctan V$ and let $\mathcal T=2(p+q)/\pi$, $\mathcal X=2(q-p)/\pi$. The [conformal compactification](../../../geometry-and-topology.md#conformal-compactification) rescales the metric to remove the coordinate factors from the radial metric while preserving its [null directions](../../../special-relativity.md#null-directions). Since $UV=1$ gives $p+q=\pm\pi/2$ on the two singular branches, they become the horizontal lines $\mathcal T=\pm1$. The resulting [Penrose diagram](../../../general-relativity.md#penrose-diagram) displays the two exteriors, each with its own [past null infinity](../../../general-relativity.md#past-null-infinity), [future null infinity](../../../general-relativity.md#future-null-infinity) and spatial infinity, plus the future and past interiors. The singularities are spacelike boundaries; the horizons are interior null surfaces. Future [event horizons](../../../general-relativity.md#event-horizon) separate events that can escape to an exterior's future null infinity from events in the black-hole interior.

<a id="1/image-kruskal-and-compactified-diagrams-of-the-maximal-schwarzschild-extension-showing-both-exteriors-horizons-and-spacelike-singularities"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-62-extension.png)

**[Figure 1](#1/image-kruskal-and-compactified-diagrams-of-the-maximal-schwarzschild-extension-showing-both-exteriors-horizons-and-spacelike-singularities). Kruskal and compactified diagrams of the maximal Schwarzschild extension, showing both exteriors, horizons and spacelike singularities**.

The time-symmetric spatial slice has a bridge between the exteriors, but it is not a traversable passage. Future-directed causal curves have nondecreasing $U$ and $V$. Moving from the right exterior to the left would require $V$ to decrease from positive to negative; the reverse passage would require $U$ to decrease. Both are impossible. This proves the [non-traversability of the Schwarzschild bridge](../../../general-relativity.md#non-traversability-of-the-schwarzschild-bridge). **The complete eternal vacuum extension has two exteriors, a [black hole](../../../general-relativity.md#black-hole) and a [white hole](../../../general-relativity.md#white-hole); it has no causal route between its exteriors.** A [black hole](../../../general-relativity.md#black-hole) made by stellar collapse is a different global spacetime: its matter-filled past replaces the [white hole](../../../general-relativity.md#white-hole) region, and it normally has only one exterior. The vacuum extension constructed here should not be mistaken for the collapse history of a single star.

With [electric charge](../../../electromagnetism.md#electric-charge), spherical electrovacuum instead gives the [Reissner-Nordstrom metric](../../../general-relativity.md#reissner-nordstrom-spacetime), in an electromagnetic normalization absorbing the charge conversion constants:

$$
f(r)=1-\frac{2M}{r}+\frac{Q^2}{r^2},\qquad r_\pm=M\pm\sqrt{M^2-Q^2}.
$$

For $0<|Q|<M$, there are two simple horizons. Outside $r_+$ the metric is static; between $r_-$ and $r_+$, $f<0$ and $r$ is timelike. Inside $r_-$, $f>0$ again, so $r$ is spacelike and the $r=0$ singularity is timelike. The outer horizon is the [event horizon](../../../general-relativity.md#event-horizon); the inner horizon is a [Cauchy horizon](../../../general-relativity.md#cauchy-horizon). The same logarithmic tortoise-coordinate and exponential-null-coordinate method crosses each simple horizon locally, but one exponential scale does not regularize both simultaneously: their [surface gravities](../../../general-relativity.md#surface-gravity) have different magnitudes,

$$
|\kappa_\pm|=\frac{r_+-r_-}{2r_\pm^2}.
$$

Continuing the exact metric through successive inner horizons produces repeated blocks with further exteriors, and evolution beyond a [Cauchy horizon](../../../general-relativity.md#cauchy-horizon) is not uniquely fixed by data on the original [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface). The timelike singularity can be avoided by some trajectories in this ideal extension, unlike the unavoidable spacelike singularity of the future [Schwarzschild spacetime](../../../general-relativity.md#schwarzschild-spacetime) interior. However, the enormous inner-horizon blueshift makes this exact continuation unstable: perturbations can cause [mass inflation](../../../general-relativity.md#mass-inflation). This is an important qualification on the [global structure of a charged spherical black hole](../../../general-relativity.md#global-structure-of-a-charged-spherical-black-hole).

At $|Q|=M$ the two horizons coalesce, $f=(1-M/r)^2$ and [surface gravity](../../../general-relativity.md#surface-gravity) is zero. The horizon is a [degenerate Killing horizon](../../../general-relativity.md#degenerate-killing-horizon), the tortoise-coordinate divergence becomes a pole and the ordinary nondegenerate [Kruskal spacetime](../../../general-relativity.md#kruskal-spacetime) construction must be replaced. The exterior develops an infinitely long spatial throat and the formal [Hawking temperature](../../../general-relativity.md#hawking-temperature) vanishes. For $|Q|>M$, no real zero of $f$ remains: the electrovacuum solution has a [naked singularity](../../../general-relativity.md#naked-singularity), not a [black hole](../../../general-relativity.md#black-hole). Consequently arbitrarily allowing charge changes the causal structure, not just the horizon radius.

## 2

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use $\hbar=c=k_B=1$ and normalize the time-translation [Killing vector field](../../../general-relativity.md#killing-vector-field) at infinity. The simple outer zero and positivity on its exterior imply $b=V'(r_0)>0$. Near the horizon, write $x=r-r_0$; then $V=bx+O(x^2)$. The [Wick rotation](../../../perturbative-quantum-field-theory.md#wick-rotation) $t=-it_E$ gives the radial Euclidean metric

$$
ds_E^2=V\,dt_E^2+\frac{dr^2}{V}+r^2d\Omega^2.
$$

Define $\rho=2\sqrt{x/b}$, so $x=b\rho^2/4$. Its leading near-horizon form is

$$
ds_E^2=d\rho^2+\rho^2\left(\frac b2dt_E\right)^2+r_0^2d\Omega^2+O(\rho^2)d\rho^2+O(\rho^4)dt_E^2+O(\rho^2)d\Omega^2.
$$

Thus $bt_E/2$ is a polar angle. Smoothness at the origin requires period $2\pi$, rather than a cone or a multiple cover with a branched origin. The [Euclidean black-hole regularity condition](../../../general-relativity.md#euclidean-black-hole-regularity-condition) is

$$
\beta=\frac{4\pi}{b}.
$$

A thermal quantum state has imaginary-time period $\beta=1/T$. Since $V\to1$, this time coordinate is normalized to the clocks at infinity, and the [Hawking temperature](../../../general-relativity.md#hawking-temperature) is

$$
\boxed{T=\frac{V'(r_0)}{4\pi}.}
$$

A static clock at radius $r>r_0$ measures the redshifted local temperature $T/\sqrt{V(r)}$; that local quantity is not the temperature requested with the asymptotic normalization.

The static coordinates are singular on the horizon, so calculate its [surface gravity](../../../general-relativity.md#surface-gravity) in a regular ingoing chart. With $v=t+\int dr/V$, the metric and the same normalized [Killing vector field](../../../general-relativity.md#killing-vector-field) are

$$
ds^2=-V\,dv^2+2\,dv\,dr+r^2d\Omega^2,\qquad k=\partial_v.
$$

The inverse radial block has $g^{vr}=1$, $g^{rr}=V$, $g^{vv}=0$. Direct calculation gives

$$
\Gamma^v{}_{vv}=\frac{V'}2,\qquad\Gamma^r{}_{vv}=\frac{VV'}2.
$$

Since $k$ has constant coordinate components, its acceleration is

$$
k^a\nabla_a k^b=\frac{V'}2(\partial_v)^b+\frac{VV'}2(\partial_r)^b.
$$

On the future horizon, $V=0$ and $k$ is null, so the defining equation gives $\kappa=b/2$. In the outgoing chart regular on the past branch, the radial cross-term is $-2\,du\,dr$ and the same calculation gives $\kappa=-b/2$ for $k=\partial_u$. Hence the branch-independent physical statement is

$$
\boxed{|\kappa|=\frac{V'(r_0)}2=2\pi T.}
$$

This proves the [Euclidean temperature and signed horizon surface gravity](../../../general-relativity.md#euclidean-temperature-and-signed-horizon-surface-gravity) relation directly. Rescaling the [Killing vector field](../../../general-relativity.md#killing-vector-field) would rescale its [surface gravity](../../../general-relativity.md#surface-gravity); the condition at infinity fixes that otherwise arbitrary normalization.

## 3

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use [Planck units](../../../physics.md#planck-units) for the following formulas. The [black-hole area theorem](../../../general-relativity.md#hawking-s-area-theorem) is a classical statement with hypotheses. Assume the [Einstein field equations](../../../general-relativity.md#einstein-field-equations), the [null energy condition](../../../general-relativity.md#null-energy-condition) and appropriate global future regularity/predictability. For a clean version of the focusing sketch, take the future horizon generators to remain on a regular horizon and to be future complete in affine parameter. The usual [strong asymptotic predictability](../../../general-relativity.md#strong-asymptotic-predictability) formulation supplies the global causal control needed to exclude the same focusing pathology; an arbitrary spacetime with naked future breakdown is not covered by the theorem.

Let $\ell^a$ be an affinely parametrized generator of a smooth portion of the [event horizon](../../../general-relativity.md#event-horizon), and let $\theta=d\log dA/d\lambda$ be its [null expansion](../../../geodesic-congruence.md#null-expansion). The horizon is a null hypersurface, so its generators have zero [null twist](../../../geodesic-congruence.md#null-twist). In four dimensions the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) is

$$
\frac{d\theta}{d\lambda}=-\frac12\theta^2-\sigma_{ab}\sigma^{ab}-R_{ab}\ell^a\ell^b.
$$

The [Einstein field equations](../../../general-relativity.md#einstein-field-equations) give $R_{ab}\ell^a\ell^b=8\pi T_{ab}\ell^a\ell^b\ge0$, since the metric terms vanish when contracted with a null vector. The screen-space [null shear](../../../geodesic-congruence.md#null-shear) term is also nonnegative, so $\theta'\le-\theta^2/2$. If $\theta_0<0$ at $\lambda_0$, integrating this inequality while the congruence remains regular gives

$$
\theta(\lambda)\le\frac{\theta_0}{1+\tfrac12\theta_0(\lambda-\lambda_0)}.
$$

It focuses within affine distance at most $2/|\theta_0|$. The vanishing area element is a focal point to an earlier spacelike horizon cut. Past such a point the [null geodesic](../../../special-relativity.md#null-geodesic) can no longer generate an [achronal boundary](../../../general-relativity.md#achronal-boundary), but the [event horizon](../../../general-relativity.md#event-horizon) is precisely such a boundary. Future completeness and the global hypotheses exclude its escaping this contradiction by ending prematurely at a pathology. Therefore $\theta\ge0$ everywhere the smooth horizon description applies.

Integrate $d(dA)/d\lambda=\theta\,dA$ between ordered horizon cuts. Every continuing generator contributes a nondecreasing area element. New generators can enter at past endpoints or merger crease sets, adding area; generators cannot leave a regular future horizon through future endpoints under these hypotheses. Thus, including the total area of disconnected components,

$$
\boxed{A_{\rm later}\ge A_{\rm earlier}.}
$$

This is the [future-complete horizon focusing proof of the area theorem](../../../general-relativity.md#future-complete-horizon-focusing-proof-of-the-area-theorem). A smooth elementary congruence proof requires the stated regularity; the general theorem also treats the horizon's nonsmooth joining set rather than assuming mergers have a globally smooth horizon.

[Hawking radiation](../../../general-relativity.md#hawking-radiation) changes the situation because the quantum field state in a collapsing geometry is not a classical positive-energy fluid. For a large isolated [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime),

$$
T_H=\frac1{8\pi M},\qquad r_H\simeq2M,\qquad A\simeq16\pi M^2
$$

in natural units. Outgoing quantum modes at [future null infinity](../../../general-relativity.md#future-null-infinity) have a nearly thermal occupation, modified by [greybody factors](../../../general-relativity.md#greybody-factor); an accompanying negative [Killing energy](../../../general-relativity.md#killing-energy) flux near the horizon reduces the hole's mass. On timescales short compared with the evaporation time but long compared with $M$, its geometry is approximately [Schwarzschild spacetime](../../../general-relativity.md#schwarzschild-spacetime) with slowly decreasing $M(t)$. It is not an exactly stationary vacuum solution with a parameter changed by hand: the radiation's [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) sources the time dependence through the [semiclassical Einstein equation](../../../quantum-theory.md#semiclassical-einstein-equation). The distant luminosity is carried by the outgoing radiation, while the horizon-area decrease accompanies the inward negative-energy contribution.

As the [black hole](../../../general-relativity.md#black-hole) loses mass, its horizon scale and [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy) shrink, its temperature rises and its luminosity increases. This is the [negative heat capacity of a Schwarzschild black hole](../../../general-relativity.md#negative-heat-capacity-of-a-schwarzschild-black-hole). Large astrophysical holes evaporate extremely slowly in isolation; small holes evaporate more rapidly, and increasingly massive particle species become accessible as the temperature rises. An incoming radiation bath or accretion can instead offset the loss, so the pure evaporation law assumes negligible incoming energy. A formal complete evaporation also raises the [black hole information paradox](../../../general-relativity.md#black-hole-information-paradox); the low-curvature calculation alone does not determine how information or the final state is resolved.

For an elementary luminosity estimate, treat the horizon as emitting photon [blackbody radiation](../../../statistical-physics.md#black-body-radiation). In natural units the [Stefan–Boltzmann law](../../../thermodynamics.md#stefan-boltzmann-law) has $\sigma=\pi^2/60$, giving

$$
P=A\sigma T_H^4=\frac1{15360\pi M^2}.
$$

The horizon area used here is an estimate of emitting area, not the exact frequency-dependent absorption cross-section. More generally write $P=\alpha/M^2$, where $\alpha>0$ includes the [greybody factors](../../../general-relativity.md#greybody-factor) and the active particle species. For constant effective $\alpha$, energy balance and direct integration give

$$
\frac{dM}{dt}=-\frac{\alpha}{M^2},\qquad \frac{d(M^3)}{dt}=-3\alpha,
\qquad\boxed{M(t)=\bigl(M_0^3-3\alpha t\bigr)^{1/3}.}
$$

Here $t$ is time measured at infinity. The formal evaporation timescale is $M_0^3/(3\alpha)$; with the photon blackbody estimate it is $5120\pi M_0^3$. Restoring constants gives

$$
\boxed{t_{\rm evap}\simeq\frac{5120\pi G^2M_0^3}{\hbar c^4}}
$$

for that specified estimate. If particle thresholds make $\alpha$ mass dependent, the precise leading law is instead $t=\int_{M(t)}^{M_0}m^2\,dm/\alpha(m)$. The robust result is the inverse-square mass-loss rate for a fixed species regime and the cubic mass scaling of its lifetime. This is the [semiclassical cubic mass law for Schwarzschild evaporation](../../../general-relativity.md#semiclassical-cubic-mass-law-for-schwarzschild-evaporation). Extrapolating its zero to a definite end state is unjustified once $M$ approaches the [Planck mass](../../../physics.md#planck-mass) and curvature requires [quantum gravity](../../../quantum-theory.md#quantum-gravity).

There is **no contradiction with the classical area theorem**: the renormalized quantum [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) can violate the [null energy condition](../../../general-relativity.md#null-energy-condition) used in the focusing inequality. In the evaporation regime,

$$
\frac{dA}{dt}\simeq32\pi M\frac{dM}{dt}=-\frac{32\pi\alpha}{M}<0,
$$

which is permitted when that hypothesis fails. The thermodynamic replacement is the [generalized second law](../../../general-relativity.md#generalized-second-law), concerning $S_{\rm outside}+A/(4G\hbar)$ rather than horizon area alone. Outside radiation can carry entropy while the hole's [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy) decreases.

## 4

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use [geometrized units](../../../general-relativity.md#geometrized-units) $G=c=1$ until converting the clock readings. By the [Birkhoff theorem](../../../general-relativity.md#birkhoff-s-theorem), the spherical vacuum exterior is a portion of the [Schwarzschild spacetime](../../../general-relativity.md#schwarzschild-spacetime) with fixed mass $M$:

$$
\boxed{ds^2_{\rm out}=-\left(1-\frac{2M}{r}\right)dt^2+\left(1-\frac{2M}{r}\right)^{-1}dr^2+r^2d\Omega^2,\qquad r>R(\tau).}
$$

The exterior is not flat and is not radiating merely because the surface moves. When the surface crosses $r=2M$, this exterior must be represented in regular [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates), rather than treating the Schwarzschild-coordinate divergence as a physical barrier.

The [Oppenheimer-Snyder model](../../../general-relativity.md#oppenheimer-snyder-model) has a homogeneous [pressureless matter](../../../cosmology.md#pressureless-matter) interior. Since its initial expansion vanishes but its [density](../../../fluid-mechanics.md#density) is positive, the [Friedmann equation](../../../cosmology.md#friedmann-equations) requires positive spatial curvature. Choose a comoving radial angle $\chi$ and the boundary's [proper time](../../../special-relativity.md#proper-time) $\tau$, with the stopwatch set to zero at release. The interior [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) and [density](../../../fluid-mechanics.md#density) are

$$
\boxed{ds^2_{\rm in}=-d\tau^2+a(\tau)^2\bigl(d\chi^2+\sin^2\chi\,d\Omega^2\bigr),\qquad0\le\chi\le\chi_0,}
\qquad \rho(\tau)=\rho_0\left(\frac{a_{\max}}a\right)^3.
$$

The [density](../../../fluid-mechanics.md#density) law follows from the [dust stress-energy tensor](../../../general-relativity.md#dust-stress-energy-tensor) and its covariant conservation. The [Friedmann equation](../../../cosmology.md#friedmann-equations) and the initial rest condition give

$$
\dot a^2+1=\frac{8\pi}3\rho a^2=\frac{a_{\max}}a,\qquad \frac{8\pi}3\rho_0a_{\max}^2=1.
$$

Its contracting branch has the parameterization

$$
a=\frac{a_{\max}}2(1+\cos\eta),\qquad
\tau=\frac{a_{\max}}2(\eta+\sin\eta),\qquad0\le\eta<\pi.
$$

Indeed $d\tau/d\eta=a$ and $\dot a=-\sin\eta/(1+\cos\eta)$ satisfy the displayed equation; $\eta=0$ is the turning point and $\eta=\pi$ is the final [curvature singularity](../../../general-relativity.md#curvature-singularity).

For [homogeneous dust-ball matching](../../../general-relativity.md#homogeneous-dust-ball-matching), the boundary has [areal radius](../../../general-relativity.md#areal-radius) $R=a\sin\chi_0$. Matching its mass to the exterior gives

$$
M=\frac{4\pi}3\rho R^3=\frac{a_{\max}}2\sin^3\chi_0,\qquad
\sin^2\chi_0=\frac{2M}{R_0},\qquad
\boxed{a_{\max}=\sqrt{\frac{R_0^3}{2M}}.}
$$

This $M$ is the gravitational mass parameter, not the integral of rest [density](../../../fluid-mechanics.md#density) over the curved proper-volume element. The matching can also be checked directly. The outward angular [extrinsic curvature](../../../differential-geometry.md#extrinsic-curvature) inside is $K_{\theta\theta}=R\cos\chi_0$; outside it is $R\sqrt{1-2M/R+\dot R^2}$. The boundary motion has

$$
\dot R^2=\frac{2M}{R}-\frac{2M}{R_0},\qquad E=\sqrt{1-\frac{2M}{R_0}}=\cos\chi_0,
$$

so these curvatures agree. The induced metric is $-d\tau^2+R^2d\Omega^2$ on both sides and $K_{\tau\tau}=0$ because the pressure-free boundary is geodesic. No artificial surface stress layer is required.

The observer moving with this boundary meets the [event horizon](../../../general-relativity.md#event-horizon) when $R=2M$. From $R=R_0(1+\cos\eta)/2$, the [proper-time horizon crossing in homogeneous dust collapse](../../../general-relativity.md#proper-time-horizon-crossing-in-homogeneous-dust-collapse) occurs at

$$
\eta_H=2\arccos\sqrt{\frac{2M}{R_0}}=\pi-2\chi_0,
\qquad
\tau_H=\frac{a_{\max}}2(\eta_H+\sin\eta_H).
$$

The singularity is reached at $\tau_s=\pi a_{\max}/2$, so the remaining clock time is

$$
\Delta\tau=\tau_s-\tau_H=\frac{a_{\max}}2(\pi-\eta_H-\sin\eta_H).
$$

These are finite [proper times](../../../special-relativity.md#proper-time), even though the external static time diverges at horizon crossing.

Convert the supplied rounded units consistently: $M=10^{38}$ [Planck masses](../../../physics.md#planck-mass) and $R_0=6.25\times10^{39}$ [Planck lengths](../../../physics.md#planck-length). Thus $2M/R_0=0.032$, $\chi_0\simeq0.17985$, and $a_{\max}\simeq3.4939\times10^{40}$ in [Planck units](../../../physics.md#planck-units). Multiplying geometric times by $5\times10^{-44}$ seconds gives

$$
\boxed{\tau_H\simeq2.737\times10^{-3}\ {\rm s},\qquad
\tau_s\simeq2.744\times10^{-3}\ {\rm s},\qquad
\Delta\tau\simeq6.73\times10^{-6}\ {\rm s}.}
$$

At the accuracy justified by the rounded constants, these are **about three milliseconds to horizon crossing and about seven microseconds more to the singularity**. For $R_0\gg2M$, expanding $\eta_H=\pi-2\chi_0$ gives $\Delta\tau\simeq(2/3)a_{\max}\chi_0^3\simeq4M/3$, independently confirming the microsecond scale. The exact expression above retains the finite release-radius correction.

Strictly, this boundary clock reading is when the observer crosses the horizon, not when the horizon first exists anywhere. The [event horizon inside an Oppenheimer-Snyder cloud](../../../general-relativity.md#event-horizon-inside-an-oppenheimer-snyder-cloud) is an outgoing radial null ray. Since $d\tau=a\,d\eta$, the interior metric is conformal to $-d\eta^2+d\chi^2+\sin^2\chi\,d\Omega^2$, and that ray has $d\chi/d\eta=1$. Tracing it back from $(\eta_H,\chi_0)$ gives

$$
\chi_{\mathcal H}=\eta-\eta_H+\chi_0,\qquad \eta_{\rm birth}=\eta_H-\chi_0=\pi-3\chi_0.
$$

For this cloud it starts at the centre after release, at comoving time $\tau_{\rm birth}\simeq2.722\times10^{-3}$ seconds. This answers the literal global-formation interpretation as well; it is not an event on the outer observer's worldline. The distinction matters because an [event horizon](../../../general-relativity.md#event-horizon) is defined by the entire future causal escape problem, not by a locally detectable signal of formation.

For the observer at infinity, use the boundary's conserved [Killing energy](../../../general-relativity.md#killing-energy) $E$ in the exterior:

$$
\frac{dt}{d\tau}=\frac{E}{1-2M/R}.
$$

As $\tau\uparrow\tau_H$, $\dot R\to-E$ and $R-2M\simeq E(\tau_H-\tau)$. Consequently

$$
t=-2M\log\left(\frac{\tau_H-\tau}{\tau_*}\right)+O(1)\longrightarrow+\infty,
$$

where $\tau_*>0$ fixes a harmless dimensionless logarithm. For actual outgoing light signals the relevant retarded time is $u=t-r_*(R)$. Since $r_*\simeq2M\log(R-2M)+O(1)$,

$$
u=-4M\log\left(\frac{\tau_H-\tau}{\tau_*}\right)+O(1)\longrightarrow+\infty.
$$

Therefore **she never receives a signal showing the surface cross the horizon at any finite asymptotic time**. Radiation emitted ever closer to crossing arrives ever later and is increasingly redshifted and diluted; photons emitted at or inside the [event horizon](../../../general-relativity.md#event-horizon) cannot reach her. The formal crossing time at infinity is infinite, not the finite boundary stopwatch reading. Nor can the earlier global birth of the horizon be observed directly as a local flash from its central birth event.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
