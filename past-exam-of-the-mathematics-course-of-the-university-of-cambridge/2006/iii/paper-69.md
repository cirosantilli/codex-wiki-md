# Paper 69

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper69.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper69.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

[Statistical homogeneity](../../../probability-and-statistics.md#statistical-homogeneity) makes the two-point [correlation](../../../variance.md#pearson-correlation-coefficient) depend on the displacement $\mathbf u=\mathbf r-\mathbf r'$. Substituting the [Fourier transforms](../../../analysis.md#fourier-transform) and changing variables from $(\mathbf r,\mathbf r')$ to $(\mathbf u,\mathbf r')$ gives

$$
\begin{aligned}
\mathbb E[\widehat B_i(\mathbf k)\widehat B_j(\mathbf k')]
&=\int d^3u\,d^3r'\,C_{ij}(\mathbf u)e^{-i\mathbf k\cdot\mathbf u}e^{-i(\mathbf k+\mathbf k')\cdot\mathbf r'}\\
&=\widehat C_{ij}(\mathbf k)\int d^3r'\,e^{-i(\mathbf k+\mathbf k')\cdot\mathbf r'}.
\end{aligned}
$$

The last [integral](../../../calculus.md#integral) is a [Dirac delta function](../../../distribution-theory.md#dirac-delta-function), so

$$
\boxed{\mathbb E[\widehat B_i(\mathbf k)\widehat B_j(\mathbf k')]=(2\pi)^3\delta(\mathbf k+\mathbf k')\widehat C_{ij}(\mathbf k).}
$$

The plus sign occurs because neither [Fourier transform](../../../analysis.md#fourier-transform) has undergone [complex conjugation](../../../complex-analysis.md#complex-conjugation). For a real [magnetic field](../../../electromagnetism.md#magnetic-field), the version with $\widehat B_j(\mathbf k')^*$ instead has $\delta(\mathbf k-\mathbf k')$. Homogeneity determines dependence on the displacement vector; dependence only on its [norm](../../../functional-analysis.md#norm) needs [statistical isotropy](../../../probability-and-statistics.md#statistical-isotropy) as well.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

[Statistical isotropy](../../../probability-and-statistics.md#statistical-isotropy) and [statistical reflection symmetry](../../../probability-and-statistics.md#statistical-reflection-symmetry) allow the [spectral tensor](../../../probability-and-statistics.md#spectral-tensor) to contain only $\delta_{ij}$ and $k_i k_j$:

$$
\widehat C_{ij}(\mathbf k)=A(k)\delta_{ij}+D(k)k_i k_j.
$$

The [solenoidal magnetic-field constraint](../../../electromagnetism.md#solenoidal-magnetic-field-constraint) is essential here. Taking its [Fourier transform](../../../analysis.md#fourier-transform) gives $k_i\widehat B_i=0$, hence $k_i\widehat C_{ij}=0$ and $A+Dk^2=0$. Thus the [spectral tensor](../../../probability-and-statistics.md#spectral-tensor) is a scalar multiple of the [transverse projector of a vector field](../../../relativistic-quantum-field.md#transverse-projector-of-a-vector-field). Its [trace](../../../linear-algebra.md#matrix-trace) is $2A$, so the prescribed normalization gives

$$
\boxed{\widehat C_{ij}(\mathbf k)=H(k)\left(\delta_{ij}-\frac{k_i k_j}{k^2}\right),\qquad k\ne0.}
$$

This is the [solenoidal isotropic spectral tensor](../../../probability-and-statistics.md#solenoidal-isotropic-spectral-tensor). Without the [solenoidal](../../../calculus.md#solenoidal-vector-field) condition, isotropy and reflection symmetry would leave two scalar functions. Without reflection symmetry, an antisymmetric term proportional to $i\epsilon_{ijm}k_m$ could additionally encode [magnetic helicity](../../../electromagnetism.md#magnetic-helicity).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write the transverse displacement as $\mathbf s$ and take the common line-of-sight interval to be $[0,L]$. The [rotation measure](../../../electromagnetism.md#rotation-measure) is a line integral of the [magnetic field](../../../electromagnetism.md#magnetic-field), so its [correlation](../../../variance.md#pearson-correlation-coefficient) is

$$
C_{\mathrm{RM}}(\mathbf s)=a_0^2n_e^2\int_0^L dz\int_0^L dz'\,C_{zz}(\mathbf s,z-z').
$$

Substitute the [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) of the [solenoidal isotropic spectral tensor](../../../probability-and-statistics.md#solenoidal-isotropic-spectral-tensor). Keeping the finite observation length gives the exact windowed expression

$$
C_{\mathrm{RM}}(\mathbf s)=a_0^2n_e^2\int\frac{d^3k}{(2\pi)^3}H(k)\left(1-\frac{k_z^2}{k^2}\right)e^{i\mathbf k_\perp\cdot\mathbf s}\left|\int_0^L e^{ik_z z}\,dz\right|^2.
$$

The allowed extension of the longitudinal displacement integral to the whole real line is the [long-path projection of a magnetic correlation](../../../electromagnetism.md#long-path-projection-of-a-magnetic-correlation). It applies when $L$ is much larger than the [correlation length](../../../critical-phenomenon.md#correlation-length): equivalently, the squared window becomes $2\pi L\delta(k_z)$ inside the [integral](../../../calculus.md#integral). The [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) sets $k_z=0$, leaving

$$
\boxed{C_{\mathrm{RM}}(s)\simeq a_0^2n_e^2L\int\frac{d^2k_\perp}{(2\pi)^2}H(k_\perp)e^{i\mathbf k_\perp\cdot\mathbf s}.}
$$

[Statistical isotropy](../../../probability-and-statistics.md#statistical-isotropy) makes this a function of $s=|\mathbf s|$. The displayed two-dimensional relation is the intended long-path approximation; the preceding windowed formula accounts for finite-length edge effects.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Invert the two-dimensional [Fourier transform](../../../analysis.md#fourier-transform) from part (c):

$$
H(k)=\frac1{a_0^2n_e^2L}\int_{\mathbb R^2}C_{\mathrm{RM}}(s)e^{-i\mathbf k_\perp\cdot\mathbf s}\,d^2s.
$$

In [polar coordinates](../../../calculus.md#polar-coordinates), the angular integral is $2\pi J_0(ks)$, where $J_0$ is a [Bessel function of the first kind](../../../analysis.md#bessel-function-of-the-first-kind). The [Fourier-Hankel normalization for an isotropic spectrum](../../../analysis.md#fourier-hankel-normalization-for-an-isotropic-spectrum) therefore yields

$$
\boxed{H(k)=\frac{2\pi}{a_0^2n_e^2L}\int_0^\infty s\,J_0(ks)C_{\mathrm{RM}}(s)\,ds.}
$$

This [Hankel inversion of a rotation-measure correlation](../../../electromagnetism.md#hankel-inversion-of-a-rotation-measure-correlation) recovers the scalar [spectral tensor](../../../probability-and-statistics.md#spectral-tensor) coefficient. To obtain the shell-integrated [magnetic energy spectrum](../../../electromagnetism.md#magnetic-energy-spectrum), take the [trace](../../../linear-algebra.md#matrix-trace) of the three-dimensional tensor:

$$
\mathbb E|\mathbf B|^2=\int\frac{d^3k}{(2\pi)^3}\,2H(k)=\frac1{\pi^2}\int_0^\infty k^2H(k)\,dk.
$$

With [magnetic energy](../../../electromagnetism.md#magnetic-energy) density $B^2/(8\pi)$ in [Gaussian units](../../../electromagnetism.md#gaussian-units), the one-dimensional convention $\int_0^\infty E_B(k)\,dk=\mathbb E|\mathbf B|^2/(8\pi)$ gives $\boxed{E_B(k)=k^2H(k)/(8\pi^3)}$. A spectrum normalized instead to $\mathbb E|\mathbf B|^2/2$ has coefficient $k^2H(k)/(2\pi^2)$; the physical normalization must be stated.

## 2

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Put $a=c/(4\pi en)$ and retain terms linear in $\delta\mathbf B$. The [electron magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#electron-magnetohydrodynamics) induction equation becomes

$$
\partial_t\delta\mathbf B=-aB_0\partial_z(\nabla\times\delta\mathbf B).
$$

Here the [curl](../../../calculus.md#curl) of $(\nabla\times\delta\mathbf B)\times B_0\hat{\mathbf z}$ reduces to $B_0\partial_z\nabla\times\delta\mathbf B$, since the background [magnetic field](../../../electromagnetism.md#magnetic-field) is constant and the [divergence](../../../calculus.md#divergence) of a curl vanishes. For a [plane wave](../../../quantum-mechanics.md#plane-wave) $\delta\mathbf B=\mathbf b\,e^{i(\mathbf k\cdot\mathbf r-\omega t)}$, the linear equation and the [solenoidal](../../../calculus.md#solenoidal-vector-field) constraint are

$$
\omega\mathbf b=i aB_0k_\parallel\,\mathbf k\times\mathbf b,\qquad \mathbf k\cdot\mathbf b=0.
$$

On the transverse plane, the operator $i\mathbf k\times$ has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\pm k$ by the [helicity decomposition of a transverse Fourier mode](../../../special-relativity.md#helicity-decomposition-of-a-transverse-fourier-mode). Equivalently, squaring the equation and using the [vector triple product](../../../calculus.md#vector-triple-product) gives $\omega^2=a^2B_0^2k_\parallel^2k^2$. Since $aB_0=v_Ad_i$, where $v_A$ is the [Alfvén speed](../../../astrophysical-fluid-dynamics.md#alfven-speed) and $d_i$ the [ion skin depth](../../../physics.md#ion-skin-depth),

$$
\boxed{\omega_\pm(\mathbf k)=\pm v_Ad_i k_\parallel k.}
$$

The two branches have opposite [circular polarizations](../../../electromagnetism.md#circular-polarization). The specified electron-only induction model describes a [whistler wave](../../../astrophysical-fluid-dynamics.md#whistler-wave); the paper calls these branches [kinetic Alfvén waves](../../../astrophysical-fluid-dynamics.md#kinetic-alfven-wave). The following cascade calculation uses the specified model and its [dispersion relation](../../../wave-equation.md#dispersion-relation), without adding the pressure response needed for the usual kinetic Alfvén interpretation.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $b_l=\delta B_l/B_0$. The nonlinear term has two perpendicular spatial [derivatives](../../../calculus.md#derivative), so its rate relative to the fluctuation amplitude is

$$
\tau_{\mathrm{nl}}^{-1}\sim\frac{v_Ad_i b_l}{l_\perp^2},\qquad \tau_{\mathrm{nl}}\sim\frac{l_\perp^2}{v_Ad_i b_l}.
$$

The [wave period](../../../physics.md#wave-period) from part (a), using $k\sim k_\perp$, is $\tau_w\sim l_\parallel l_\perp/(v_Ad_i)$. A [weak wave cascade](../../../turbulence.md#weak-wave-cascade) requires that one interaction change a packet only slightly:

$$
\chi=\frac{\tau_w}{\tau_{\mathrm{nl}}}\sim b_l\frac{l_\parallel}{l_\perp}\ll1.
$$

For interactions with decorrelated phases, successive fractional changes accumulate as a [random walk](../../../markov-process.md#random-walk). An order-one change needs $N\chi^2\sim1$, giving

$$
\boxed{\tau_l\sim N\tau_w\sim\frac{\tau_{\mathrm{nl}}^2}{\tau_w}=\frac{l_\perp^3}{v_Ad_i b_l^2l_\parallel}.}
$$

Constant [energy flux](../../../physics.md#energy-flux) per unit mass then gives $\epsilon\sim v_A^2b_l^2/\tau_l\sim v_A^3d_i b_l^4l_\parallel/l_\perp^3$, hence

$$
\boxed{\frac{\delta B_l}{B_0}\sim\left(\frac{\epsilon l_\perp^3}{v_A^3d_i l_\parallel}\right)^{1/4}.}
$$

The [weak electron-magnetohydrodynamic cascade](../../../turbulence.md#weak-electron-magnetohydrodynamic-cascade) scaling uses both locality in scale and the decorrelation assumption; a small amplitude by itself does not specify the cascade time.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For an isotropic [weak electron-magnetohydrodynamic cascade](../../../turbulence.md#weak-electron-magnetohydrodynamic-cascade), set $l_\parallel\sim l_\perp\sim l$. Part (b) gives $\delta B_l\propto l^{1/2}$. With the one-dimensional shell convention for the [magnetic energy spectrum](../../../electromagnetism.md#magnetic-energy-spectrum), fluctuations on scale $l\sim k^{-1}$ satisfy $\delta B_l^2\sim kE_B(k)$ up to normalization constants. Therefore

$$
\boxed{E_B(k)\propto k^{-2}.}
$$

This is the shell-integrated spectrum. The three-dimensional [spectral tensor](../../../probability-and-statistics.md#spectral-tensor) coefficient has two additional powers of $k^{-1}$ and scales as $H(k)\propto k^{-4}$. These exponents apply within the assumed local, weak cascade range.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

[Critical balance](../../../turbulence.md#critical-balance) makes the nonlinear interaction time comparable to the [wave period](../../../physics.md#wave-period):

$$
\frac{l_\perp^2}{v_Ad_i b_l}\sim\frac{l_\parallel l_\perp}{v_Ad_i},\qquad l_\parallel\sim\frac{l_\perp}{b_l}.
$$

An order-one interaction transfers energy in $\tau_l\sim\tau_{\mathrm{nl}}$, so constant [energy flux](../../../physics.md#energy-flux) gives $\epsilon\sim v_A^3d_i b_l^3/l_\perp^2$. Thus the [critically balanced electron-magnetohydrodynamic cascade](../../../turbulence.md#critically-balanced-electron-magnetohydrodynamic-cascade) has

$$
\boxed{\frac{\delta B_l}{B_0}\sim\left(\frac{\epsilon}{v_A^3d_i}\right)^{1/3}l_\perp^{2/3},\qquad l_\parallel\sim\left(\frac{v_A^3d_i}{\epsilon}\right)^{1/3}l_\perp^{1/3}.}
$$

For the corresponding perpendicular [magnetic energy spectrum](../../../electromagnetism.md#magnetic-energy-spectrum), $\delta B_l^2\sim k_\perp E_B(k_\perp)$ gives $E_B(k_\perp)\propto k_\perp^{-7/3}$. The increasing ratio $l_\parallel/l_\perp\propto l_\perp^{-2/3}$ describes progressively more anisotropic fluctuations at smaller perpendicular scales, within the range in which the model and [critical balance](../../../turbulence.md#critical-balance) assumptions hold.

## 3

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The strain is an [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process). Multiplying its equation by the [integrating factor](../../../differential-equation.md#integrating-factor) $e^{t/\tau}$ and using the zero initial condition gives

$$
\widetilde\sigma(t)=\int_0^t e^{-(t-s)/\tau}f(s)\,ds=\sqrt\kappa\int_0^t e^{-(t-s)/\tau}\,dW_s.
$$

The second expression is a [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) against [Brownian motion](../../../brownian-motion.md). A deterministic linear functional of [Gaussian white noise](../../../stochastic-process.md#gaussian-white-noise) is [Gaussian](../../../probability-theory.md#normal-distribution), and its [expected value](../../../probability-theory.md#expected-value) is zero. For $t\ge t'$, the noise [covariance](../../../variance.md#covariance) gives

$$
\begin{aligned}
\mathbb E[\widetilde\sigma(t)\widetilde\sigma(t')]
&=\kappa\int_0^{t'}e^{-(t-s)/\tau}e^{-(t'-s)/\tau}\,ds\\
&=\frac{\kappa\tau}{2}\left[e^{-(t-t')/\tau}-e^{-(t+t')/\tau}\right].
\end{aligned}
$$

For $t'\gg\tau$, the initial-condition term is negligible. The stationary [autocorrelation](../../../time-series.md#autocorrelation) is therefore

$$
\boxed{\mathbb E[\widetilde\sigma(t)\widetilde\sigma(t')]\simeq\frac{\kappa\tau}{2}e^{-|t-t'|/\tau}.}
$$

Its normalized exponential decay has [correlation time](../../../time-series.md#correlation-time) $\tau$. The [zero-start Ornstein-Uhlenbeck covariance](../../../stochastic-process.md#zero-start-ornstein-uhlenbeck-covariance) also shows how stationarity is approached.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Differentiate the product of [Dirac delta functions](../../../distribution-theory.md#dirac-delta-function) defining $\widetilde P$, regarding $B$ and $\sigma$ as independent density arguments. The random continuity equation is

$$
\partial_t\widetilde P=-\partial_B(\sigma B\widetilde P)+\frac1\tau\partial_\sigma(\sigma\widetilde P)-\partial_\sigma(f\widetilde P).
$$

For $0<s<t$, the causal [functional derivatives](../../../calculus-of-variations.md#functional-derivative) follow from the explicit strain solution and $\widetilde B(t)=B_0\exp[\int_0^t\widetilde\sigma(u)\,du]$:

$$
\frac{\delta\widetilde\sigma(t)}{\delta f(s)}=e^{-(t-s)/\tau},\qquad \frac{\delta\widetilde B(t)}{\delta f(s)}=\widetilde B(t)\tau\left[1-e^{-(t-s)/\tau}\right].
$$

Consequently,

$$
\frac{\delta\widetilde P(t)}{\delta f(s)}=-e^{-(t-s)/\tau}\partial_\sigma\widetilde P-\tau\left[1-e^{-(t-s)/\tau}\right]\partial_B(\widetilde B(t)\widetilde P).
$$

In the [Furutsu–Novikov formula](../../../stochastic-process.md#novikov-s-theorem), the covariance $\kappa\delta(t-s)$ samples the upper endpoint of the causal time integral. Symmetric regularization of the [white noise](../../../time-series.md#white-noise) gives half the mass there. The $B$ response vanishes as $s\uparrow t$, while the strain response tends to one, so $\mathbb E[f(t)\widetilde P(t)]=-(\kappa/2)\partial_\sigma P$. Averaging the continuity equation yields the [Fokker-Planck equation](../../../probability-theory.md#fokker-planck-equation)

$$
\boxed{\partial_tP=-\partial_B(\sigma BP)+\frac1\tau\partial_\sigma(\sigma P)+\frac\kappa2\partial_\sigma^2P.}
$$

There is no direct diffusion term in $B$: its equation contains the time integral of [colored noise](../../../stochastic-process.md#colored-noise), whereas the strain equation receives [Gaussian white noise](../../../stochastic-process.md#gaussian-white-noise). The same result follows from the [Itô diffusion](../../../stochastic-calculus.md#ito-diffusion) with drift $(\sigma B,-\sigma/\tau)$ and diffusion vector $(0,\sqrt\kappa)$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Multiply the [Fokker-Planck equation](../../../probability-theory.md#fokker-planck-equation) by $B^n$ and integrate over $B>0$ and all $\sigma$, assuming the required boundary terms vanish. [Integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\frac{d}{dt}\mathbb E[B^n]=n\mathbb E[\sigma B^n].
$$

The mixed [moment](../../../probability-theory.md#moment) is not determined by $\mathbb E[B^n]$: the current strain and the accumulated [magnetic field](../../../electromagnetism.md#magnetic-field) are correlated. Zero mean strain does not imply $\mathbb E[\sigma B^n]=0$, so this is an unclosed [moment equation](../../../mathematical-biology.md#moment-equation).

Keep the strain dependence by defining $P_n(\sigma,t)=\int_0^\infty B^nP(B,\sigma,t)\,dB$. The magnetic drift term satisfies

$$
-\int_0^\infty B^n\partial_B(\sigma BP)\,dB=n\sigma P_n.
$$

The strain derivatives commute with the $B$ integral. Hence

$$
\boxed{\partial_tP_n=\frac\kappa2\partial_\sigma^2P_n+\frac1\tau\partial_\sigma(\sigma P_n)+n\sigma P_n.}
$$

This weighted density obeys a tilted [Ornstein-Uhlenbeck Fokker-Planck equation](../../../probability-theory.md#ornstein-uhlenbeck-fokker-planck-equation). Its integral over $\sigma$ is the desired [moment](../../../probability-theory.md#moment), while retaining $\sigma$ makes the evolution closed.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For a separated weighted density, write $P_n=e^{\gamma t}p(\sigma)$. Its [eigenvalue equation](../../../linear-operator-theory.md#eigenvalue-equation) is

$$
\frac\kappa2p''+\frac1\tau(\sigma p)'+n\sigma p=\gamma p.
$$

Set $p=\psi\exp[-\sigma^2/(2\kappa\tau)]$. Differentiation eliminates the first derivative of $\psi$, giving the [tilted Ornstein-Uhlenbeck oscillator transformation](../../../stochastic-process.md#tilted-ornstein-uhlenbeck-oscillator-transformation)

$$
\frac\kappa2\psi''+\left[\frac1{2\tau}-\frac{\sigma^2}{2\kappa\tau^2}+n\sigma\right]\psi=\gamma\psi.
$$

Complete the square and introduce the [dimensionless variable](../../../mathematics.md#dimensionless-variable) $x=(\sigma-\kappa n\tau^2)/\sqrt{\kappa\tau}$. The equation becomes

$$
\frac{d^2\psi}{dx^2}+\left[1+\kappa n^2\tau^3-2\gamma\tau-x^2\right]\psi=0.
$$

Comparing with the [quantum harmonic oscillator](../../../quantum-mechanics.md#quantum-harmonic-oscillator) gives $2E=1+\kappa n^2\tau^3-2\gamma\tau$. Its energies $E_m=m+1/2$ therefore correspond to $\gamma_m=\kappa n^2\tau^2/2-m/\tau$. The dominant nonnegative separated mode is the [ground state](../../../quantum-mechanics.md#ground-state), which is [nodeless](../../../linear-operator-theory.md#nodeless-eigenfunction). Consequently

$$
\boxed{\gamma_n=\frac12\kappa\tau^2n^2.}
$$

For an independent check, $\log[\widetilde B(t)/B_0]=\int_0^t\widetilde\sigma(s)\,ds$ is a centered [Gaussian random variable](../../../probability-theory.md#gaussian-random-variable) with [variance](../../../variance.md)

$$
V(t)=\kappa\tau^2\left[t-2\tau(1-e^{-t/\tau})+\frac\tau2(1-e^{-2t/\tau})\right].
$$

The [exponential moment of a Gaussian linear functional](../../../stochastic-process.md#exponential-moment-of-a-gaussian-linear-functional) gives $\mathbb E[B^n]=B_0^n\exp[n^2V(t)/2]$, whose long-time growth rate is the same $\gamma_n$. This exact [Ornstein-Uhlenbeck multiplicative amplification](../../../stochastic-process.md#ornstein-uhlenbeck-multiplicative-amplification) formula also distinguishes the finite-time transient from the asymptotic exponential law. A general transient can contain sign-changing excited eigenfunctions in its expansion while the total weighted density remains nonnegative.

## 4

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Assume statistically steady, three-dimensional [turbulence](../../../turbulence.md) at large [Reynolds number](../../../fluid-mechanics.md#reynolds-number), with local [statistical homogeneity](../../../probability-and-statistics.md#statistical-homogeneity) and [statistical isotropy](../../../probability-and-statistics.md#statistical-isotropy) at scales small compared with the forcing scale $L$. The [Kolmogorov 1941 theory](../../../turbulence.md#kolmogorov-1941-theory) additionally assumes a local [energy cascade](../../../turbulence.md#energy-cascade), constant mean [energy flux](../../../physics.md#energy-flux) per unit mass $\epsilon$, and negligible [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) within the [inertial range](../../../turbulence.md#inertial-range). Its dimensional form neglects corrections from [internal intermittency](../../../turbulence.md#internal-intermittency).

At separation $l$, let $\delta u_l$ be a typical [velocity increment](../../../turbulence.md#velocity-increment). The [eddy turnover time](../../../turbulence.md#eddy-turnover-time) is $\tau_l\sim l/\delta u_l$. Constant transfer rate then gives $\epsilon\sim\delta u_l^2/\tau_l\sim\delta u_l^3/l$, hence

$$
\boxed{\delta u_l\sim(\epsilon l)^{1/3},\qquad E(k)=C_K\epsilon^{2/3}k^{-5/3}.}
$$

Here $E(k)$ is the one-dimensional [turbulent energy spectrum](../../../turbulence.md#turbulent-energy-spectrum), obtained from $\delta u_l^2\sim kE(k)$ with $k\sim l^{-1}$. The scaling holds only for

$$
\boxed{\eta\ll l\ll L,\qquad L^{-1}\ll k\ll\eta^{-1},\qquad \eta=(\nu^3/\epsilon)^{1/4}.}
$$

The [Kolmogorov length scale](../../../turbulence.md#kolmogorov-length-scale) follows by setting the scale-dependent [Reynolds number](../../../fluid-mechanics.md#reynolds-number) $\delta u_l l/\nu$ to one. The associated [Kolmogorov microscales](../../../turbulence.md#kolmogorov-microscales) give $\tau_\eta=(\nu/\epsilon)^{1/2}$. At larger scales the forcing matters; at smaller scales [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) matters.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Take a positive initial separation $0<l_0\ll\eta$. In the [dissipation range](../../../turbulence.md#dissipation-range), the [velocity field](../../../fluid-mechanics.md#velocity-field) is smooth, so the difference of the two [Lagrangian trajectories](../../../continuum-mechanics.md#lagrangian-trajectory) obeys the linearized separation equation $\dot{\boldsymbol l}\simeq(\nabla\mathbf u)\boldsymbol l$. Chaotic stretching gives a positive [Lyapunov exponent](../../../dynamical-systems.md#lyapunov-exponent) of order $\tau_\eta^{-1}$ and a typical separation

$$
l(t)\sim l_0e^{\lambda t},\qquad t_1\sim\lambda^{-1}\log(\eta/l_0).
$$

This needs a nonzero initial separation: exactly coincident particles remain coincident in a smooth flow.

Once $l$ lies in the [inertial range](../../../turbulence.md#inertial-range), the [Kolmogorov 1941 theory](../../../turbulence.md#kolmogorov-1941-theory) gives a relative speed of order $(\epsilon l)^{1/3}$. A scale-local typical-separation estimate $dl/dt\sim(\epsilon l)^{1/3}$ integrates to

$$
l(t)^{2/3}\sim\eta^{2/3}+C\epsilon^{1/3}(t-t_1).
$$

After loss of the entry-scale memory, the statistical [Richardson pair dispersion](../../../turbulence.md#richardson-pair-dispersion) law is $\mathbb E[l^2]\sim g_R\epsilon(t-t_1)^3$. Thus the characteristic separation grows as $(t-t_1)^{3/2}$ while $\eta\ll l\ll L$. This is a statistical scaling closure, rather than a deterministic equation for every pair.

For $l\gg L$, the particle velocities become approximately independent. If their [Lagrangian velocity autocorrelations](../../../turbulence.md#lagrangian-velocity-autocorrelation) have a finite [Lagrangian integral time](../../../turbulence.md#lagrangian-integral-time) $T_L\sim L/U$, the [diffusive large-scale pair dispersion](../../../turbulence.md#diffusive-large-scale-pair-dispersion) has effective relative [diffusivity](../../../brownian-motion.md#diffusion-coefficient) of order $UL$. After a further velocity-decorrelation transient,

$$
\mathbb E[l^2(t)]\sim L^2+C_DUL(t-t_2),\qquad l_{\mathrm{rms}}\propto(t-t_2)^{1/2}.
$$

This is the long-time mechanism of [Taylor turbulent dispersion](../../../turbulence.md#taylor-turbulent-dispersion) applied to the difference of two decorrelated trajectories. The [root mean square](../../../analysis.md#root-mean-square) separation eventually loses memory of the $L^2$ term.

Reaching $l=L$ at the end of the [inertial range](../../../turbulence.md#inertial-range) takes

$$
\boxed{t_2-t_1\sim\epsilon^{-1/3}\left(L^{2/3}-\eta^{2/3}\right)\sim\left(\frac{L^2}{\epsilon}\right)^{1/3}\sim\frac LU.}
$$

Order-one coefficients depend on the dispersion closure. The initial exponential stage can take a long time if $l_0$ is extremely small, but the inertial-range stage is of order one outer [eddy turnover time](../../../turbulence.md#eddy-turnover-time).

<a id="4/b/image-exponential-richardson-and-diffusive-regimes-of-turbulent-pair-separation"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69-pair-dispersion.png)

**[Figure 1](#4/b/image-exponential-richardson-and-diffusive-regimes-of-turbulent-pair-separation). Exponential, Richardson and diffusive regimes of turbulent pair separation**.

The [three-regime turbulent pair-separation model](../../../turbulence.md#three-regime-turbulent-pair-separation-model) in the sketch matches the regimes continuously for illustration. Its coefficients are schematic; the universal claims here are the scaling powers under the stated stretching, locality and decorrelation assumptions.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
