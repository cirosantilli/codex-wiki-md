# Paper 63

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper63.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper63.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use [metric signature](../../../topology.md#metric-signature) $(+---)$ throughout this solution. [Stress-energy conservation](../../../general-relativity.md#stress-energy-conservation) for the [perfect fluid](../../../general-relativity.md#perfect-fluid) is $\nabla_bT^{ab}=0$. Expanding it and using [metric compatibility](../../../fiber-bundle.md#metric-compatibility) gives

$$
0=U^a\nabla_b[(\rho+p)U^b]+(\rho+p)U^b\nabla_bU^a-\nabla^ap.
$$

The normalization of the [four-velocity](../../../special-relativity.md#four-velocity) implies $U_aU^b\nabla_bU^a=0$. Contracting with $U_a$ therefore gives the [relativistic perfect-fluid energy equation](../../../general-relativity.md#relativistic-perfect-fluid-energy-equation),

$$
U^b\nabla_b\rho+(\rho+p)\nabla_bU^b=0,
$$

while subtracting the component parallel to $U$ gives the [relativistic Euler equation](../../../general-relativity.md#relativistic-euler-equation),

$$
\boxed{(\rho+p)U^b\nabla_bU_a=\nabla_ap-U_aU^b\nabla_bp.}
$$

Equivalently, apply the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) $\delta_a{}^c-U_aU^c$ to the conservation equation. This form makes clear that a [pressure](../../../thermodynamics.md#pressure) gradient orthogonal to the [four-velocity](../../../special-relativity.md#four-velocity) supplies the fluid's [four-acceleration](../../../special-relativity.md#four-acceleration).

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $N=\sqrt{K^aK_a}>0$ on the fluid region and choose the [Killing vector field](../../../general-relativity.md#killing-vector-field) $K$ to be future-directed. The normalized [four-velocity](../../../special-relativity.md#four-velocity) is

$$
\boxed{U^a=\frac{K^a}{N}.}
$$

The [Killing equation](../../../general-relativity.md#killing-equation) implies both $K^b\nabla_bN=0$ and

$$
K^b\nabla_bK_a=-K^b\nabla_aK_b=-\frac12\nabla_a(K^bK_b).
$$

Consequently its [Killing-flow four-acceleration](../../../general-relativity.md#killing-flow-four-acceleration) is

$$
U^b\nabla_bU_a=\frac1{N^2}K^b\nabla_bK_a=-\nabla_a\log N.
$$

For a scalar, the [Lie derivative](../../../differential-form.md#lie-derivative-of-a-differential-form) is $\mathcal L_Kp=K^b\nabla_bp$. Thus the assumed stationarity of the [pressure](../../../thermodynamics.md#pressure) gives $U^b\nabla_bp=0$. These are the ingredients needed for [hydrostatic equilibrium along a Killing vector](../../../general-relativity.md#hydrostatic-equilibrium-along-a-killing-vector); hypersurface orthogonality of $K$ is not needed.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Substitute the [Killing-flow four-acceleration](../../../general-relativity.md#killing-flow-four-acceleration) and stationary [pressure](../../../thermodynamics.md#pressure) into the [relativistic Euler equation](../../../general-relativity.md#relativistic-euler-equation). It gives

$$
\boxed{\nabla_ap=-(\rho+p)\nabla_a\log N,
\qquad N=\sqrt{K^cK_c}.}
$$

For the [equation of state](../../../thermodynamics.md#equation-of-state) of [blackbody radiation](../../../statistical-physics.md#black-body-radiation), $p=\rho/3$, this becomes $d\rho=-4\rho\,d\log N$. The [barotropic hydrostatic first integral](../../../general-relativity.md#barotropic-hydrostatic-first-integral) therefore gives, on each connected nonvacuum fluid region,

$$
\boxed{\rho N^4=C>0,\qquad \rho=C(K^cK_c)^{-2}.}
$$

This is the [stationary radiation density](../../../general-relativity.md#stationary-radiation-density) law. Combining it with the [Stefan–Boltzmann law](../../../thermodynamics.md#stefan-boltzmann-law) $\rho\propto T^4$ also gives the [Tolman–Ehrenfest relation](../../../thermodynamics.md#tolman-ehrenfest-relation) $TN=\mathrm{constant}$.

At a regular finite [free surface](../../../fluid-mechanics.md#free-surface), a smooth [Killing vector field](../../../general-relativity.md#killing-vector-field) has finite norm. Hence $C/N^4$ cannot approach zero there. More globally, its norm has a finite upper bound on a [compact](../../../topology.md#compact-space) regular fluid closure, which bounds the density away from zero whenever $C>0$. If the timelike norm instead tends to zero, the density diverges. Thus a [radiation fluid has no regular free surface](../../../general-relativity.md#radiation-fluid-has-no-regular-free-surface): a finite radiation-filled cavity needs a material wall supporting nonzero [pressure](../../../thermodynamics.md#pressure), rather than an unsupported radiation-vacuum interface.

## 2

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Take $z$ positive outward and define the separation as upper minus lower position. The [Newtonian potential of a point mass](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass) gives the acceleration $a(z)=-\partial_z\phi=-GM/z^2$. Expanding its difference across a separation $\zeta\ll z$ gives the [tidal force](../../../classical-mechanics.md#tidal-force) equation

$$
\ddot\zeta=a(z+\zeta)-a(z)=a'(z)\zeta+O(\zeta^2/z^2)
\simeq\boxed{\frac{2GM}{z^3}\zeta}.
$$

The upper particle falls slightly less rapidly, so the separation increases. If the upper particle carries the [electric charge](../../../electromagnetism.md#electric-charge) and the [electric field](../../../electromagnetism.md#electric-field) points outward, the extra relative acceleration is $qE/m$. Reversing the field or placing the charge on the lower particle changes its sign. Write this signed acceleration as $a_e$ and put $k=2GM/z^3$. With initial relative velocity zero and nearly constant $k$ and $a_e$, the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) has solution

$$
\zeta(t)=\zeta_0\cosh(\sqrt{k}\,t)
+\frac{a_e}{k}\bigl[\cosh(\sqrt{k}\,t)-1\bigr].
$$

For $kt^2\ll1$, the leading changes due to the [tidal force](../../../classical-mechanics.md#tidal-force) and [electric field](../../../electromagnetism.md#electric-field) are respectively

$$
\boxed{\Delta\zeta_g\simeq\frac{GM}{z^3}\zeta_0t^2,
\qquad \Delta\zeta_e\simeq\frac{qE}{2m}t^2}
$$

with the stated sign convention. Thus, for a nonzero fixed electric acceleration,

$$
\frac{|\Delta\zeta_g|}{|\Delta\zeta_e|}
\simeq\frac{2mGM|\zeta_0|}{|qE|z^3}
=\frac{2mg}{|qE|}\frac{|\zeta_0|}{z},
\qquad g=\frac{GM}{z^2}.
$$

A laboratory of size $L$ has $|\zeta_0|\leq L$, so this ratio tends to zero as $L\to0$. This is [local tidal acceleration scaling](../../../general-relativity.md#local-tidal-acceleration-scaling): gravitational relative acceleration is proportional to separation, whereas the electric difference persists even at coincident positions.

The duration also matters. At fixed time, $\Delta\zeta_g\to0$ in absolute size, but $\Delta\zeta_g/\zeta_0\simeq(GM/z^3)t^2$ need not tend to zero. To keep the electrically displaced particles in the shrinking laboratory, take $|a_e|t^2\lesssim L$; then $|\Delta\zeta_g|/L\lesssim GM L/(z^3|a_e|)\to0$. Alternatively a stationary terrestrial laboratory has a free-fall time of order $\sqrt{L/g}$, giving $|\Delta\zeta_g|/|\zeta_0|=O(L/z)$. Both make precise the small spacetime-region limit. An extended, long-running experiment can still measure arbitrarily small [tidal forces](../../../classical-mechanics.md#tidal-force).

The [weak equivalence principle](../../../general-relativity.md#weak-equivalence-principle) says that freely falling [test particles](../../../classical-mechanics.md#test-particle) with the same initial data have composition-independent motion. In particular, a freely falling frame removes the common gravitational acceleration of both particles. The electric accelerations depend on charge and cannot be removed for charged and uncharged particles simultaneously by the same change of frame.

The [Einstein equivalence principle](../../../general-relativity.md#einstein-equivalence-principle) extends the freely falling laboratory statement to all local nongravitational experiments: their outcomes obey [special relativity](../../../special-relativity.md), with local Lorentz invariance and local position invariance. The [strong equivalence principle](../../../general-relativity.md#strong-equivalence-principle) also includes local gravitational experiments and bodies with significant gravitational binding energy. It asserts universality of their free fall and independence of local experimental outcomes from the laboratory's location and velocity. The two-particle experiment illustrates the local distinction between gravity and a nongravitational force; by itself it does not establish this stronger claim about self-gravitating bodies.

In a metric theory, the common freely falling trajectories are [timelike geodesics](../../../general-relativity.md#timelike-geodesic) of a [Lorentzian metric](../../../general-relativity.md#lorentzian-metric). [Normal coordinates](../../../general-relativity.md#normal-coordinates) make $g_{ab}=\eta_{ab}$ and the [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) zero at one point. [Fermi normal coordinates](../../../general-relativity.md#fermi-coordinates) do the same along a reference [timelike geodesic](../../../general-relativity.md#timelike-geodesic). The residual effects are controlled by the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) through [geodesic deviation](../../../general-relativity.md#geodesic-deviation), and enter the local metric at quadratic order in distance. Curvature is a physical tidal field, so no coordinate choice removes it over a finite region.

A relativistic theory should consequently couple matter universally to the [metric tensor](../../../general-relativity.md#metric-tensor), recover nongravitational laws in local inertial frames and recover the Newtonian limit. [General relativity](../../../general-relativity.md) implements this with the [Einstein field equations](../../../general-relativity.md#einstein-field-equations); the [contracted Bianchi identity](../../../general-relativity.md#contracted-bianchi-identity) is consistent with [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation). The [Equivalence principle](../../../general-relativity.md#equivalence-principle) motivates this geometric description but does not alone uniquely determine the field equations. Extra gravitational fields may satisfy the [Einstein equivalence principle](../../../general-relativity.md#einstein-equivalence-principle) for ordinary matter while failing the [strong equivalence principle](../../../general-relativity.md#strong-equivalence-principle) because local gravitational measurements or self-gravitating trajectories depend on those fields.

## 3

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $I^{ij}(t)=\int T^{00}(t,\mathbf x)x^ix^j\,d^3x$, using spatial indices $i,j$. [Stress-energy conservation](../../../general-relativity.md#stress-energy-conservation), symmetry of the [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) and [integration by parts](../../../calculus.md#integration-by-parts) give

$$
\dot I^{ij}=-\int\partial_kT^{0k}x^ix^j\,d^3x
=\int(T^{0i}x^j+T^{0j}x^i)\,d^3x,
$$

and a second derivative gives

$$
\ddot I^{ij}=-\int(\partial_kT^{ik}x^j+\partial_kT^{jk}x^i)\,d^3x
=\int(T^{ij}+T^{ji})\,d^3x.
$$

All boundary terms vanish by [compact support](../../../function.md#compact-support). This proves the [stress-energy quadrupole identity](../../../general-relativity.md#stress-energy-quadrupole-identity),

$$
\boxed{\int T^{ij}\,d^3x=\frac12\ddot I^{ij}.}
$$

The support is understood to remain bounded over the time interval used for differentiating these integrals.

For the radiation calculation set $c=1$, write $g_{ab}=\eta_{ab}+h_{ab}$ and use the [trace-reversed metric perturbation](../../../general-relativity.md#trace-reversed-metric-perturbation) $\bar h_{ab}=h_{ab}-\eta_{ab}h/2$ in [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity). With the curvature and field-equation signs in this paper, the linear equation is

$$
\Box\bar h_{ab}=-16\pi GT_{ab},\qquad \Box=\partial_t^2-\nabla^2.
$$

The retarded solution with no incoming radiation is consequently

$$
\bar h_{ab}(t,\mathbf x)=-4G\int
\frac{T_{ab}(t-|\mathbf x-\mathbf x'|,\mathbf x')}
{|\mathbf x-\mathbf x'|}\,d^3x'.
$$

Let $r=|\mathbf x|$ be the distance from the source's [centre of mass](../../../classical-mechanics.md#center-of-mass), and let $d$ be its size. In the [radiation zone](../../../electromagnetism.md#radiation-zone), $r\gg d$. The leading [multipole expansion](../../../electromagnetism.md#electric-multipole-expansion) additionally assumes slow internal motion, or $d$ small compared with the radiation wavelength. These assumptions allow $|\mathbf x-\mathbf x'|\simeq r$ in the denominator and the common retarded time $u=t-r$ at leading quadrupole order. Thus

$$
\bar h_{ij}\simeq-\frac{4G}{r}\int T_{ij}(u,\mathbf x')\,d^3x'
=-\frac{2G}{r}\ddot I_{ij}(u).
$$

Define the trace-free [mass quadrupole moment](../../../general-relativity.md#mass-quadrupole-moment) by

$$
Q^{ij}=I^{ij}-\frac13\delta^{ij}I^{kk}
=\int T^{00}\left(x^ix^j-\frac13\delta^{ij}|\mathbf x|^2\right)d^3x.
$$

To make the requested normalization explicit, write the trace-free spatial metric coefficient as $h_{ij}^{\mathrm{TF}}=-2E_{ij}$. Trace reversal only adds a spatial trace, so the preceding equations give the [far-zone quadrupole strain](../../../general-relativity.md#far-zone-quadrupole-strain) coefficient

$$
\boxed{E^{ij}(t,\mathbf x)=\frac{G}{r}\ddot Q^{ij}(t-r).}
$$

The supplied scan does not contain the referenced perturbation handout. The definition above fixes the normalization of $E$ directly. If $E$ denotes the physical [transverse-traceless tensor](../../../general-relativity.md#transverse-traceless-tensor) in that handout, the right-hand side is also to be transversely projected for the observation direction. Trace-free alone does not imply transverse. With $\mathbf n=\mathbf x/r$, put

$$
P_{ij}=\delta_{ij}-n_in_j,\qquad
\Lambda_{ij,kl}=P_{i(k}P_{l)j}-\frac12P_{ij}P_{kl}.
$$

The [transverse-traceless projector](../../../general-relativity.md#transverse-traceless-projector) gives $E^{\mathrm{TT}}_{ij}=\Lambda_{ij,kl}E_{kl}$ and the physical spatial strain is $H^{\mathrm{TT}}_{ij}=2E^{\mathrm{TT}}_{ij}$. This also states the result without relying on omitted handout notation. The retarded construction and direction-dependent transverse projection are described in [Carroll's general relativity lectures](https://ned.ipac.caltech.edu/level5/March01/Carroll3/Carroll6.html), with the appropriate changes of metric-sign convention.

For the equal-mass [binary star](../../../stellar-astrophysics.md#binary-star), its [centre of mass](../../../classical-mechanics.md#center-of-mass) is at the origin and the separation is $2R$. The gravitational force on either star is $Gm^2/(2R)^2$, while its centripetal force is $mR\omega^2$. Hence

$$
\boxed{\omega^2=\frac{Gm}{4R^3},\qquad \theta(t)=\omega t+\theta_0.}
$$

At leading Newtonian order, $T^{00}$ is the sum of the two point-mass densities. Its moments are

$$
I^{ij}=2mR^2
\begin{pmatrix}
\cos^2\theta&\sin\theta\cos\theta&0\\
\sin\theta\cos\theta&\sin^2\theta&0\\
0&0&0
\end{pmatrix},
\qquad I^{kk}=2mR^2,
$$

so the trace-free [mass quadrupole moment](../../../general-relativity.md#mass-quadrupole-moment) is

$$
Q^{ij}=mR^2
\begin{pmatrix}
\cos2\theta+\frac13&\sin2\theta&0\\
\sin2\theta&\frac13-\cos2\theta&0\\
0&0&-\frac23
\end{pmatrix}.
$$

The Newtonian bound system is treated in the usual leading weak-field quadrupole approximation; an exactly conserved effective source also includes the interaction stresses. Accelerated point-mass dust alone would not satisfy the conservation hypothesis.

Differentiating twice and evaluating at $u=t-r$ gives

$$
\boxed{E^{ij}=-\frac{4GmR^2\omega^2}{r}
\begin{pmatrix}
\cos2\theta(u)&\sin2\theta(u)&0\\
\sin2\theta(u)&-\cos2\theta(u)&0\\
0&0&0
\end{pmatrix}.}
$$

For an observer on the $z$ axis this is already transverse and traceless. Its alternating [plus polarization](../../../general-relativity.md#plus-polarization) and [cross polarization](../../../general-relativity.md#cross-polarization) have a phase difference of $\pi/2$, giving circularly polarized [gravitational radiation](../../../general-relativity.md#gravitational-wave) at twice the orbital frequency. The amplitude decays as $1/r$, as expected for outgoing radiation in three spatial dimensions.

More generally take the line of sight in the $xz$ plane at inclination $\iota$ to the orbital angular-momentum axis. In the transverse basis $\mathbf e_\theta=(\cos\iota,0,-\sin\iota)$, $\mathbf e_\phi=(0,1,0)$, define $A=4GmR^2\omega^2/r$. Projection gives the physical [gravitational wave polarizations](../../../general-relativity.md#gravitational-wave-polarization)

$$
h_+=-A(1+\cos^2\iota)\cos2\theta(u),
\qquad h_\times=-2A\cos\iota\sin2\theta(u).
$$

Thus a generic view is elliptically polarized, the face-on view is circularly polarized and the edge-on view is linearly polarized. This is [circular-binary quadrupole radiation](../../../general-relativity.md#circular-binary-quadrupole-radiation); an overall sign or transverse-axis rotation only changes the polarization convention.

## 4

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For the full unit-radius [two-dimensional de Sitter spacetime](../../../general-relativity.md#two-dimensional-de-sitter-spacetime), the coordinate ranges are

$$
\boxed{t\in\mathbb R,\qquad \chi\in\mathbb R/(2\pi\mathbb Z).}
$$

One can use $0\leq\chi<2\pi$ with endpoints identified. If the identification is omitted, the same line element describes the universal covering spacetime instead. The periodicity follows from the [hyperboloid](../../../differential-geometry.md#hyperboloid) embedding

$$
X^0=\sinh t,\qquad X^1=\cosh t\cos\chi,\qquad X^2=\cosh t\sin\chi,
\qquad (X^0)^2-(X^1)^2-(X^2)^2=-1.
$$

The induced ambient [Minkowski metric](../../../special-relativity.md#minkowski-metric) is precisely the given [Lorentzian metric](../../../general-relativity.md#lorentzian-metric).

Using an [affine parameter](../../../riemannian-geometry.md#affine-parameter) $s$, the [geodesic Lagrangian](../../../riemannian-geometry.md#geodesic-lagrangian) is $\tfrac12(\dot t^2-\cosh^2t\,\dot\chi^2)$. The nonzero [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) are

$$
\Gamma^t{}_{\chi\chi}=\sinh t\cosh t,
\qquad \Gamma^\chi{}_{t\chi}=\Gamma^\chi{}_{\chi t}=\tanh t.
$$

Thus the [geodesic equations](../../../riemannian-geometry.md#geodesic-equation) and their [first integrals](../../../differential-equation.md#first-integral) are

$$
\boxed{\ddot t+\sinh t\cosh t\,\dot\chi^2=0,
\qquad \ddot\chi+2\tanh t\,\dot t\dot\chi=0,}
$$



$$
J=\cosh^2t\,\dot\chi=\mathrm{constant},
\qquad \dot t^2-\frac{J^2}{\cosh^2t}=\varepsilon,
\qquad \varepsilon\in\{1,0,-1\}.
$$

Here $\varepsilon=1$ for unit-speed [timelike geodesics](../../../general-relativity.md#timelike-geodesic), $0$ for [null geodesics](../../../special-relativity.md#null-geodesic) and $-1$ for unit-speed [spacelike geodesics](../../../riemannian-geometry.md#spacelike-geodesic). The conserved $J$ is the [geodesic conserved quantity from a Killing vector](../../../general-relativity.md#geodesic-conserved-quantity-from-a-killing-vector) for the angular symmetry.

All [geodesics of two-dimensional de Sitter spacetime](../../../general-relativity.md#geodesics-of-two-dimensional-de-sitter-spacetime) can be written especially simply in the embedding. If $P$ is the initial point and $V$ the initial tangent, with $P^2=-1$, $P\cdot V=0$, $V^2=\varepsilon$, the geodesic has normal ambient acceleration $X''=\varepsilon X$. Therefore

$$
X(s)=
\begin{cases}
P\cosh s+V\sinh s,&\varepsilon=1,\\
P+sV,&\varepsilon=0,\\
P\cos s+V\sin s,&\varepsilon=-1.
\end{cases}
$$

These curves stay in the two-plane spanned by $P$ and $V$, preserve both constraints and have no tangential acceleration. They consequently solve the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) and exhaust all initial directions.

An [isometry](../../../riemannian-geometry.md#isometry) can move the chosen point to $P=(0,1,0)$, namely $(t,\chi)=(0,0)$. For future-directed [timelike geodesics](../../../general-relativity.md#timelike-geodesic) take $V=(\cosh\alpha,0,\sinh\alpha)$, obtaining

$$
\sinh t=\cosh\alpha\sinh s,
\qquad \tan\chi=\sinh\alpha\tanh s.
$$

The continuous angular branch has $|\chi|<\pi/2$, and every real $\alpha$ gives a distinct timelike direction. The two [null geodesics](../../../special-relativity.md#null-geodesic) have $V=(1,0,\pm1)$ and

$$
\sinh t=s,\qquad \tan\chi=\pm s.
$$

For [spacelike geodesics](../../../riemannian-geometry.md#spacelike-geodesic) take $V=(\sinh\alpha,0,\cosh\alpha)$, giving

$$
\sinh t=\sinh\alpha\sin s,
\quad \cosh t\cos\chi=\cos s,
\quad \cosh t\sin\chi=\cosh\alpha\sin s.
$$

They are closed with period $2\pi$ in affine arclength and $|t|\leq|\alpha|$. In particular, $\alpha=0$ is the equatorial geodesic $t=0$. These three families, with reversals of parametrization allowed, are the requested complete set through the chosen point.

The [conformal time](../../../cosmology.md#conformal-time) substitution gives

$$
T=2\arctan(e^t)-\frac\pi2,
\qquad \sin T=\tanh t,
\qquad \cos T=\operatorname{sech}t,
\qquad \frac{dT}{dt}=\operatorname{sech}t.
$$

Hence

$$
\boxed{ds^2=\sec^2T(dT^2-d\chi^2),
\qquad -\frac\pi2<T<\frac\pi2,\quad\chi\sim\chi+2\pi.}
$$

Multiplying by $\cos^2T$ gives the regular [conformal cylinder of two-dimensional de Sitter spacetime](../../../general-relativity.md#conformal-cylinder-of-two-dimensional-de-sitter-spacetime). Adding $T=\pm\pi/2$ completes the [conformal compactification](../../../geometry-and-topology.md#conformal-compactification); both boundary circles are spacelike. [Null geodesics](../../../special-relativity.md#null-geodesic) are straight lines $\chi=\pm T$ through the origin. The other families have the useful diagram equations

$$
\chi(T)=\arcsin(\tanh\alpha\sin T)\quad\text{for timelike geodesics},
\qquad T(\chi)=\arcsin(\tanh\alpha\sin\chi)\quad\text{for spacelike geodesics}.
$$

The image sketches representative directions from each family; the formulas allow all intermediate directions.

<a id="4/image-geodesics-through-one-point-and-observer-horizons-on-the-two-dimensional-de-sitter-conformal-cylinder"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-63-de-sitter-geodesics.png)

**[Figure 1](#4/image-geodesics-through-one-point-and-observer-horizons-on-the-two-dimensional-de-sitter-conformal-cylinder). Geodesics through one point and observer horizons on the two-dimensional de Sitter conformal cylinder**.

For the complete observer $\chi=0$, let $d(\chi,0)\in[0,\pi]$ be the shortest angular distance on the circle. Since light travels one unit of angular distance per unit [conformal time](../../../cosmology.md#conformal-time), an event at $(T,\chi)$ can signal to the observer at some finite future time precisely when

$$
\boxed{d(\chi,0)<\frac\pi2-T.}
$$

Equality defines its future [observer event horizon](../../../general-relativity.md#observer-event-horizon). Likewise an event can receive a signal emitted by the observer precisely when

$$
\boxed{d(\chi,0)<T+\frac\pi2,}
$$

and equality defines the past horizon. In the lift $-\pi\leq\chi\leq\pi$, their branches are $\chi=\pm(\pi/2-T)$ and $\chi=\pm(T+\pi/2)$. The common communication region is the diamond $|\chi|+|T|<\pi/2$, the observer's [static patch of de Sitter spacetime](../../../general-relativity.md#static-patch-of-de-sitter-spacetime). These are the [observer horizons in two-dimensional de Sitter spacetime](../../../general-relativity.md#observer-horizons-in-two-dimensional-de-sitter-spacetime). Every complete timelike observer has analogous horizons after a [de Sitter isometry](../../../general-relativity.md#de-sitter-isometry); they depend on the observer, rather than enclosing an intrinsic black-hole region.

Despite these horizons, each constant-$T$ circle is a [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) of the full spacetime: any inextendible [causal curve](../../../general-relativity.md#causal-curve) crosses it exactly once. The global spacetime is therefore [globally hyperbolic](../../../general-relativity.md#globally-hyperbolic-spacetime) and has no [Cauchy horizons](../../../general-relativity.md#cauchy-horizon). The conformal boundaries lie at infinite proper time for complete [timelike geodesics](../../../general-relativity.md#timelike-geodesic) and infinite affine distance for complete [null geodesics](../../../special-relativity.md#null-geodesic), so their finite height in the diagram is not a physical incompleteness.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
