# Paper 64

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper64.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper64.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)

## 1

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $h_{ij}={}^{(3)}g_{ij}$ for the [induced metric](../../../riemannian-geometry.md#induced-metric) and lower the [shift vector](../../../numerical-relativity.md#shift-vector) with it, $N_i=h_{ij}N^j$. In the stated negative-shift convention the four-dimensional components and inverse components are

$$
g_{00}=-N^2+N_iN^i,\quad g_{0i}=-N_i,\quad g_{ij}=h_{ij},
\qquad g^{00}=-\frac1{N^2},\quad g^{0i}=-\frac{N^i}{N^2}.
$$

Multiplying the given future [unit normal](../../../differential-geometry.md#unit-normal) by this [metric tensor](../../../general-relativity.md#metric-tensor) gives $n_\mu=(-N,0,0,0)$. In particular the tangential normal components vanish, but their [covariant derivatives](../../../general-relativity.md#covariant-derivative) do not:

$$
n_{i;j}=-\Gamma^\mu{}_{ij}n_\mu=N\Gamma^0{}_{ij},\qquad K_{ij}=-N\Gamma^0{}_{ij}.
$$

The relevant [Christoffel symbol](../../../riemannian-geometry.md#christoffel-symbol) is

$$
\begin{aligned}
\Gamma^0{}_{ij}
&=\frac1{2N^2}\left[\dot h_{ij}+\partial_iN_j+\partial_jN_i
-N^k(\partial_i h_{jk}+\partial_jh_{ik}-\partial_kh_{ij})\right]\\
&=\frac1{2N^2}\left(\dot h_{ij}+N_{i|j}+N_{j|i}\right).
\end{aligned}
$$

For the second equality, the last parenthesis is $2h_{k\ell}{}^{(3)}\Gamma^\ell{}_{ij}$, so its contraction subtracts the two spatial connection terms in the symmetrized derivative of $N_i$. Therefore

$$
\boxed{K_{ij}=-\frac1{2N}\left(\dot h_{ij}+N_{i|j}+N_{j|i}\right).}
$$

This is [extrinsic curvature with a negative shift](../../../numerical-relativity.md#extrinsic-curvature-with-a-negative-shift). Both the future-normal orientation and the definition $K=-\nabla n$ matter: replacing the threading by $dx^i+N^idt$ reverses the shift terms. The spatial [induced metric](../../../riemannian-geometry.md#induced-metric) is generally a function of time as well as position; restricting it to time-independent data would simply make the displayed time derivative vanish.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Retain the homogeneous [lapse function](../../../numerical-relativity.md#lapse-function) $\bar N(t)$, and define the physical [Hubble parameter](../../../cosmology.md#hubble-parameter) $H=\dot a/(\bar Na)$. At first order the scalar [metric perturbations](../../../general-relativity.md#linearized-gravity) give $\delta g_{00}=-2\bar N^2\Phi$, $\delta g_{0i}=a^2B_{,i}$, and $\delta g_{ij}=-2a^2(\Psi\delta_{ij}+E_{,ij})$. Applying the passive coordinate displacement component by component gives the [scalar gauge transformations with a background lapse](../../../linear-cosmological-perturbation-theory.md#scalar-gauge-transformations-with-a-background-lapse)

$$
\boxed{\widetilde\Phi=\Phi-\dot\xi^0-\frac{\dot{\bar N}}{\bar N}\xi^0,\quad
\widetilde B=B-\dot\lambda+\frac{\bar N^2}{a^2}\xi^0,\quad
\widetilde\Psi=\Psi+\frac{\dot a}{a}\xi^0,\quad
\widetilde E=E+\lambda.}
$$

For example the $0i$ transformation is $\delta\widetilde g_{0i}=a^2\partial_iB-a^2\partial_i\dot\lambda+\bar N^2\partial_i\xi^0$. The spatial isotropic part acquires $-2a\dot a\xi^0\delta_{ij}$, explaining the positive sign in the transformation of $\Psi$.

Preserving [synchronous gauge](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) requires both transformed $\Phi$ and $B$ to remain zero. The first condition is $\partial_t(\bar N\xi^0)=0$, and the second is $\dot\lambda=\bar N^2\xi^0/a^2$. Integrating them gives

$$
\boxed{\xi^0=\frac{C(\mathbf x)}{\bar N},\qquad
\lambda=C(\mathbf x)\int^t\frac{\bar N(t')}{a(t')^2}dt'+D(\mathbf x).}
$$

Thus fixing the [lapse function](../../../numerical-relativity.md#lapse-function) and [shift vector](../../../numerical-relativity.md#shift-vector) perturbations does not exhaust the scalar coordinate freedom. The functions $C,D$ describe [residual synchronous-gauge freedom](../../../linear-cosmological-perturbation-theory.md#residual-synchronous-gauge-freedom); an integration-origin change in the integral is absorbed into $D$.

To move from [synchronous gauge](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) to [Newtonian gauge](../../../linear-cosmological-perturbation-theory.md#newtonian-gauge), choose $\lambda=-E_S$ to set $\widetilde E=0$. Requiring $\widetilde B=0$ then gives

$$
\xi^0=-\frac{a^2}{\bar N^2}\dot E_S.
$$

A scalar [energy density](../../../statistical-physics.md#energy-density) transforms as $\delta\rho_N=\delta\rho_S-\dot{\bar\rho}\xi^0$. Dividing by the background [energy density](../../../statistical-physics.md#energy-density), which changes the contrast only at second order if perturbed in that denominator, yields the [synchronous-to-Newtonian density transformation with a lapse](../../../linear-cosmological-perturbation-theory.md#synchronous-to-newtonian-density-transformation-with-a-lapse)

$$
\boxed{\delta_N=\delta_S+\frac{a^2\dot E_S}{\bar N^2}\frac{\dot{\bar\rho}}{\bar\rho}
=\delta_S-3(1+w)\frac{a^2H}{\bar N}\dot E_S,
\qquad\delta=\frac{\delta\rho}{\bar\rho}.}
$$

The last form uses background [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation), $\dot{\bar\rho}=-3\bar NH(\bar\rho+\bar P)$. With [cosmic time](../../../cosmology.md#cosmic-time) $\bar N=1$ this is $\delta_N=\delta_S-3(1+w)a^2H\dot E_S$; with [conformal time](../../../cosmology.md#conformal-time) $\bar N=a$ it is $\delta_N=\delta_S-3(1+w)\mathcal H E_S'$, where $\mathcal H=a'/a$. Keeping these clock conventions distinct is essential to the factors of $a$.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Use the spatial-potential convention of this paper and assume $\bar\rho+\bar P\ne0$. A passive time displacement changes the spatial scalar by $\widetilde\Psi-\Psi=\bar NH\xi^0$ and changes the [energy density](../../../statistical-physics.md#energy-density) by

$$
\delta\widetilde\rho-\delta\rho=-\dot{\bar\rho}\xi^0
=3\bar NH(\bar\rho+\bar P)\xi^0.
$$

The two contributions to the [uniform-density curvature perturbation](../../../linear-cosmological-perturbation-theory.md#uniform-density-curvature-perturbation) therefore cancel:

$$
\widetilde\zeta-\zeta=-\bar NH\xi^0+
\frac{3\bar NH(\bar\rho+\bar P)\xi^0}{3(\bar\rho+\bar P)}=0.
$$

A spatial scalar displacement changes $E$ but not this combination. Hence **$\zeta$ is gauge invariant at linear order**. Pure cosmological-constant matter, for which $\bar\rho+\bar P=0$, does not supply a [energy density](../../../statistical-physics.md#energy-density) clock and this formula is not defined for that component alone.

Now take the definite constant-$w$ [barotropic equation of state](../../../cosmology.md#barotropic-equation-of-state) and use physical-time differentiation $\mathcal D=\bar N^{-1}\partial_t$. Put $A=\bar\rho+\bar P$. Background [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation) gives $\mathcal DA=-3H(1+w)A$. Differentiating $\zeta=-\Psi+\delta\rho/(3A)$, then substituting the two supplied perturbation equations, gives

$$
\begin{aligned}
\mathcal D\zeta
&=-\mathcal D\Psi+\frac{\mathcal D\delta\rho}{3A}
+H(1+w)\frac{\delta\rho}{A}\\
&=H\Phi-\frac\kappa3-\frac{\Delta\chi}3
-H\frac{\delta\rho+\delta P}{A}+\frac\kappa3-H\Phi
-\frac{\Delta u}{3A}+H(1+w)\frac{\delta\rho}{A}\\
&=-\frac H A(\delta P-w\delta\rho)
-\frac13\Delta\left(\chi+\frac uA\right).
\end{aligned}
$$

Thus the lapse and expansion perturbations cancel without imposing a gauge. In terms of the [non-adiabatic pressure perturbation](../../../cosmic-inflation.md#non-adiabatic-pressure-perturbation) $\delta P_{\rm nad}=\delta P-w\delta\rho$,

$$
\boxed{\frac{\dot\zeta}{\bar N}=-\frac{H\delta P_{\rm nad}}{\bar\rho+\bar P}
-\frac13\Delta\left(\chi+\frac{u}{\bar\rho+\bar P}\right).}
$$

For the stipulated [barotropic equation of state](../../../cosmology.md#barotropic-equation-of-state), $\delta P=w\delta\rho$, so the first term vanishes. For a [Fourier mode](../../../fourier-analysis.md#fourier-mode), $\Delta=-k^2/a^2$. For regular long-wavelength solutions the remaining gradients are suppressed when $k\ll aH$. Consequently **$\dot\zeta\simeq0$ on [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale)**, with exact conservation in the leading zero-gradient limit. It is not an exact finite-$k$ identity. Entropy perturbations or a singular [gradient expansion](../../../critical-phenomenon.md#gradient-expansion) can invalidate that conclusion; the supplied adiabatic assumption is what removes the unsuppressed [pressure](../../../thermodynamics.md#pressure) source.

This [superhorizon conservation of uniform-density curvature](../../../linear-cosmological-perturbation-theory.md#superhorizon-conservation-of-uniform-density-curvature) is useful because inflationary fluctuations leave the horizon during [cosmic inflation](../../../cosmic-inflation.md) and may re-enter only much later. In an adiabatic single-clock evolution, the conserved [uniform-density curvature perturbation](../../../linear-cosmological-perturbation-theory.md#uniform-density-curvature-perturbation) transports their initial amplitude through reheating and the later [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology) and matter eras without solving every short-distance process. It then determines the initial conditions for large-scale structure and [Cosmic microwave background anisotropy](../../../cosmic-microwave-background-anisotropy.md). Extra fluctuating fields or fluids can introduce [isocurvature perturbations](../../../cosmic-inflation.md#cosmological-entropy-perturbation) and convert them into curvature, so conservation must be checked rather than assumed during such transitions.

## 2

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Let $\mathcal H=a'/a$ and $\theta_N=i\mathbf k\cdot\mathbf v_N$. Choose the [synchronous gauge](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) rest frame of [cold dark matter](../../../cosmology.md#cold-dark-matter), so $\theta_C=0$. Its continuity equation then gives $h'=-2\delta_C'$. Substitution in the trace Einstein equation gives

$$
\boxed{\delta_C''+\mathcal H\delta_C'
-\frac32\mathcal H^2(\Omega_C\delta_C+2\Omega_R\delta_R)=0.}
$$

For [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology) the continuity and Euler equations are $\delta_R'+4\theta_R/3+2h'/3=0$ and $\theta_R'=k^2\delta_R/4$. Differentiate the first, eliminate $\theta_R'$ and $h''$, and obtain

$$
\boxed{\delta_R''+\frac{k^2}3\delta_R-\frac43\delta_C''=0.}
$$

[radiation in cosmology](../../../cosmology.md#radiation-in-cosmology) [pressure](../../../thermodynamics.md#pressure) supplies the acoustic restoring term while its [energy density](../../../statistical-physics.md#energy-density) contributes twice as strongly to the trace gravitational source through $1+3w_R=2$.

Deep in [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), $a\propto\tau$, $\mathcal H=1/\tau$, $\Omega_R\simeq1$ and $\Omega_C\simeq0$. At long wavelengths $k\tau\ll1$, the [adiabatic initial conditions](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) require $\delta_C=3\delta_R/4$. The cold-matter equation reduces to

$$
\delta_C''+\frac1\tau\delta_C'-\frac4{\tau^2}\delta_C=0.
$$

A power $\tau^p$ gives $p^2-4=0$. The regular growing solution therefore has

$$
\boxed{\delta_C=A(\mathbf k)\tau^2,\qquad
\delta_R=\frac43A(\mathbf k)\tau^2,\qquad k\tau\ll1.}
$$

The other adiabatic solution diverges as $\tau^{-2}$ and is discarded for the regular primordial growing mode. The relation between the [density contrasts](../../../linear-cosmological-density-perturbation.md#density-contrast) fixes their relative entropy to zero, not their subsequent equality inside the acoustic horizon.

One can also solve the leading radiation-era equations explicitly, which proves that the same regular mode develops logarithmic cold-matter growth after horizon entry. Put $x=k\tau/\sqrt3$. The first equation gives $\delta_R=(x^2\delta_{C,xx}+x\delta_{C,x})/3$. Substituting in the second gives

$$
x^2\delta_{C,xxxx}+5x\delta_{C,xxx}+x^2\delta_{C,xx}+x\delta_{C,x}=0.
$$

Define

$$
F(x)=\int_0^x\frac{1-\cos t}{t}dt+
\frac{\sin x}{x}-\frac{1-\cos x}{x^2}-\frac12.
$$

Its useful derivative is $F'=1/x-2\sin x/x^2+2(1-\cos x)/x^3$. Direct differentiation verifies the fourth-order equation and gives the associated [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology) solution:

$$
\delta_C=K(\mathbf k)F(x),\qquad
\delta_R=\frac K3\left[-2\cos x+\frac{4\sin x}x
-\frac{4(1-\cos x)}{x^2}\right].
$$

At zero, $F=x^2/8+O(x^4)$ and $\delta_R=Kx^2/6+O(x^4)$, so this is precisely the regular [adiabatic radiation-era cold-dark-matter transfer solution](../../../linear-cosmological-density-perturbation.md#adiabatic-radiation-era-cold-dark-matter-transfer-solution) with $K=24A/k^2$. The other indicial behaviors of the fourth-order equation are $1,x,x^{-2}$; they are either nonadiabatic at leading order or singular and do not add another regular growing adiabatic mode.

For $x\gg1$, the integral is $\gamma+\ln x-\operatorname{Ci}(x)$, where $\gamma$ is the [Euler's constant](../../../complex-analysis.md#euler-s-constant) and $\operatorname{Ci}$ the [cosine integral](../../../calculus.md#cosine-integral). Its oscillatory tail cancels the explicit leading $\sin x/x$ term, giving

$$
\delta_C=K\left[\ln x+\gamma-\frac12+O(x^{-2})\right],\qquad
\delta_R=-\frac{2K}3\cos x+O(x^{-1}).
$$

Thus the requested late sound-horizon behavior is

$$
\boxed{\delta_C\simeq B(\mathbf k)\ln(\tau/\tau_*),\qquad
\delta_R\simeq C(\mathbf k)\cos(k\tau/\sqrt3)+D(\mathbf k)\sin(k\tau/\sqrt3).}
$$

An additive constant in $\delta_C$ is absorbed into the reference $\tau_*$; the regular adiabatic solution fixes the acoustic phase, with $D=0$ in the explicit time-origin convention above. A general acoustic mixture has both terms. The physical expansion parameter is $k\tau/\sqrt3$; comparisons with $2\pi/k$ describe the same long- and short-wavelength regimes up to fixed numerical factors.

The contrast grows much more slowly after entry during [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination): [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology) undergoes pressure-supported acoustic oscillations and cold matter only the logarithmic [Mészáros effect](../../../linear-cosmological-density-perturbation.md#meszaros-effect). Modes entering well before [matter-radiation equality](../../../cosmology.md#matter-radiation-equality) consequently have suppressed late amplitudes relative to modes that stay outside the horizon until near equality. After [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination) begins, pressureless growing modes can grow as $a$. This scale-dependent history produces the turnover and small-scale suppression of the matter transfer function and affects the initial conditions for [large-scale structure of the universe](../../../large-scale-structure-of-the-universe.md). The early subhorizon limit requires both $k\tau\gg1$ and $\tau\ll\tau_{\rm eq}$; it is not applicable to a mode that enters only in the [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $w=c_s^2$ be constant and small, and write $\theta=i\mathbf k\cdot\mathbf v$. The supplied [synchronous gauge](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) equations imply

$$
\delta'=-(1+w)(\theta+h'/2),\qquad
\theta'+(1-3w)\mathcal H\theta-\frac{w}{1+w}k^2\delta=0.
$$

Differentiating the first and eliminating $\theta$ gives

$$
\delta''+(1-3w)\mathcal H\delta'+wk^2\delta
=-\frac{1+w}2\left[h''+(1-3w)\mathcal Hh'\right].
$$

For the dominant single component, the Einstein equation gives $h''+\mathcal Hh'=-3\mathcal H^2(1+3w)\delta$. Therefore the exact algebraic intermediate relation is

$$
\delta''+(1-3w)\mathcal H\delta'
+\left[wk^2-\frac32(1+w)(1+3w)\mathcal H^2\right]\delta
=\frac32w(1+w)\mathcal Hh'.
$$

The requested [nonrelativistic density equation in synchronous gauge](../../../linear-cosmological-density-perturbation.md#nonrelativistic-density-equation-in-synchronous-gauge) follows to leading nonrelativistic order: discard [pressure](../../../thermodynamics.md#pressure) corrections to the background, Hubble damping, and [metric tensor](../../../general-relativity.md#metric-tensor) terms while retaining $c_s^2k^2\delta$, which can be comparable to gravity at the [Jeans wavenumber](../../../linear-cosmological-density-perturbation.md#jeans-wavenumber). Since $w\ll1$, that scale lies well inside the [Hubble radius](../../../cosmology.md#hubble-radius), so keeping its enhanced gradient term is consistent. The resulting equation is

$$
\delta''+\mathcal H\delta'+(c_s^2k^2-4\pi Ga^2\bar\rho_m)\delta=0,
$$

where the [Friedmann equation](../../../cosmology.md#friedmann-equations) gave $3\mathcal H^2/2=4\pi Ga^2\bar\rho_m$. Now $\delta'=a\dot\delta$ and $\delta''=a^2(\ddot\delta+H\dot\delta)$, so

$$
\boxed{\ddot\delta+2H\dot\delta-
\left(4\pi G\bar\rho_m-\frac{c_s^2k^2}{a^2}\right)\delta=0.}
$$

This is the specified approximation, not an exact finite-$w$ relativistic identity. The pressure-gradient term stabilizes short wavelengths, while gravity drives the long-wavelength [Jeans instability](../../../linear-cosmological-density-perturbation.md#jeans-instability).

Now apply the stipulated equation to $P=K\rho^{4/3}$ with $K>0$. In the pressure-negligible matter background,

$$
a\propto t^{2/3},\qquad \bar\rho_m=\frac1{6\pi Gt^2},\qquad
c_s^2=\frac43K\bar\rho_m^{1/3}\propto t^{-2/3}\propto a^{-1}.
$$

Thus $c_s^2k^2/a^2$ is proportional to $t^{-2}$, exactly like the gravitational term. Define

$$
k_J^2=\frac{4\pi G\bar\rho_m a^2}{c_s^2},\qquad
q=\frac{k^2}{k_J^2}.
$$

The comoving [Jeans wavenumber](../../../linear-cosmological-density-perturbation.md#jeans-wavenumber) and $q$ are constant in this era. The equation becomes the [Euler-Cauchy equation](../../../differential-equation.md#euler-cauchy-equation)

$$
\ddot\delta+\frac4{3t}\dot\delta+\frac{2(q-1)}{3t^2}\delta=0.
$$

Setting $\delta\propto t^p$ gives $p^2+p/3+2(q-1)/3=0$. For distinct real roots the full pair of modes is

$$
\boxed{\delta(t)=A\left(\frac t{t_*}\right)^{p_+}
+B\left(\frac t{t_*}\right)^{p_-},\qquad
p_\pm=\frac{-1\pm\sqrt{25-24q}}6.}
$$

These are the [Jeans modes of a four-thirds polytropic cosmological fluid](../../../linear-cosmological-density-perturbation.md#jeans-modes-of-a-four-thirds-polytropic-cosmological-fluid). The physical [Jeans length](../../../linear-cosmological-density-perturbation.md#jeans-length) is

$$
\boxed{\lambda_J=\frac{2\pi a}{k_J}
=c_s\sqrt{\frac\pi{G\bar\rho_m}},\qquad
q=\left(\frac{\lambda_J}{\lambda}\right)^2,
\quad\lambda=\frac{2\pi a}{k}.}
$$

Here $\lambda_J\propto a$, so its comoving value is constant. For $\lambda>\lambda_J$, $q<1$ and $p_+>0$, giving genuine growth; the other solution decays. In the long-wavelength pressure-free limit, $p_+=2/3$ and $p_-=-1$, the familiar matter-era modes. At $\lambda=\lambda_J$, the two powers are $0$ and $-1/3$, so the leading mode is constant rather than growing.

For $1<q<25/24$ both powers are negative: [pressure](../../../thermodynamics.md#pressure) prevents growth, although the modes still decay without oscillation. At $q=25/24$ they coincide and the complete solution is

$$
\delta=t^{-1/6}\left[A+B\ln(t/t_*)\right].
$$

For $q>25/24$ they become a complex-conjugate pair; a real basis is

$$
\boxed{\delta=t^{-1/6}\left[A\cos\bigl(\omega\ln(t/t_*)\bigr)
+B\sin\bigl(\omega\ln(t/t_*)\bigr)\right],\qquad
\omega=\frac{\sqrt{24q-25}}6.}
$$

These short-wavelength acoustic oscillations have a decaying envelope. The onset of instability is $q=1$, while the threshold for oscillatory time dependence is slightly larger, $q=25/24$; expansion damping explains why these two thresholds are not identical.

## 3

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [comoving observer](../../../cosmology.md#comoving-observer) measures $E=ap^0$, so $q=aE=a^2p^0$. Write $\mathcal H=a'/a$. The [null geodesic](../../../special-relativity.md#null-geodesic) condition implies

$$
(\delta_{ij}+h_{ij})p^ip^j=(p^0)^2.
$$

The time component of the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation), using $d\tau/d\lambda=p^0$, is therefore

$$
\frac{dp^0}{d\tau}
=-\mathcal Hp^0-\frac{\mathcal H(\delta_{ij}+h_{ij})p^ip^j+\tfrac12h'_{ij}p^ip^j}{p^0}
=-2\mathcal Hp^0-\frac{h'_{ij}p^ip^j}{2p^0}.
$$

Differentiate $q=a^2p^0$. The homogeneous expansion terms cancel:

$$
q'=2\mathcal Ha^2p^0+a^2\frac{dp^0}{d\tau}
=-\frac{a^2}{2p^0}h'_{ij}p^ip^j.
$$

At zeroth order $p^i/p^0=n^i$, with $\delta_{ij}n^in^j=1$. The difference between coordinate [velocity](../../../classical-mechanics.md#velocity) and physical unit direction is already first order and multiplies $h'$, so it can be discarded in this expression. We obtain the [synchronous photon momentum redshift](../../../cosmic-microwave-background-anisotropy.md#synchronous-photon-momentum-redshift)

$$
\boxed{\frac{dq}{d\tau}=-\frac12q h'_{ij}n^in^j.}
$$

In the unperturbed universe $q$ is constant and physical [photon](../../../quantum-mechanics.md#photon) energy redshifts as $a^{-1}$; the displayed term is the additional anisotropic first-order redshift.

To check the direction, let $v^i=p^i/p^0$. Combining the spatial and temporal [geodesic equations](../../../riemannian-geometry.md#geodesic-equation) cancels their homogeneous Hubble terms and gives

$$
\frac{dv^i}{d\tau}
=-h'^i{}_jv^j-\Gamma^i{}_{jk}v^jv^k
+\frac12v^i h'_{jk}v^jv^k=O(h).
$$

Every remaining connection or explicit metric-derivative term is first order. A local orthonormal spatial frame defines the physical unit vector by $n^i=v^i+\tfrac12h^i{}_jv^j+O(h^2)$. Its derivative adds only first-order terms, so

$$
\boxed{\frac{dn^i}{d\tau}=O(h).}
$$

Consequently direction deflection multiplied by an already first-order [temperature](../../../thermodynamics.md#temperature) anisotropy is second order. The first-order brightness calculation may use a straight unperturbed ray without neglecting the first-order gravitational frequency change.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Before decoupling, rapid [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) makes the [photon](../../../quantum-mechanics.md#photon) distribution nearly isotropic in the local photon-fluid rest frame. A local blackbody [temperature](../../../thermodynamics.md#temperature) perturbation changes its [energy density](../../../statistical-physics.md#energy-density) by $\delta_\gamma=4\delta T/T$. A first-order boost by the fluid [velocity](../../../classical-mechanics.md#velocity) adds a [temperature](../../../thermodynamics.md#temperature) [photon dipole](../../../cosmic-microwave-background-anisotropy.md#photon-dipole) $\mathbf n\cdot\mathbf v$; it does not generate a [photon quadrupole](../../../cosmic-microwave-background-anisotropy.md#photon-quadrupole) until second order in that boost. Thus the [photon brightness perturbation](../../../cosmic-microwave-background-anisotropy.md#photon-brightness-perturbation) at instantaneous decoupling is

$$
\Delta_* =\delta_{\gamma *}+4\mathbf n\cdot\mathbf v_*.
$$

Higher angular moments are suppressed by the [photon](../../../quantum-mechanics.md#photon) mean-free-path to perturbation-length ratio in the [tight-coupling approximation](../../../cosmic-microwave-background-anisotropy.md#tight-coupling-approximation). The idealized equilibrium assumption neglects those finite-mean-free-path corrections, polarization effects and finite thickness of the last-scattering surface. It is not an assertion that collisionless [photons](../../../quantum-mechanics.md#photon) remain isotropic after decoupling. The distinction between a fluid treatment and the subsequent hierarchy is discussed in [the primary synchronous and Newtonian perturbation treatment](https://arxiv.org/abs/astro-ph/9506072).

Let $\mu=\hat{\mathbf k}\cdot\mathbf n$ and $W(\tau)=e^{ik\mu(\tau-\tau_0)}$. Multiplication of the [synchronous photon brightness equation](../../../cosmic-microwave-background-anisotropy.md#synchronous-photon-brightness-equation) by its [integrating factor](../../../differential-equation.md#integrating-factor) gives

$$
\left(e^{ik\mu\tau}\Delta\right)'
=-2e^{ik\mu\tau}h'_{ij}n^in^j.
$$

Integration from $\tau_*=\tau_{\rm dec}$ to $\tau_0$ and division by four yield

$$
\boxed{\Theta(\mathbf k,\mu,\tau_0)
=\left(\frac{\delta_{\gamma *}}4+\mathbf n\cdot\mathbf v_*\right)
 e^{-ik\mu(\tau_0-\tau_*)}
-\frac12\int_{\tau_*}^{\tau_0}W(\tau)h'_{ij}n^in^j\,d\tau,
\qquad\Theta=\frac{\Delta T}{T}.}
$$

For the real-space observation point $\mathbf x_0$, the corresponding background ray is $\mathbf x(\tau)=\mathbf x_0-\mathbf n(\tau_0-\tau)$. Fourier inversion gives the [synchronous Sachs-Wolfe line-of-sight formula](../../../cosmic-microwave-background-anisotropy.md#synchronous-sachs-wolfe-line-of-sight-formula)

$$
\boxed{\Theta(\mathbf x_0,\mathbf n,\tau_0)
=\frac14\delta_\gamma(\mathbf x_*,\tau_*)
+\mathbf n\cdot\mathbf v(\mathbf x_*,\tau_*)
-\frac12\int_{\tau_*}^{\tau_0}
 h'_{ij}(\mathbf x(\tau),\tau)n^in^j\,d\tau,
\quad\mathbf x_*=\mathbf x(\tau_*).}
$$

Every source is evaluated at its appropriate point on the ray, rather than at the observation position. Here $\mathbf n$ is [photon](../../../quantum-mechanics.md#photon) propagation direction, opposite to the outward observer-to-source sky direction; changing that convention changes the written sign of the Doppler projection consistently.

The first term is the intrinsic [photon](../../../quantum-mechanics.md#photon) [temperature](../../../thermodynamics.md#temperature) at last scattering. On wavelengths larger than the [sound horizon](../../../cosmic-microwave-background-anisotropy.md#sound-horizon), it retains primordial adiabatic information; inside that horizon the [photon-baryon fluid](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-fluid) has acoustic [energy density](../../../statistical-physics.md#energy-density) oscillations, producing the acoustic [temperature](../../../thermodynamics.md#temperature) peaks. The second term is the [Doppler effect](../../../physics.md#doppler-effect) from the fluid's bulk motion at emission. A regular long-wavelength [velocity](../../../classical-mechanics.md#velocity) is gradient-suppressed; the Doppler contribution is important near and below the acoustic horizon, with its acoustic phase displaced from that of the [energy density](../../../statistical-physics.md#energy-density) oscillation.

The integral is the gravitational energy shift produced by the changing spatial [metric tensor](../../../general-relativity.md#metric-tensor) along the [photon](../../../quantum-mechanics.md#photon) path. In [synchronous gauge](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) it includes endpoint gravitational redshifts as well as evolving-potential effects. It must not be identified solely with the [Integrated Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#integrated-sachs-wolfe-effect): in [Newtonian gauge](../../../linear-cosmological-perturbation-theory.md#newtonian-gauge) the same total separates into the ordinary last-scattering [Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-effect), local observer terms, and an integral of time-varying potentials. The ordinary contribution is important on scales outside the [sound horizon](../../../cosmic-microwave-background-anisotropy.md#sound-horizon) at decoupling. A late integrated contribution is strongest on large angular scales when dark energy or curvature changes the potentials; evolution around [matter-radiation equality](../../../cosmology.md#matter-radiation-equality) also contributes near the first acoustic scales.

The relevant comoving sound scale is $r_s(\tau_*)=\int^{\tau_*}c_s(\tau)d\tau$, while the projection distance is $D_*\simeq\tau_0-\tau_*$. Modes project roughly to [photon temperature multipole](../../../cosmic-microwave-background-anisotropy.md#photon-temperature-multipole) $\ell\sim kD_*$, and the acoustic scale is $\ell\sim D_*/r_s$, with successive peak spacing of order $\pi D_*/r_s$. At much shorter wavelengths [Silk damping](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-diffusion-damping) and the finite last-scattering thickness suppress [energy density](../../../statistical-physics.md#energy-density) and [velocity](../../../classical-mechanics.md#velocity) anisotropies; the instantaneous-decoupling approximation alone does not model that cutoff. These scale distinctions explain why the three terms cannot be assigned one common range of important wavelengths.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Use the exact scalar-metric normalization specified by the preceding brightness equation:

$$
h_{ij}n^in^j=\frac h3+\left(\mu^2-\frac13\right)h_s.
$$

The [temperature](../../../thermodynamics.md#temperature) source is therefore $-(h'-h_s')/6-\mu^2h_s'/2$. Let $W=e^{ik\mu(\tau-\tau_0)}$, so $W'=ik\mu W$ and $W''=-k^2\mu^2W$. The formula just derived becomes

$$
\Theta_0=W_*\left(\frac{\delta_\gamma}4+\mathbf n\cdot\mathbf v\right)_*
-\int_{\tau_*}^{\tau_0}W\frac{h'-h_s'}6\,d\tau
-\frac{\mu^2}2\int_{\tau_*}^{\tau_0}Wh_s'\,d\tau.
$$

For $k\ne0$ the last term may be integrated twice by parts:

$$
\begin{aligned}
-\frac{\mu^2}2\int Wh_s'd\tau
&=\frac1{2k^2}\int W''h_s'd\tau\\
&=\frac1{2k^2}\left[W'h_s'-Wh_s''\right]_{\tau_*}^{\tau_0}
+\frac1{2k^2}\int Wh_s'''d\tau.
\end{aligned}
$$

No field equation beyond the supplied brightness relation has been used for this identity.

For scalar [velocity](../../../classical-mechanics.md#velocity) the supplied [photon continuity equation](../../../cosmic-microwave-background-anisotropy.md#photon-continuity-equation) gives

$$
i\mathbf k\cdot\mathbf v=-\frac34\delta_\gamma'-\frac12h',
\qquad
\mathbf n\cdot\mathbf v=\frac{3i\mu}{4k}\delta_\gamma'
+\frac{i\mu}{2k}h'.
$$

The sign follows from division by $i$: with the Fourier streaming term $+ik\mu$, the [velocity](../../../classical-mechanics.md#velocity) projection has the plus $h'$ term shown here. Combining it with the lower endpoint from the integrations by parts gives the complete [endpoint terms in the synchronous Sachs-Wolfe formula](../../../cosmic-microwave-background-anisotropy.md#endpoint-terms-in-the-synchronous-sachs-wolfe-formula):

$$
\boxed{\begin{aligned}
\Theta_0={}&W_*\left[
\frac14\delta_\gamma+\frac{3i\mu}{4k}\delta_\gamma'
+\frac{i\mu}{2k}(h'-h_s')+\frac{h_s''}{2k^2}\right]_*\\
&+\left[\frac{i\mu}{2k}h_s'-\frac{h_s''}{2k^2}\right]_0\\
&-\int_{\tau_*}^{\tau_0}W(\tau)
\left[\frac{h'-h_s'}6-\frac{h_s'''}{2k^2}\right]d\tau.
\end{aligned}}
$$

The local observer bracket is an angular [photon monopole](../../../cosmic-microwave-background-anisotropy.md#photon-monopole) plus [photon dipole](../../../cosmic-microwave-background-anisotropy.md#photon-dipole). Removing the local mean [temperature](../../../thermodynamics.md#temperature) and [photon dipole](../../../cosmic-microwave-background-anisotropy.md#photon-dipole), or restricting the result to measured multipoles $\ell\geq2$, permits omitting that bracket. It must be retained for the literal full brightness amplitude. The $k=0$ limit should be taken in the original line-of-sight integral, rather than treating the separate inverse-$k$ endpoint terms as independently defined.

**The final target formula printed in the PDF does not follow from its preceding equations.** With the stated streaming and scalar conventions, the decoupling terms proportional to $h'-h_s'$ and $h_s''$ have plus signs as derived above, not the printed minus signs. Moreover the integral has no additional outside factor $1/2$ when its bracket is $(h'-h_s')/6-h_s'''/(2k^2)$. Equivalently one may retain an outside $-1/2$ only if that bracket is doubled to $(h'-h_s')/3-h_s'''/k^2$. Omitting the observer [photon monopole](../../../cosmic-microwave-background-anisotropy.md#photon-monopole) and [photon dipole](../../../cosmic-microwave-background-anisotropy.md#photon-dipole) does not fix these discrepancies.

For a direct counterexample to the integral coefficient, take $h_s=0$, $h'=\varepsilon$ constant, $\mu=0$, and $\delta_{\gamma *}=\delta_{\gamma *}'=0$. A scalar emission [velocity](../../../classical-mechanics.md#velocity) with $i\mathbf k\cdot\mathbf v_*=-\varepsilon/2$ satisfies the stated continuity equation; its projection along this transverse [photon](../../../quantum-mechanics.md#photon) direction is zero. Keep $\varepsilon(\tau_0-\tau_*)\ll1$ so [perturbation theory](../../../analysis.md#perturbation-theory) is valid. The original brightness equation or the line-of-sight integral gives

$$
\Theta_0=-\frac{\varepsilon(\tau_0-\tau_*)}{6},
$$

whereas the printed final expression gives $-\varepsilon(\tau_0-\tau_*)/12$. All $h_s$ observer terms vanish in this example, so an observer-term convention cannot remove the contradiction. The boxed corrected identity supplies the requested integration-by-parts result with every boundary contribution and its observable higher-multipole version specified.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
