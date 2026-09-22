# Paper 78

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_78.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_78.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)

## 1

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let the fluid approach a uniform, quiescent state $(\rho_0,p_0,c_0)$ at infinity. Use the outward unit [normal vector](../../../differential-geometry.md#normal-vector) $N=\nabla f/|\nabla f|$, pointing from the object into the fluid. Write $H=H(f)$ for the [Heaviside step function](../../../analysis.md#heaviside-step-function), $q=\rho-\rho_0$, and $\delta_S=\delta(f)|\nabla f|$. With the [viscous stress tensor](../../../fluid-mechanics.md#viscous-stress-tensor) $\tau_{ij}$, define

$$
P_{ij}=(p-p_0)\delta_{ij}-\tau_{ij},\qquad T_{ij}=\rho u_i u_j+P_{ij}-c_0^2q\delta_{ij},\qquad L_i=P_{ij}N_j.
$$

Thus $T_{ij}$ is the [Lighthill stress tensor](../../../linear-acoustics.md#lighthill-stress-tensor), and $L_i$ is the surface loading exerted on the fluid. The total [force](../../../classical-mechanics.md#force) on the object has the opposite sign. Extend $q$ by zero inside the object. Since the boundary is fixed and impermeable, $u\cdot N=0$, and the distributional [mass conservation](../../../continuum-mechanics.md#mass-conservation) and [momentum conservation](../../../classical-mechanics.md#momentum-conservation) equations are

$$
\partial_t(Hq)+\partial_i(H\rho u_i)=0,
$$



$$
\partial_t(H\rho u_i)+c_0^2\partial_i(Hq)+\partial_j(HT_{ij})=L_i\delta_S.
$$

For example, the surface contribution to the momentum equation is $(\rho u_i u_j+P_{ij})N_j\delta_S=L_i\delta_S$. Differentiating the first equation in time and subtracting the divergence of the second gives the fixed-body [Ffowcs Williams-Hawkings equation](../../../linear-acoustics.md#ffowcs-williams-hawkings-equation):

$$
\boxed{(\partial_t^2-c_0^2\Delta)(Hq)=\partial_i\partial_j(HT_{ij})-\partial_i(L_i\delta_S).}
$$

There is no [acoustic thickness noise](../../../linear-acoustics.md#acoustic-thickness-noise): a fixed impermeable boundary injects no mass. Apply the [retarded acoustic Green function](../../../wave-equation.md#retarded-acoustic-green-function) $\delta(t-R/c_0)/(4\pi c_0^2R)$, where $R=|x-y|$. The supplied surface-delta identity converts the loading term to a surface integral. For an exterior observer, the required integral equation is

$$
\boxed{q(x,t)=\frac{1}{4\pi c_0^2}\partial_{x_i}\partial_{x_j}\int_{f(y)>0}\frac{T_{ij}(y,t-R/c_0)}{R}\,d^3y-\frac{1}{4\pi c_0^2}\partial_{x_i}\int_{f(y)=0}\frac{L_i(y,t-R/c_0)}{R}\,dS_y.}
$$

This [acoustic analogy](../../../physics.md#acoustic-analogy) is an exact rearrangement of the fluid equations; source approximations enter later. In the distant linear acoustic region, $p'=c_0^2q$.

The [acoustic far field](../../../linear-acoustics.md#acoustic-far-field) requires observer distance $r$ much larger than the source extent $\ell$ and $k_0r\gg1$, so derivatives of the retarded phase dominate derivatives of $1/R$. The [acoustic compact-source approximation](../../../linear-acoustics.md#acoustic-compact-source-approximation) requires $k_0\ell\ll1$, so the source's differential propagation delays can be neglected. These conditions concern different lengths and neither implies the other. Put $n=x/r$, $t_r=t-r/c_0$, and define the loading and stress moments

$$
F_i(t)=\int_S L_i(y,t)\,dS_y,\qquad Q_{ij}(t)=\int_{f>0}T_{ij}(y,t)\,d^3y.
$$

The leading compact [acoustic far field](../../../linear-acoustics.md#acoustic-far-field) is

$$
\boxed{p'(x,t)\simeq\frac{1}{4\pi r}\left[\frac{n_i}{c_0}\dot F_i(t_r)+\frac{n_i n_j}{c_0^2}\ddot Q_{ij}(t_r)\right].}
$$

The surface term is an [acoustic dipole](../../../linear-acoustics.md#acoustic-dipole); the volume term is an [acoustic quadrupole](../../../linear-acoustics.md#acoustic-quadrupole). The plus sign of the loading term follows from the minus sign of its spatial divergence and the derivative of retarded time.

For the power comparison, assume low [Mach number](../../../compressible-flow.md#mach-number) $M=U/c_0$, high [Reynolds number](../../../fluid-mechanics.md#reynolds-number), eddy size $\ell$, characteristic time $\tau=\ell/U$, and stress magnitude $\rho_0U^2$. Keep the prescribed turbulent region and its leading volume stress comparable when inserting the object; neglect changes of source statistics and exceptional cancellations of the leading moments. Compactness follows from $\ell/(c_0\tau)=M\ll1$. Since $Q\sim\rho_0U^2\ell^3$ and the outgoing [acoustic intensity](../../../continuum-mechanics.md#acoustic-energy-flux) is $\langle p'^2\rangle/(\rho_0c_0)$, the volume power is

$$
\boxed{\mathcal P_Q\sim\frac{\rho_0U^8\ell^2}{c_0^5}=\rho_0c_0^3\ell^2M^8.}
$$

If the object's size is comparable to $\ell$ and its fluctuating resultant loading is $F\sim\rho_0U^2\ell^2$, then

$$
\boxed{\mathcal P_D\sim\frac{\rho_0U^6\ell^2}{c_0^3}=\rho_0c_0^3\ell^2M^6,\qquad \mathcal P_D/\mathcal P_Q\sim M^{-2}.}
$$

Angular factors and dimensionless loading coefficients have been omitted. The [acoustic dipole](../../../linear-acoustics.md#acoustic-dipole) and [acoustic quadrupole](../../../linear-acoustics.md#acoustic-quadrupole) interference vanishes in the leading power integrated over a full sphere, by odd angular parity; individual directions can show interference.

A size threshold also requires a loading model. For a small nonseparating object of size $a\ll\ell$ in an approximately inviscid, smoothly varying incident eddy, a spatially uniform pressure has zero resultant on its closed surface. The first surviving loading is the pressure-gradient or [added mass](../../../physics.md#added-mass) force, $F\sim\rho_0a^3U/\tau=\rho_0U^2a^3/\ell$. Under these explicitly stated assumptions,

$$
\mathcal P_D\sim\frac{\rho_0U^6a^6}{c_0^3\ell^4},\qquad \frac{\mathcal P_D}{\mathcal P_Q}\sim\frac{(a/\ell)^6}{M^2}.
$$

**The two mechanisms become comparable at $a\sim\ell M^{1/3}$; for smaller objects the cases with and without the object have the same leading order of power.** This is the [small-body loading-noise threshold](../../../linear-acoustics.md#small-body-loading-noise-threshold). It is not a geometry-independent size law: a separated drag force $F\sim\rho_0U^2a^2$ fluctuating on the original eddy time instead gives $\mathcal P_D/\mathcal P_Q\sim(a/\ell)^4/M^2$ and $a\sim\ell\sqrt M$. If both force and time are set by body-scale eddies, $\tau=a/U$, their loading power is $\rho_0U^6a^2/c_0^3$ and comparison with the original volume source gives $a\sim M\ell$. Each estimate states which source time and force it uses.

The physical distinction is [momentum conservation](../../../classical-mechanics.md#momentum-conservation). Unforced turbulence in a fluid supplies internal stresses, whose net-force contribution cancels and leaves [acoustic quadrupole](../../../linear-acoustics.md#acoustic-quadrupole) radiation. The supported object exchanges momentum with the fluid and the external support, permitting a time-dependent resultant [force](../../../classical-mechanics.md#force) and [acoustic dipole](../../../linear-acoustics.md#acoustic-dipole) radiation. One fewer retarded derivative makes the loading radiation more efficient at low [Mach number](../../../compressible-flow.md#mach-number).

## 2

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Suppress the common time factor $e^{i\omega t}$ and use the [Fourier transform](../../../analysis.md#fourier-transform) convention

$$
\widetilde\phi(k,y)=\int_{\mathbb R}e^{ikx}\phi(x,y)\,dx,\qquad \phi(x,y)=\frac{1}{2\pi}\int_\Gamma e^{-ikx}\widetilde\phi(k,y)\,dk.
$$

A right [Half-range Fourier transform](../../../analysis.md#half-range-fourier-transform) is analytic above its convergence line and a left transform below it. For the [limiting absorption principle](../../../gravity-wave.md#limiting-absorption-principle) with this time convention take $\omega=\omega_r-i\varepsilon$, $\omega_r>0$, $\varepsilon>0$, before taking $\varepsilon\downarrow0$. Set

$$
\gamma(k)=\sqrt{k^2-\omega^2},\qquad \operatorname{Re}\gamma(k)>0\quad(k\in\mathbb R).
$$

This is the [outgoing acoustic square-root branch](../../../linear-acoustics.md#outgoing-acoustic-square-root-branch): at a propagating real wavenumber, $\gamma\to i\sqrt{\omega_r^2-k^2}$. Put $J=[\widetilde\phi]_{y=-0}^{y=+0}$ and $d^+=\partial_y\Phi^+(k,0)$. Across the fluid part of $y=0$, the field and its normal derivative are continuous; on the sheet both sides have the same normal velocity. The outgoing [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) solutions therefore have equal normal derivatives and opposite scattered traces:

$$
\widetilde\phi(k,y)=\begin{cases}\frac12J(k)e^{-\gamma y},&y>0,\\-\frac12J(k)e^{\gamma y},&y<0,\end{cases}\qquad \widetilde\phi_y(k,0)=-\frac{\gamma J}{2}.
$$

The jump $J$ is supported on $x<0$, and so is a minus transform.

The linear fluid equation $i\omega v_y=-\partial_y\rho'$ and the sheet velocity $v_y=i\omega\eta$ imply $\partial_y\rho'=\omega^2\eta$ on either face. The incident contribution to the left derivative transform is $\omega\sin\theta_0/(k+\omega\cos\theta_0)$. Writing $\eta^- =\int_{-\infty}^0e^{ikx}\eta(x)\,dx$, it follows that

$$
-\frac{\gamma J}{2}=\omega^2\eta^- -\frac{\omega\sin\theta_0}{k+\omega\cos\theta_0}+d^+.
$$

The upward net pressure is lower minus upper, hence $P=-J$ in transform space. If $s=\eta'(0)$, the pinned endpoint gives

$$
\widetilde{\eta''}^{\,-}=s-k^2\eta^-,\qquad J=(m\omega^2-Tk^2)\eta^-+Ts.
$$

Combining these identities gives the [Wiener-Hopf equation](../../../differential-equation.md#wiener-hopf-equation)

$$
\boxed{K(k)J(k)+d^+(k)=F(k),\qquad K(k)=\frac{\gamma(k)}2+\frac{\omega^2}{m\omega^2-Tk^2},}
$$



$$
F(k)=\frac{\omega\sin\theta_0}{k+\omega\cos\theta_0}+\frac{T\omega^2s}{m\omega^2-Tk^2}.
$$

This is the [plane-wave forcing of a pinned elastic half-sheet](../../../linear-acoustics.md#plane-wave-forcing-of-a-pinned-elastic-half-sheet).

Let $b=\omega\sqrt{m/T}$ and assume initially that the distinguished points are distinct. Besides the branch points $\pm\omega$, $K$ has simple poles at $\pm b$. Its physical-sheet zeros $\pm k_s$ solve the fluid-loaded [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\gamma(k_s)(Tk_s^2-m\omega^2)=2\omega^2.
$$

For real positive frequency there is exactly one positive real root $k_s>\max(\omega_r,\omega_r\sqrt{m/T})$: the left side increases strictly from zero to infinity on that interval. Equivalently, with $q=\gamma(k_s)>0$, $Tq^3+(T-m)\omega_r^2q-2\omega_r^2=0$. Its other roots have negative real part and do not belong to this outgoing sheet. Continue $k_s$ with small absorption; $+\omega,+b,+k_s$ lie below the real line and their negative partners above it. The [Wiener-Hopf factorization](../../../differential-equation.md#wiener-hopf-factorization) assigns the lower branch cut and pole to $K^+$, and the upper branch cut and pole to $K^-$. The continued $K^+$ has a zero at $+k_s$, and $K^-$ at $-k_s$; these are poles of their reciprocals, rather than poles of the factors. Branch cuts can be drawn away from the real line into the corresponding half-planes.

For this standard assignment a common strip of analyticity and nonvanishing is

$$
\boxed{\mathcal D=\{k:-d<\operatorname{Im}k<d\},\qquad d=\min\{\varepsilon,\ \varepsilon\sqrt{m/T},\ -\operatorname{Im}k_s\}>0.}
$$

The strip shrinks to the real contour as absorption is removed. The factors continue meromorphically beyond their designated half-planes; the allocation of the poles and branch points is part of the [radiation condition](../../../gravity-wave.md#radiation-condition). The incident pole $-\omega\cos\theta_0$ belongs above the inversion contour. For incidence with $0<\theta_0<\pi/2$ the real contour is a direct choice. Other nongrazing angles are obtained by [analytic continuation](../../../complex-analysis.md#analytic-continuation) with the incident pole kept on its prescribed side, deforming the contour locally if necessary. Coincident distinguished points and grazing incidence are treated by the corresponding limits, not by dividing by a coincident pole.

Divide the [Wiener-Hopf equation](../../../differential-equation.md#wiener-hopf-equation) by $K^+$ and use [pole subtraction in a Wiener-Hopf equation](../../../differential-equation.md#pole-subtraction-in-a-wiener-hopf-equation). With $a=\omega\cos\theta_0$, the minus part of $F/K^+$ is

$$
B^-(k)=\frac{\omega\sin\theta_0}{K^+(-a)(k+a)}+\frac{\omega^2s}{2bK^+(-b)(k+b)}.
$$

Indeed these are exactly the incident-pole and upper bare-sheet-pole residues. At the lower bare-sheet pole $+b$, the forcing pole is canceled by the pole of $K^+$ before splitting. Thus $B^+=F/K^+-B^-$ is analytic on the plus side of the contour. The separated equation is

$$
K^-J-B^-=B^+-d^+/K^+=E.
$$

With the stipulated $E=0$,

$$
J=\frac{B^-}{K^-},\qquad d^+=K^+B^+=F-K^+B^-.
$$

The scattered field is consequently

$$
\boxed{\phi(x,y)=\frac{\operatorname{sgn}y}{4\pi}\int_\Gamma e^{-ikx-\gamma(k)|y|}\frac{B^-(k)}{K^-(k)}\,dk,\qquad y\ne0.}
$$

The full time-dependent density perturbation is the incident field plus $e^{i\omega t}\phi$. The two traces at $y=0$ follow by limiting from above and below. A constant rescaling of the two factors does not change this field.

To determine the endpoint slope, reconstruct the sheet transform using the fluid condition:

$$
\eta^-(k)=\frac1{\omega^2}\left[-\frac{\gamma J}{2}-d^++\frac{\omega\sin\theta_0}{k+a}\right]=\frac{J-Ts}{m\omega^2-Tk^2}.
$$

At $+b$ the continued $K^+$ has residue $-\omega^2/(2TbK^-(b))$. Therefore the derivative transform $d^+$ generically has the lower-plane pole

$$
\operatorname{Res}_{k=b}d^+=-\frac{\omega^2s}{2b}+\frac{\omega^2B^-(b)}{2TbK^-(b)}.
$$

This pole produces a forbidden incoming bare-sheet wave in the reconstructed displacement: $e^{i\omega t-ibx}$ travels towards the endpoint from $x=-\infty$. A minus transform of the specified outgoing solution must be analytic there. The [incoming-pole cancellation at a pinned membrane edge](../../../linear-acoustics.md#incoming-pole-cancellation-at-a-pinned-membrane-edge) is precisely

$$
\boxed{B^-(b)=TsK^-(b),\qquad J(b)=Ts.}
$$

For generic parameters this determines

$$
\boxed{s=\frac{\omega\sin\theta_0}{K^+(-a)(b+a)\left[TK^-(b)-\dfrac{\omega^2}{4b^2K^+(-b)}\right]}.}
$$

The lower pole is removed; the upper zero $-k_s$ of $K^-$ can still produce the legitimate outgoing [evanescent acoustic surface wave](../../../linear-acoustics.md#evanescent-acoustic-surface-wave), whose phase travels to negative $x$. This distinction separates the spurious bare-sheet wave from the coupled fluid-loaded mode. No explicit factorization has been used.

## 3

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the [scattering potential](../../../inverse-problem.md#scattering-potential) convention $V=k_0^2(n^2-1)$. With time dependence $e^{-i\omega t}$ the outgoing [Green function](../../../analysis.md#green-s-function) is $G_0(r,r')=e^{ik_0|r-r'|}/(4\pi|r-r'|)$ and satisfies $(\Delta+k_0^2)G_0=-\delta$. The total-field [Lippmann-Schwinger equation](../../../quantum-mechanics.md#lippmann-schwinger-equation) is

$$
\psi(r)=\psi_0(r)+\int_DG_0(r,r')V(r')\psi(r')\,d^3r'.
$$

Replacing the field in the integral by the incident field gives the first [Born approximation for scalar wave scattering](../../../inverse-problem.md#born-approximation-for-scalar-wave-scattering):

$$
\boxed{\psi_B=\psi_0+\psi_1,\qquad \psi_1(r)=\int_DG_0(r,r')V(r')\psi_0(r')\,d^3r'.}
$$

For the first [Rytov approximation](../../../inverse-problem.md#rytov-approximation), write $\psi=\psi_0e^\chi$ on a region where the incident field is nonzero and a continuous [complex logarithm](../../../analysis.md#complex-logarithm) can be chosen. The [logarithmic wave perturbation](../../../inverse-problem.md#logarithmic-wave-perturbation) equation is

$$
\Delta\chi+2\nabla\log\psi_0\cdot\nabla\chi+\nabla\chi\cdot\nabla\chi=-V.
$$

The last dot product is bilinear, not a squared modulus. Dropping it leaves a linear equation for $\chi_1$. Multiplication by $\psi_0$ shows that $\psi_0\chi_1$ satisfies the same outgoing inhomogeneous [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) as $\psi_1$. Hence

$$
\boxed{\chi_1=\frac{\psi_1}{\psi_0},\qquad \psi_R=\psi_0\exp\left(\frac{\psi_1}{\psi_0}\right).}
$$

Introduce a small multiplier $\lambda$ on $V$. Then $\psi_1=O(\lambda)$ and

$$
\psi_R=\psi_0+\psi_1+\frac{\psi_1^2}{2\psi_0}+O(\lambda^3)=\psi_B+O(\lambda^2).
$$

**The two total-field approximations agree to first order.** Exponentiating the first [logarithmic wave perturbation](../../../inverse-problem.md#logarithmic-wave-perturbation) does not supply the generally missing second-order [Born series](../../../inverse-problem.md#born-series) contribution.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write the observation point as $r\widehat r$, put $q=k_0(\widehat r-\widehat r_0)$, and take $\psi_0(r\widehat r)=e^{ik_0r\widehat r_0\cdot\widehat r}$. For a bounded medium, the [far-field approximation for an outgoing source](../../../inverse-problem.md#far-field-approximation-for-an-outgoing-source) uses

$$
|r\widehat r-r'|=r-\widehat r\cdot r'+O(\ell^2/r),\qquad G_0\simeq\frac{e^{ik_0r}}{4\pi r}e^{-ik_0\widehat r\cdot r'}.
$$

For finite-distance accuracy require $r\gg\ell$ and $k_0\ell^2/r\ll1$ as well as being in the radiation region. Define the [Fourier transform](../../../analysis.md#fourier-transform) sample $S(q)=\int_DV(r')e^{-iq\cdot r'}\,d^3r'$ and the known factor

$$
B(r,\widehat r)=\frac{e^{ik_0r(1-\widehat r_0\cdot\widehat r)}}{4\pi r}.
$$

Then the required total [Born approximation for scalar wave scattering](../../../inverse-problem.md#born-approximation-for-scalar-wave-scattering) and total [Rytov approximation](../../../inverse-problem.md#rytov-approximation) are

$$
\boxed{\psi_B(r\widehat r)\simeq e^{ik_0r\widehat r_0\cdot\widehat r}+\frac{e^{ik_0r}}{4\pi r}S(q),\qquad \psi_R(r\widehat r)\simeq e^{ik_0r\widehat r_0\cdot\widehat r}\exp\{B S(q)\}.}
$$

The first [Born approximation](../../../quantum-theory.md#born-approximation) [far-field pattern](../../../inverse-problem.md#far-field-pattern) is $S(q)/(4\pi)$. In both formulas the incident field is retained; an outgoing scattered term alone would not be a total-field answer.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The zero-mean fluctuation is $W$, not the [refractive index](../../../electromagnetism.md#refractive-index) $n$: $\langle n\rangle=1$. Also the full [scattering potential](../../../inverse-problem.md#scattering-potential) has a nonzero mean and is not Gaussian:

$$
V=2\mu k_0^2W+\mu^2k_0^2W^2,\qquad \overline V=\mu^2k_0^2.
$$

The usual Gaussian closure requires $W$ to be a jointly [Gaussian random field](../../../stochastic-process.md#gaussian-random-field), not merely to have a [Gaussian distribution](../../../probability-theory.md#normal-distribution) at each point. We first give the intended leading weak-fluctuation result with the linearized potential $V_1=2\mu k_0^2W$, then account for the quadratic term.

Keep the definitions $q,B$ from the preceding solution and let $\chi_1=B\int_D V_1(y)e^{-iq\cdot y}\,dy$. Because the incident field has unit modulus,

$$
I=\langle e^{\chi_1+\chi_1^*}\rangle,\qquad h(y)=B e^{-iq\cdot y}+B^*e^{iq\cdot y}=2\operatorname{Re}(B e^{-iq\cdot y}).
$$

The exponent is a real Gaussian linear functional $Z=\int_DhV_1$. If $C_W(y-z)=\langle W(y)W(z)\rangle$, the linearized potential has [autocorrelation function of a random field](../../../stochastic-process.md#autocorrelation-function-of-a-random-field) $C_1(s)=4\mu^2k_0^4 C_W(s)$. Complete the square in the one-dimensional Gaussian density of $Z$: $\langle e^Z\rangle=\exp(\langle Z\rangle+\operatorname{Var}Z/2)$. Here its mean is zero, so

$$
\boxed{I_{\mathrm{lin}}=\exp\left\{\frac12\int_D\int_D h(y)h(z)C_1(y-z)\,dy\,dz\right\}.}
$$

This is [Gaussian intensity in the first Rytov approximation](../../../inverse-problem.md#gaussian-intensity-in-the-first-rytov-approximation). In a more explicit complex notation, put

$$
J_1=\int_D\int_D C_1(y-z)e^{-iq\cdot(y-z)}\,dy\,dz,\qquad J_2=\int_D\int_D C_1(y-z)e^{-iq\cdot(y+z)}\,dy\,dz.
$$

Then

$$
\boxed{I_{\mathrm{lin}}=\exp\{|B|^2J_1+\operatorname{Re}(B^2J_2)\}.}
$$

The second term is the [pseudo-covariance of a complex random variable](../../../variance.md#pseudo-covariance) contribution. It does not vanish for an arbitrary finite real medium. The real-kernel expression shows that the combined exponent is nonnegative, even though its two complex-form contributions need not be separately nonnegative.

For the full potential, [Gaussian moment pairing theorem](../../../probability-theory.md#isserlis-s-theorem) gives its centered [covariance function](../../../stochastic-process.md#covariance-function)

$$
C_V(s)=\operatorname{Cov}(V(y),V(y+s))=4\mu^2k_0^4C_W(s)+2\mu^4k_0^4C_W(s)^2.
$$

Its uncentered autocorrelation is $R_V(s)=C_V(s)+\mu^4k_0^4$. The first [Rytov approximation](../../../inverse-problem.md#rytov-approximation) is linear in $V$, but its intensity is an exponential average; applying a Gaussian formula exactly to this quadratic potential would be incorrect. A consistent expansion through order $\mu^2$ is

$$
\boxed{\log I=2\mu^2k_0^2\operatorname{Re}\left[B\int_De^{-iq\cdot y}\,dy\right]+\frac12\int_D\int_D h(y)h(z)C_1(y-z)\,dy\,dz+O(\mu^4).}
$$

The first term is the coherent mean-potential correction. Odd powers vanish by the symmetry of the joint Gaussian field. The variance term can equally use $C_V=R_V-\overline V^2$ through this order. Thus the mean shift must not be discarded while retaining the order-$\mu^2$ fluctuation intensity.

An exact expression within the far-field, first-[Rytov approximation](../../../inverse-problem.md#rytov-approximation) model is also available when the full $n^2$ is retained. Assume the restriction of $W$ to $D$ is a Gaussian element of the real [Hilbert space](../../../hilbert-space.md) $L^2(D)$, with covariance operator $C$ of kernel $C_W(y-z)$. Let $H$ denote multiplication by $h$, $\ell_h=2\mu k_0^2h$, $Q=\mu^2k_0^2 C^{1/2}HC^{1/2}$ and $b_h=C^{1/2}\ell_h$. The [Gaussian quadratic exponential moment](../../../stochastic-process.md#gaussian-quadratic-exponential-moment) is

$$
\boxed{I=\det(I-2Q)^{-1/2}\exp\left[\frac12\langle b_h,(I-2Q)^{-1}b_h\rangle\right].}
$$

Here the determinant is the [Fredholm determinant](../../../compact-operator.md#fredholm-determinant); require $I-2Q$ strictly positive for finiteness. Diagonalize the self-adjoint trace-class operator $Q$ and complete the square in each Gaussian coordinate to derive the formula. On a bounded $D$, unit pointwise variance makes $\operatorname{tr}C=|D|$, so the covariance is trace class under the stated measurable $L^2$ hypothesis. Small enough $\mu$ satisfies the positivity condition. Expanding the determinant and inverse recovers the preceding mean and covariance terms. For small $\mu$ this is also determined by the potential autocorrelation: since $C_W\in[-1,1]$,

$$
C_W(s)=\frac{-1+\sqrt{1+C_V(s)/(2k_0^4)}}{\mu^2},\qquad C_V=R_V-\mu^4k_0^4,
$$

using the branch near zero. This makes explicit the extra joint-Gaussian assumption behind an exact correlation-based answer.

Finally, Gaussian marginals alone are insufficient. Take $X\sim N(0,1)$ and independent random signs $S_j$. The stationary sequence $W_j=S_jX$ has Gaussian marginals and covariance $\langle W_iW_j\rangle=\delta_{ij}$, just like independent standard Gaussian variables. However $\langle e^{t(W_1+W_2)}\rangle=(1+e^{2t^2})/2$, whereas for the independent Gaussian pair it is $e^{t^2}$. The different intensities show why the joint hypothesis is needed. The mean-zero hint is interpreted for $W$, and the linearized Gaussian formula is not claimed to be exact for $V=k_0^2(n^2-1)$.

## 4

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use the [inner product](../../../linear-algebra.md#inner-product) convention linear in its first argument. A [singular value system](../../../inverse-problem.md#singular-system-of-a-compact-operator) consists of positive [singular values](../../../linear-algebra.md#singular-value) $\sigma_n$ and [orthonormal bases](../../../linear-algebra.md#orthonormal-basis) $u_n$ of $(\ker A)^\perp\subset X$ and $v_n$ of $\overline{\operatorname{ran}A}\subset Y$, with

$$
Au_n=\sigma_n v_n,\qquad A^*v_n=\sigma_nu_n.
$$

For an infinite-rank [compact operator](../../../compact-operator.md), $\sigma_n\to0$; a finite-rank operator has a finite system. Applying the [spectral theorem for compact self-adjoint operators](../../../compact-operator.md#spectral-theorem-for-compact-hermitian-operators) to $A^*A$ constructs $u_n$, with eigenvalues $\sigma_n^2$, and then $v_n=Au_n/\sigma_n$. This solution uses the input/output naming of this problem, which is the reverse of another common singular-vector convention.

The [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) is

$$
\boxed{x^\dagger=A^\dagger y=\sum_n\frac{\langle y,v_n\rangle}{\sigma_n}u_n.}
$$

Its domain is $\operatorname{ran}A\oplus(\operatorname{ran}A)^\perp$, equivalently the data satisfying the [Picard criterion](../../../inverse-problem.md#picard-criterion)

$$
\sum_n\frac{|\langle y,v_n\rangle|^2}{\sigma_n^2}<\infty.
$$

It ignores the component in $\ker A^*$ and lies in $(\ker A)^\perp$. The series then converges in $X$ by orthonormality and is the [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution). If $y\in\operatorname{ran}A$, it is an exact solution; all other exact solutions are $x^\dagger+z$ with $z\in\ker A$. Compactness does not make the inverse bounded when there are infinitely many positive singular values.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A [linear regularization](../../../inverse-problem.md#linear-regularization) is a family of bounded operators $R_\alpha:Y\to X$ such that $R_\alpha y\to A^\dagger y$ for every $y$ in the domain of the [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) as $\alpha\downarrow0$. For noisy data $\|y^\delta-y\|\leq\delta$, a [convergent regularization of an inverse problem](../../../inverse-problem.md#convergent-regularization-of-an-inverse-problem) also specifies a parameter choice $\alpha(\delta,y^\delta)$ giving convergence to $A^\dagger y$, uniformly over the allowed noise at each fixed admissible exact datum.

Expand $x_\alpha$ in the input singular vectors. The [Tikhonov normal equation](../../../inverse-problem.md#tikhonov-normal-equation) implies

$$
(\alpha+\sigma_n^2)\langle x_\alpha,u_n\rangle=\sigma_n\langle y,v_n\rangle.
$$

The component in $\ker A$ is zero because $\alpha>0$. Comparing with the given filter convention gives

$$
\boxed{f_\alpha(\sigma)=\frac{\sigma^2}{\alpha+\sigma^2},\qquad R_\alpha y=\sum_n\frac{\sigma_n}{\alpha+\sigma_n^2}\langle y,v_n\rangle u_n.}
$$

The [singular-system Tikhonov filter](../../../inverse-problem.md#singular-system-tikhonov-filter) is often described by its gain $g_\alpha(\sigma)=\sigma/(\alpha+\sigma^2)$; the requested $f_\alpha$ includes one extra factor of $\sigma$. For admissible data, $f_\alpha\to1$ and $0\leq f_\alpha\leq1$, so [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) applied to the squared [Picard criterion](../../../inverse-problem.md#picard-criterion) coefficients proves exact-data convergence. Also

$$
\|R_\alpha\|\leq\sup_{\sigma\geq0}\frac{\sigma}{\alpha+\sigma^2}=\frac{1}{2\sqrt\alpha}.
$$

By the [noise-bias decomposition for linear regularization](../../../inverse-problem.md#noise-bias-decomposition-for-linear-regularization), $\alpha(\delta)\to0$ and $\delta/\sqrt{\alpha(\delta)}\to0$ suffice for noisy-data convergence; for example $\alpha=\delta$ as $\delta\downarrow0$. This establishes both consistency and stability of [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

For $f,g\in L^2(0,1)$, interchange the integrals in the [inner product](../../../linear-algebra.md#inner-product) of the [Volterra integration operator](../../../functional-analysis.md#volterra-operator):

$$
\langle Af,g\rangle=\int_0^1\int_0^x f(t)\overline{g(x)}\,dt\,dx=\int_0^1f(t)\overline{\int_t^1g(x)\,dx}\,dt.
$$

Thus the [adjoint operator](../../../hilbert-space.md#adjoint-operator) is $A^*g(t)=\int_t^1g(x)\,dx$. The triangular integration kernel is square-integrable, so $A$ is a [Hilbert-Schmidt operator](../../../compact-operator.md#hilbert-schmidt-operator) and hence a [compact operator](../../../compact-operator.md).

Set $a_n=(n-\tfrac12)\pi$ and $\sigma_n=1/a_n$. Direct integration gives

$$
Au_n(x)=\sqrt2\int_0^x\cos(a_nt)\,dt=\sigma_n\sqrt2\sin(a_nx)=\sigma_nv_n(x),
$$



$$
A^*v_n(x)=\sqrt2\int_x^1\sin(a_nt)\,dt=\sigma_n\sqrt2\cos(a_nx)=\sigma_nu_n(x),
$$

since $\cos a_n=0$. Product-to-sum identities give $\langle u_n,u_j\rangle=\langle v_n,v_j\rangle=\delta_{nj}$. For completeness, $g=A^*Af$ satisfies $g''=-f$, $g'(0)=0$, $g(1)=0$. The associated [Sturm-Liouville problem](../../../analysis.md#sturm-liouville-problem) has precisely the complete mixed-boundary cosine basis $u_n$; $AA^*$ gives the mixed-boundary sine basis $v_n$, with $v_n(0)=0$, $v_n'(1)=0$. Both $A$ and $A^*$ are injective, since differentiation of their zero integrals recovers their inputs. Their singular vectors therefore cover the entire two [Hilbert spaces](../../../hilbert-space.md), rather than just proper orthogonal complements.

**The given functions form the complete [singular value system](../../../inverse-problem.md#singular-system-of-a-compact-operator), with $\sigma_n=2/((2n-1)\pi)$.** This is the [mixed-boundary singular system of the Volterra operator](../../../functional-analysis.md#mixed-boundary-singular-system-of-the-volterra-operator).

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Substitution into the [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization) series gives an explicit reconstruction for every $y\in L^2(0,1)$:

$$
\boxed{x_\alpha(x)=\sum_{n=1}^{\infty}\frac{a_n}{1+\alpha a_n^2}\left[\int_0^1 y(t)\sqrt2\sin(a_nt)\,dt\right]\sqrt2\cos(a_nx),\qquad a_n=(n-\tfrac12)\pi.}
$$

Equivalently the summand is $\sigma_n\langle y,v_n\rangle u_n/(\alpha+\sigma_n^2)$. The [Tikhonov stability bound](../../../inverse-problem.md#tikhonov-stability-bound) makes the series converge in $L^2$ for every positive $\alpha$. It suppresses high-frequency components of unstable differentiation, rather than differentiating arbitrary noisy data pointwise.

The [range of the Volterra integration operator](../../../functional-analysis.md#range-of-the-volterra-integration-operator) is $\{y\in H^1(0,1):y(0)=0\}$. On exactly these data, $A^\dagger y=y'$ and the series converges to $y'$ as $\alpha\downarrow0$. For arbitrary $L^2$ data outside that range, a finite regularized solution still exists, but a finite-norm unregularized solution need not exist. This is [Spectral Tikhonov differentiation for the Volterra operator](../../../functional-analysis.md#spectral-tikhonov-differentiation-for-the-volterra-operator).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
