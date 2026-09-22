# Paper 79

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper79.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper79.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)

## 1

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Let $h=\sqrt{1-m^2}$ be the complementary modulus of the [complete elliptic integral of the first kind](../../../complex-analysis.md#complete-elliptic-integral-of-the-first-kind). With $\varphi=\pi/2-\theta$, write the integrand as $(\sin^2\varphi+h^2\cos^2\varphi)^{-1/2}$. Its [logarithmic endpoint asymptotic of the complete elliptic integral](../../../complex-analysis.md#logarithmic-endpoint-asymptotic-of-the-complete-elliptic-integral) comes from $\varphi=O(h)$; an expansion at fixed $\varphi$ alone misses the constant accompanying the logarithm.

Choose an intermediate cutoff $h\ll d\ll1$. In the endpoint region, the integral is

$$
\int_0^d\frac{d\varphi}{\sqrt{\varphi^2+h^2}}=\operatorname{arsinh}(d/h)=\log\frac{2d}{h}+o(1).
$$

Outside this region, the leading integral is

$$
\int_d^{\pi/2}\frac{d\varphi}{\sin\varphi}=-\log\tan(d/2)=\log\frac2d+o(1).
$$

The arbitrary cutoff cancels in this [matched asymptotic expansion](../../../differential-equation.md#matched-asymptotic-expansion), leaving

$$
\boxed{K(m)=\log\frac4{\sqrt{1-m^2}}+o(1)=-\frac12\log(1-m)+\log(2\sqrt2)+o(1).}
$$

These are the divergent logarithm and the finite constant, the requested first two terms. If terms are instead grouped by powers of the complementary modulus, the next refinement is $K(m)=\log(4/h)+(h^2/4)[\log(4/h)-1]+O(h^4\log(1/h))$; its coefficients agree with [the DLMF expansion](https://dlmf.nist.gov/19.12.E1).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

There are two contributing regions: an endpoint of width $x^{-1}$ near $u=0$, and a very narrow peak near $u=1$. Both must be retained in the [asymptotic expansion](../../../analysis.md#asymptotic-expansion).

For the peak, set $a=e^{-x}$ and $u=1+av$. At fixed $v$, $\log u\sim av$ and $e^{-xu}\sim a$, so the integrand times $du$ approaches $dv/(1+v^2)$. This is the [Lorentzian contribution from shrinking regularization](../../../analysis.md#lorentzian-contribution-from-shrinking-regularization). Its total contribution is

$$
\int_{-\infty}^{\infty}\frac{dv}{1+v^2}=\pi.
$$

For example, cut off this region at $|u-1|=e^{-x/2}$: its scaled endpoints tend to infinity, while the changes in the exponential and logarithm inside the peak are exponentially small. The matched tails outside it are also exponentially small compared with the endpoint terms below.

At the endpoint, put $v=xu$ and $L=\log x$. To algebraic orders in $L^{-1}$, the regularizing denominator term is negligible there, giving the [Laplace endpoint expansion with a logarithmic denominator](../../../analysis.md#laplace-endpoint-expansion-with-a-logarithmic-denominator)

$$
\frac1x\int_0^\infty\frac{e^{-v}}{(L-\log v)^2}\,dv\sim\frac1{xL^2}\left[1+\frac2L\int_0^\infty e^{-v}\log v\,dv+\cdots\right].
$$

This integral represents the endpoint expansion only; it is cut off before the original peak when making the argument precise. Since $\Gamma'(1)=-\gamma_E$, with $\gamma_E$ the [Euler--Mascheroni constant](../../../complex-analysis.md#euler-s-constant), the first two contributions to the original integral are

$$
\boxed{I(x)=\pi+\frac1{x(\log x)^2}+O\left(\frac1{x(\log x)^3}\right).}
$$

The endpoint correction refines to $[xL^2]^{-1}[1-2\gamma_E/L+3(\gamma_E^2+\pi^2/6)/L^2+\cdots]$, using [derivatives of the gamma function](../../../complex-analysis.md#derivative-of-the-gamma-function). An application of [Watson's lemma](../../../analysis.md#watson-s-lemma) confined to $u=0$ would omit the leading peak contribution $\pi$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The [Briggs-Bers technique](../../../wave-equation.md#briggs-bers-criterion) starts with a temporal [Laplace transform](../../../analysis.md#laplace-transform) and spatial [Fourier transform](../../../analysis.md#fourier-transform) of a localized disturbance. The temporal inversion contour must initially lie above every temporal singularity. Lower it while deforming the spatial contour away from the [roots of the dispersion relation](../../../wave-equation.md#spatial-root-of-a-dispersion-relation). A collision of spatial branches originating on opposite sides of that contour can create a [spatial pinch point](../../../wave-equation.md#spatial-pinch-point). A contributing pinch with $\operatorname{Im}\omega_*>0$ gives [absolute wave-packet instability](../../../wave-equation.md#absolute-wave-packet-instability): exponential growth at a fixed position. Growth that is transported away while a fixed position decays is [convective wave-packet instability](../../../wave-equation.md#convective-wave-packet-instability). Solving $D=D_k=0$ finds candidate double roots, but does not by itself establish a pinch.

Substitution of the [normal mode](../../../wave-equation.md#normal-mode) gives

$$
D(k,\omega)=-i\omega-\alpha k^2-i\beta k^3+\gamma=0,\qquad \boxed{\omega(k)=i\alpha k^2-\beta k^3-i\gamma.}
$$

For real [wavenumber](../../../wave-equation.md#wavenumber) $k$, the temporal [growth rate](../../../wave-equation.md#growth-rate) is

$$
\operatorname{Im}\omega(k)=(\operatorname{Re}\alpha)k^2-(\operatorname{Im}\beta)k^3-\operatorname{Re}\gamma.
$$

A nonzero real cubic coefficient in this expression makes it unbounded above on one end of the real axis. Once that coefficient vanishes, a positive quadratic coefficient also makes it unbounded above. Hence the [bounded temporal growth condition for cubic dispersion](../../../wave-equation.md#bounded-temporal-growth-condition-for-cubic-dispersion) is

$$
\boxed{\operatorname{Im}\beta=0,\qquad \operatorname{Re}\alpha\leq0.}
$$

The maximum is then $-\operatorname{Re}\gamma$, attained at $k=0$ and, when $\operatorname{Re}\alpha=0$, at all real $k$. A finite upper bound is necessary for choosing the initial temporal inversion contour; arbitrarily fast high-[wavenumber](../../../wave-equation.md#wavenumber) growth prevents the usual [Briggs-Bers criterion](../../../wave-equation.md#briggs-bers-criterion) from defining that causal inversion for generic localized data.

For $\beta\ne0$, the stationary candidates satisfy

$$
\omega'(k)=k(2i\alpha-3\beta k)=0,
$$

so

$$
k_*=0,\quad \omega_*=-i\gamma;\qquad k_*^{(1)}=\frac{2i\alpha}{3\beta},\quad \omega_*^{(1)}=-i\left(\gamma+\frac{4\alpha^3}{27\beta^2}\right).
$$

Each candidate must pass the spatial-branch pinch test before its imaginary [frequency](../../../physics.md#frequency) is used. In particular, under the finite-growth conditions the real-[wavenumber](../../../wave-equation.md#wavenumber) evolution has multiplier modulus at most $e^{-t\operatorname{Re}\gamma}$. For integrable transformed initial data this bounds its fixed-position amplitude by a constant times that exponential. Thus a further necessary condition is

$$
\boxed{\operatorname{Re}\gamma<0.}
$$

The [false complex saddle in dissipative cubic dispersion](../../../wave-equation.md#false-complex-saddle-in-dissipative-cubic-dispersion) illustrates why the second formal candidate cannot override this bound. For $\operatorname{Re}\alpha<0$, the neighborhood $k=0$ gives a fixed-position impulse response proportional to $e^{-\gamma t}/\sqrt t$: the cubic term is smaller on its $k=O(t^{-1/2})$ scale. It therefore supplies the usual growing pinch when $\operatorname{Re}\gamma<0$. The purely dispersive cases have stationary-phase algebraic prefactors instead. If $\beta=0$, only the quadratic stationary point remains; if both derivative coefficients vanish, the equation is local multiplication and its growth is directly $e^{-\gamma t}$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Write $r=\sqrt{\mu/\delta}$. At first order the amplitude-phase [perturbation](../../../analysis.md#perturbation) is $A=r+\varepsilon(A_1+ir\theta)+O(\varepsilon^2)$. Expanding the cubic term in the [focusing nonlinear Schrodinger equation](../../../integrable-systems.md#focusing-nonlinear-schrodinger-equation) gives $A|A|^2=r^3+\varepsilon(3r^2A_1+ir^3\theta)+O(\varepsilon^2)$. The constant terms cancel because $\delta r^2=\mu$. Separating real and [imaginary parts](../../../complex-analysis.md#imaginary-part) yields

$$
\boxed{(A_1)_t=\chi r\theta_{xx},\qquad r\theta_t+\chi(A_1)_{xx}+2\mu A_1=0.}
$$

For the Fourier [normal modes](../../../wave-equation.md#normal-mode), these equations give $-i\Omega\widehat A_1=-\chi rK^2\widehat\theta$ and $-ir\Omega\widehat\theta+(2\mu-\chi K^2)\widehat A_1=0$. Their [determinant](../../../linear-algebra.md#determinant) vanishes exactly when

$$
\boxed{\Omega^2=\chi K^2(\chi K^2-2\mu).}
$$

The [focusing nonlinear Schrodinger modulation dispersion](../../../wave-equation.md#focusing-nonlinear-schrodinger-modulation-dispersion) is negative for $0<K^2<2\mu/\chi$. One of the two [frequencies](../../../physics.md#frequency) then has positive imaginary part and grows exponentially: the constant state has [modulational instability](../../../wave-equation.md#modulational-instability). The [growth rate](../../../wave-equation.md#growth-rate) is $\sqrt{\chi K^2(2\mu-\chi K^2)}$, maximized at $K^2=\mu/\chi$ with value $\mu$. Modes beyond the unstable band have real [frequencies](../../../physics.md#frequency). The zero-[wavenumber](../../../wave-equation.md#wavenumber) phase mode is neutral, with possible linear phase drift from a uniform amplitude [perturbation](../../../analysis.md#perturbation).

## 2

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

First take $z>0$. Set $s=t^3-1$ in the tail integral. This puts it in the endpoint form needed for [Watson's lemma](../../../analysis.md#watson-s-lemma):

$$
F(z)=\frac{e^{-z^3}}3\int_0^\infty e^{-z^3s}(1+s)^{-2/3}\,ds.
$$

The binomial coefficients are $(-1)^r(2/3)_r/r!$, where $(a)_r=\Gamma(a+r)/\Gamma(a)$ is the [rising factorial](../../../combinatorics.md#rising-factorial). Integrating each endpoint term gives

$$
\boxed{F(z)\sim\frac{e^{-z^3}}{3z^3}\sum_{r\geq0}\frac{(-1)^r\Gamma(r+2/3)}{\Gamma(2/3)z^{3r}}.}
$$

Also, scaling the complete positive-ray integral gives $\int_0^\infty e^{-z^3t^3}dt=\Gamma(1/3)/(3z)$. Hence

$$
\boxed{G(z)\sim\frac{\Gamma(1/3)}{3z}-\frac{e^{-z^3}}{3z^3}\left[1-\frac{2}{3z^3}+\frac{10}{9z^6}-\cdots\right].}
$$

The endpoint term is exponentially small on this positive ray but must be retained for continuation to other sectors.

For complex $z$, use $s=zt$ so $G(z)=z^{-1}\int_0^z e^{-s^3}ds$. Put $C=\Gamma(1/3)/3$ and $\omega=e^{2\pi i/3}$. The complete [steepest descent contours](../../../analysis.md#steepest-descent-contour) from the cubic saddle are the rays $\arg s=2\pi j/3$, whose integrals are $C\omega^j$. Deform the finite contour onto one of these rays followed by the endpoint contour. The [cubic exponential integral Stokes sectors](../../../analysis.md#cubic-exponential-integral-stokes-sectors) give

$$
\boxed{G(z)\sim\frac{C\omega^j}{z}-\frac{e^{-z^3}}{3z^3}\sum_{r\geq0}\frac{(-1)^r(2/3)_r}{z^{3r}},\qquad \frac{(2j-1)\pi}{3}<\arg z<\frac{(2j+1)\pi}{3}.}
$$

For $0\leq\arg z\leq2\pi$, take $j=0$ below $\pi/3$, $j=1$ between $\pi/3$ and $\pi$, $j=2$ between $\pi$ and $5\pi/3$, and $j=3$ above $5\pi/3$. The corresponding algebraic coefficients are $C,C\omega,C\omega^2,C$. A negative-real $z$ provides a useful sign check: $G(z)=G(|z|e^{i\pi})$ is real and positive, so its two lateral algebraic coefficients must be [complex conjugates](../../../complex-analysis.md#complex-conjugate).

The subdominant algebraic term switches across the [Stokes lines](../../../analysis.md#stokes-line)

$$
\boxed{\arg z=\frac\pi3,\ \pi,\ \frac{5\pi}3.}
$$

There $z^3$ is negative real and the endpoint exponential is dominant. The intervening [anti-Stokes lines](../../../analysis.md#anti-stokes-line) are $\arg z=\pi/6+j\pi/3$, where $\operatorname{Re}z^3=0$ and the exponential changes from growth to decay. The naming convention here distinguishes switching from equal exponential magnitude.

To resolve the jump near $\theta_s=\pi/3$, optimally truncate the endpoint series at $N$ with $N+2/3=R+O(1)$, where $R=|z|^3$. Let $P_N$ denote that truncated endpoint contribution. The [Borel remainder for a cubic exponential integral](../../../analysis.md#borel-remainder-for-a-cubic-exponential-integral) derived in [solution](#2/a/solution), together with the [Gaussian pole transition for a large gamma parameter](../../../analysis.md#gaussian-pole-transition-for-a-large-gamma-parameter) in [solution](#2/b/solution), gives

$$
\boxed{G(z)=P_N(z)+\frac C z\left[1+(\omega-1)S(\theta)\right]+O\left(\frac1{|z|\sqrt R}\right),\qquad S(\theta)=\frac12\left[1+\operatorname{erf}\left(3(\theta-\pi/3)\sqrt{\frac R2}\right)\right].}
$$

This estimate is on the transition scale $\theta-\pi/3=O(R^{-1/2})$ after [optimal truncation](../../../analysis.md#optimal-truncation). The [error-function smoothing of a Stokes multiplier](../../../analysis.md#error-function-smoothing-of-a-stokes-multiplier) has width $O(|z|^{-3/2})$. Before the line $S\to0$ and the coefficient is $C$; after it $S\to1$ and the coefficient is $C\omega$, agreeing with the sector expansions. On the line the leading coefficient is their average. The original $G$ is an [entire function](../../../complex-analysis.md#entire-function); only its asymptotic decomposition has these sector-dependent coefficients.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The factorial tail provides the connection with the supplied [Borel summation](../../../analysis.md#borel-summation) formula. Near the first switching line choose $\lambda=-z^3$ with $\arg\lambda=3(\arg z-\pi/3)$, so $\lambda$ is near the positive real axis and $\lambda^{-1/3}=e^{i\pi/3}/z$. The endpoint contribution through $N-1$ terms is

$$
P_N(z)=\frac{e^\lambda}{3\lambda\Gamma(2/3)}\sum_{r=0}^{N-1}\frac{\Gamma(r+2/3)}{\lambda^r}.
$$

Writing $r=N+p$ in its formal remainder, with $\gamma=N+2/3$, gives

$$
\frac{\lambda^{-1/3}}{3\Gamma(2/3)}\sum_{p\geq0}\frac{\Gamma(\gamma+p)e^\lambda}{\lambda^{p+\gamma}}.
$$

Thus the [Borel remainder for a cubic exponential integral](../../../analysis.md#borel-remainder-for-a-cubic-exponential-integral), using the contour just above the pole specified in the paper, is

$$
\boxed{G(z)-P_N(z)=\frac C z+\frac{e^{i\pi/3}}{3\Gamma(2/3)z}I(\lambda,\gamma).}
$$

The continuation is chosen from the sector below the switching line. The term $C/z$ fixes that continuation; an alternative lateral pole contour would shift it by the corresponding residue. This is why the contour prescription must accompany the divergent factorial series.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Choose $N$ near the least term, so $\gamma=N+2/3=R+O(1)$ with $R=|z|^3$. On writing $\beta=3(\arg z-\pi/3)$, the parameter is $\lambda=Re^{i\beta}$. For $\beta=O(R^{-1/2})$,

$$
\lambda=R+iR\beta+O(1)=\gamma+i\mu\sqrt\gamma+O(1),\qquad \mu\sim\beta\sqrt R.
$$

The supplied [Gaussian pole transition for a large gamma parameter](../../../analysis.md#gaussian-pole-transition-for-a-large-gamma-parameter) therefore gives $I\sim i\pi[1+\operatorname{erf}(\mu/\sqrt2)]$. Substitution in [solution](#2/a/solution) gives the smoothing formula in [solution](#2/solution) once the amplitude identity in [solution](#2/c/solution) is used.

The origin of the [error function](../../../calculus.md#error-function) can also be seen locally. Set $t=1+s/\sqrt\gamma$ in the Borel integral. Then

$$
(\gamma-1)\log t+\lambda(1-t)=-\frac{s^2}{2}-i\mu s+O(\gamma^{-1/2}),\qquad \frac{dt}{1-t}=-\frac{ds}{s}.
$$

The saddle has become a [Gaussian integral](../../../calculus.md#gaussian-integral) meeting a simple pole. With the upper-pole contour, the leading integral is $-\int_{\mathcal C_+}e^{-s^2/2-i\mu s}ds/s$. Its value at $\mu=0$ is $i\pi$ from the indentation. Differentiating with respect to $\mu$ gives $i\sqrt{2\pi}e^{-\mu^2/2}$, so integration from zero gives $i\pi[1+\operatorname{erf}(\mu/\sqrt2)]$. This independently fixes the sign and the half-jump on the [Stokes line](../../../analysis.md#stokes-line).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [gamma reflection formula](../../../complex-analysis.md#gamma-reflection-formula), $\Gamma(a)\Gamma(1-a)=\pi/\sin(\pi a)$, at $a=1/3$ gives $\Gamma(1/3)\Gamma(2/3)=2\pi/\sqrt3$. Consequently, with $\omega=e^{2\pi i/3}$ and $C=\Gamma(1/3)/3$,

$$
\boxed{\frac{2\pi i e^{i\pi/3}}{3\Gamma(2/3)}=C(\omega-1).}
$$

Multiplication by $[1+\operatorname{erf}(\mu/\sqrt2)]/2$ therefore changes the algebraic coefficient by exactly the required amount, from $C$ to $C\omega$. This confirms both the magnitude and phase of the smoothed jump, rather than only its error-function shape.

## 3

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [square-root reaction problem with nested boundary layers](../../../differential-equation.md#square-root-reaction-problem-with-nested-boundary-layers) has a small positive plateau $y\sim\varepsilon^2k^2$, an $O(\varepsilon)$ left-end layer, and two distinct scales on the right. The broad right layer has width $O(\sqrt\varepsilon)$; its inner edge needs a thinner $O(\varepsilon)$ transition to the plateau. A single right-end scale cannot describe both matches.

Here is a uniformly matched leading solution. Let $L(\xi)$ solve

$$
L''=\sqrt L-k,\qquad L(0)=0,\qquad L(+\infty)=k^2,
$$

using the increasing branch below $k^2$. Define

$$
\Phi(Y)=\sqrt{2k}\log\left|\frac{\sqrt{k+2\sqrt Y}-\sqrt{3k}}{\sqrt{k+2\sqrt Y}+\sqrt{3k}}\right|+\sqrt{6(k+2\sqrt Y)}.
$$

Then $\Phi(L(\xi))=\Phi(0)-\xi$. For the right-hand branch, define $R(\xi)>k^2$ by $\Phi(R(\xi))=\xi$; it tends to $k^2$ as $\xi\to-\infty$. These formulas follow from the [first integral of a square-root reaction layer](../../../differential-equation.md#first-integral-of-a-square-root-reaction-layer) and are expanded in [solution](#3/b/i/solution) and [solution](#3/b/ii/solution).

For sufficiently small $\varepsilon$, let $x_*=1-\varepsilon\Phi(\varepsilon^{-2})$. Then $R((1-x_*)/\varepsilon)=\varepsilon^{-2}$, so the right profile meets the prescribed order-one endpoint. The [composite asymptotic expansion](../../../differential-equation.md#additive-composite-expansion) is

$$
\boxed{y_{\rm comp}(x)=\varepsilon^2\left[L\left(\frac x\varepsilon\right)+R\left(\frac{x-x_*}{\varepsilon}\right)-k^2\right],\qquad 0\leq x\leq1.}
$$

The subtraction removes the common plateau counted twice. Its boundary residuals are exponentially small: the right profile has almost reached $k^2$ at $x=0$, and the left profile has almost reached $k^2$ at $x=1$. In each active layer the opposite profile is exponentially close to its plateau, so the composite reproduces that layer's governing equation and the shared [outer solution](../../../differential-equation.md#outer-expansion) to the retained order.

The right transition location satisfies $x_*=1-2\sqrt{3\varepsilon}+o(\sqrt\varepsilon)$. Outside its thin transition, the broad right layer is

$$
y\sim\left[1-\frac{1-x}{2\sqrt{3\varepsilon}}\right]^4
$$

where the bracket is positive; it matches through the thin layer to $\varepsilon^2k^2$, rather than continuing as a fourth power on the wrong side. The [dominant balances](../../../analysis.md#dominant-balance) and the end-region matches are detailed below.

<a id="3/image-the-left-layer-small-plateau-and-two-right-hand-scales-of-the-square-root-reaction-problem"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-79-nested-layers.png)

**[Figure 1](#3/image-the-left-layer-small-plateau-and-two-right-hand-scales-of-the-square-root-reaction-problem). The left layer, small plateau and two right-hand scales of the square-root reaction problem**.

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

In the [outer solution](../../../differential-equation.md#outer-expansion), derivative terms are small and $\sqrt y\sim\varepsilon k$, so $y_{\rm out}\sim\varepsilon^2k^2$. To resolve its mismatch with the zero left boundary, set $x=\varepsilon\xi$, $y=\varepsilon^2Y$. The original equation becomes exactly $Y''-\sqrt Y+k=0$. The left [inner variable](../../../differential-equation.md#inner-variable) is therefore $\xi=x/\varepsilon$, with $Y(0)=0$ and $Y\to k^2$ as $\xi\to+\infty$.

Multiplying by $Y'$ gives the [first integral of a square-root reaction layer](../../../differential-equation.md#first-integral-of-a-square-root-reaction-layer). Matching $Y=k^2$, $Y'=0$ fixes its constant:

$$
\frac12(Y')^2-\frac23Y^{3/2}+kY=\frac{k^3}{3},\qquad \boxed{(Y')^2=\frac23(\sqrt Y-k)^2(2\sqrt Y+k).}
$$

The positive derivative branch below $k^2$ begins with $Y'(0)=\sqrt{2k^3/3}$ and approaches the plateau exponentially. Thus the left layer has thickness $O(\varepsilon)$, not $O(\sqrt\varepsilon)$ despite the coefficient on the original second [derivative](../../../calculus.md#derivative). Its small amplitude is essential in the [dominant balance](../../../analysis.md#dominant-balance).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Put $w=\sqrt Y$. The separated [first integral of a square-root reaction layer](../../../differential-equation.md#first-integral-of-a-square-root-reaction-layer) gives a primitive $\Phi(Y)$ as defined in [solution](#3/solution). One can verify it directly: above the plateau,

$$
\frac{d\Phi}{dY}=\left[\frac23(\sqrt Y-k)^2(2\sqrt Y+k)\right]^{-1/2},
$$

while below it the derivative has the opposite sign. Accordingly the increasing left profile uses $\Phi(L)=\Phi(0)-\xi$, and the increasing right profile uses $\Phi(R)=\xi$ after choosing its translation constant.

As $w\to k$, the logarithm dominates:

$$
\Phi(Y)=\sqrt{2k}\log|w-k|+O(1).
$$

Hence the left profile approaches from below with $|\sqrt L-k|\propto e^{-\xi/\sqrt{2k}}$, while the right profile approaches from above with $|\sqrt R-k|\propto e^{\xi/\sqrt{2k}}$ as $\xi\to-\infty$. These are precisely the required two plateau [matching conditions](../../../differential-equation.md#asymptotic-matching-condition). The absolute value in the logarithm is necessary to use the same real primitive on both sides.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

For $Y\gg k^2$, the [first integral of a square-root reaction layer](../../../differential-equation.md#first-integral-of-a-square-root-reaction-layer) reduces to $Y'\sim(2/\sqrt3)Y^{3/4}$. Integrating gives $Y^{1/4}\sim\xi/(2\sqrt3)$ after a possible translation, or

$$
\boxed{Y\sim\frac{\xi^4}{144}.}
$$

For the right profile $R$ this large-positive-$\xi$ limit matches a broader scale with $y=O(1)$. Since $y=\varepsilon^2R$ and $\xi=(x-x_*)/\varepsilon$, the overlap is

$$
y\sim\frac{(x-x_*)^4}{144\varepsilon^2},\qquad \varepsilon\ll x-x_*\ll\sqrt\varepsilon.
$$

Thus the translated $O(\varepsilon)$ layer lies between the outer plateau and the $O(\sqrt\varepsilon)$ boundary layer. The large-$Y$ primitive also gives $\Phi(\varepsilon^{-2})\sim2\sqrt3/\sqrt\varepsilon$, establishing the leading location $x_*=1-2\sqrt{3\varepsilon}$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For the broad right layer take $\zeta=(x-1)/\sqrt\varepsilon$ and $y=Z(\zeta)$, so $\zeta\leq0$ inside the interval. Its leading equation is $Z''=\sqrt Z$, with $Z(0)=1$. One integration gives $(Z')^2=(4/3)(Z^{3/2}+c)$. The positive derivative branch produces the integral parametrization in the hint.

Matching to a small, nearly flat plateau requires $Z\to0$ and $Z'\to0$ at the inner edge, so **the leading integration constant is $c=0$**. A positive order-one $c$ would leave a nonzero slope as $Z\to0$; a negative one would prevent that limit. For $c=0$, integration with $Z(0)=1$ gives

$$
\boxed{Z(\zeta)=\left(1+\frac{\zeta}{2\sqrt3}\right)^4,\qquad -2\sqrt3\leq\zeta\leq0.}
$$

Its zero is at $\zeta=-2\sqrt3$, namely $x=1-2\sqrt{3\varepsilon}$. Near that edge it has the fourth-power overlap obtained in [solution](#3/b/ii/solution). The neglected $\varepsilon k$ reaction term becomes comparable to $\sqrt Z$ when $Z=O(\varepsilon^2)$, precisely where the thinner transition must restore it. The sketch in [solution](#3/solution) shows the plateau and both right-hand regions; extending the quartic profile past its inner edge would fail to match the positive plateau.

## 4

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

Use the [method of multiple scales](../../../differential-equation.md#method-of-multiple-scales), $T=\varepsilon t$, and write $x_0=A(T)\cos\psi$, $\psi=t+\theta(T)$. At first order,

$$
(\partial_t^2+1)x_1=2A_T\sin\psi+2A\theta_T\cos\psi+A f(A\cos\psi)\sin\psi.
$$

Removing the fundamental [secular terms](../../../differential-equation.md#secular-term) gives the [averaged amplitude for position-dependent damping](../../../differential-equation.md#averaged-amplitude-for-position-dependent-damping):

$$
A_T=-A\langle f(A\cos\psi)\sin^2\psi\rangle,\qquad \theta_T=0,
$$

where the brackets mean a full-period average. The [initial conditions](../../../differential-equation.md#initial-condition) set $A(0)=1$ and $\theta(0)=0$ at leading order. For quadratic damping, $\langle\sin^2\psi\rangle=1/2$ and $\langle\cos^2\psi\sin^2\psi\rangle=1/8$, giving

$$
A_T=\frac A2-\frac{A^3}{8},\qquad A(T)=\frac2{\sqrt{1+3e^{-T}}}.
$$

Thus the [Van der Pol amplitude evolution](../../../differential-equation.md#van-der-pol-amplitude-evolution) yields

$$
\boxed{x(t;\varepsilon)=\frac{2\cos t}{\sqrt{1+3e^{-\varepsilon t}}}+O(\varepsilon),\qquad 0\leq t\leq C/\varepsilon.}
$$

The leading amplitude approaches the stable value two. The small initial-velocity discrepancy introduced by the slow amplitude derivative is removed by the first-order correction and does not affect this leading approximation.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

For $f(x)=\sin x$, the period average $\langle\sin(A\cos\psi)\sin^2\psi\rangle$ vanishes: a half-period shift reverses the first factor and leaves the second unchanged. This is the [zero first-order amplitude drift for odd damping](../../../differential-equation.md#odd-position-dependent-damping-has-zero-first-order-amplitude-drift). The [averaged amplitude for position-dependent damping](../../../differential-equation.md#averaged-amplitude-for-position-dependent-damping) therefore has $A_T=0$, while its first-order phase equation again has $\theta_T=0$. With the [initial conditions](../../../differential-equation.md#initial-condition),

$$
\boxed{x(t;\varepsilon)=\cos t+O(\varepsilon),\qquad 0\leq t\leq C/\varepsilon.}
$$

The first-order forcing has no fundamental resonant component, so it produces bounded corrections rather than a secular amplitude change on this time scale. This statement concerns the leading approximation on $t=O(\varepsilon^{-1})$.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

For $f(x)=|x|$ and positive amplitude $A$, the [averaged amplitude for position-dependent damping](../../../differential-equation.md#averaged-amplitude-for-position-dependent-damping) gives

$$
A_T=-A^2\langle|\cos\psi|\sin^2\psi\rangle.
$$

The average is $(4/(2\pi))\int_0^{\pi/2}\cos\psi\sin^2\psi\,d\psi=2/(3\pi)$. Thus the [absolute-value damping amplitude law](../../../differential-equation.md#absolute-value-damping-amplitude-law) is

$$
A_T=-\frac{2A^2}{3\pi},\qquad A(T)=\frac1{1+2T/(3\pi)},
$$

and $\theta_T=0$ as in the other cases. Consequently,

$$
\boxed{x(t;\varepsilon)=\frac{\cos t}{1+2\varepsilon t/(3\pi)}+O(\varepsilon),\qquad 0\leq t\leq C/\varepsilon.}
$$

The dissipation makes the leading envelope decrease algebraically in slow time. The absolute value is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity), so the first-order averaging argument remains valid despite its corner at zero.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

First assume the usual diffusion regime $\gamma>0$, with $U$ real; the complex-diffusion extension is described below. Substitution of a global [normal mode](../../../wave-equation.md#normal-mode) gives

$$
\gamma a''-Ua'+(\mu_0-\nu\varepsilon^2x^2+i\omega_G)a=0.
$$

Set $a=e^{Ux/(2\gamma)}b$ to remove the first [derivative](../../../calculus.md#derivative), then put $\xi=\sqrt\varepsilon(\nu/\gamma)^{1/4}x$. The resulting oscillator equation is

$$
\boxed{b_{\xi\xi}+(\Lambda-\xi^2)b=0,\qquad \Lambda=\frac{\mu_0-U^2/(4\gamma)+i\omega_G}{\varepsilon\sqrt{\gamma\nu}}.}
$$

Writing $b=e^{-\xi^2/2}H(\xi)$ gives the [Hermite differential equation](../../../analysis.md#hermite-differential-equation), $H''-2\xi H'+(\Lambda-1)H=0$. For a [power series](../../../real-analysis.md#power-series) $H=\sum_{j\geq0}c_j\xi^j$, its recurrence is

$$
c_{j+2}=\frac{2j+1-\Lambda}{(j+2)(j+1)}c_j.
$$

Termination at degree $n$ requires $\Lambda=2n+1$. If it does not terminate in the appropriate parity, the series has a growing Gaussian component at one infinity; the solution decaying at one end then fails at the other. The [Hermite oscillator quantization](../../../analysis.md#hermite-oscillator-quantization) can also be seen from the self-adjoint operator $-d^2/d\xi^2+\xi^2$, whose square-integrable [eigenfunctions](../../../linear-operator-theory.md#eigenfunction) are the [Hermite functions](../../../numerical-analysis.md#hermite-function). Their spectrum is $2n+1$ with $n=0,1,2,\ldots$. The ground state $H_0=1$ shows that the paper's phrase “positive integer” must include zero.

The [global modes of a quadratically confined Ginzburg-Landau equation](../../../hydrodynamic-stability.md#global-modes-of-a-quadratically-confined-ginzburg-landau-equation) are therefore

$$
\boxed{\omega_{G,n}=i\left[\mu_0-\frac{U^2}{4\gamma}-(2n+1)\varepsilon\sqrt{\gamma\nu}\right],\qquad n=0,1,2,\ldots.}
$$

Their spatial functions are proportional to $e^{Ux/(2\gamma)}e^{-\xi^2/2}H_n(\xi)$; the quadratic Gaussian decay dominates the linear drift factor at both infinities. For real coefficients, the most dangerous mode is $n=0$. The system has [global hydrodynamic instability](../../../hydrodynamic-stability.md#global-hydrodynamic-instability) precisely when

$$
\boxed{\mu_0>\frac{U^2}{4\gamma}+\varepsilon\sqrt{\gamma\nu}.}
$$

Equality is marginal and smaller $\mu_0$ gives decay of all these modes. The finite-width confinement correction explains why a locally absolutely unstable region need not immediately support a growing global mode.

If complex diffusion is intended, impose the parabolic condition $\operatorname{Re}\gamma>0$ and choose $\sqrt{\nu/\gamma}$ with positive real part. The same formulas continue along the rotated $\xi$ ray, with the corresponding branch of $\sqrt{\gamma\nu}$; instability is determined by the real part of the square bracket. Arbitrary constant $\gamma$, especially negative diffusion, does not justify the asserted whole-line Hermite decay or a well-posed evolution.

## 5

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Let $q^2=k^2+l^2$ and $c=c_r+ic_i$, with $k>0$ chosen for the temporal mode convention. In the [inviscid limit](../../../viscous-fluid-flow.md#euler-limit), the [Orr-Sommerfeld equation](../../../hydrodynamic-stability.md#orr-sommerfeld-equation) reduces to the [Rayleigh equation for inviscid shear flow](../../../hydrodynamic-stability.md#rayleigh-equation-for-inviscid-shear-flow):

$$
v''-q^2v-\frac{U''}{U-c}v=0.
$$

The impermeability [boundary condition](../../../differential-equation.md#boundary-condition) is $v(\pm1)=0$; the extra viscous derivative condition is not an independent condition for this reduced second-order equation. For an unstable mode $c_i>0$, the denominator has no real zero. Multiply by $\bar v$ and apply [integration by parts](../../../calculus.md#integration-by-parts) to obtain

$$
\int_{-1}^{1}(|v'|^2+q^2|v|^2)\,dy+\int_{-1}^{1}\frac{U''(U-c_r+ic_i)}{|U-c|^2}|v|^2\,dy=0.
$$

Its imaginary part gives

$$
\boxed{c_i\int_{-1}^{1}\frac{U''|v|^2}{|U-c|^2}\,dy=0.}
$$

For a nontrivial mode, the weight is nonnegative and is positive except at isolated mode zeros. Thus $U''$ must take both signs, unless it vanishes identically. The identically zero case also has no unstable nontrivial mode, by the positive first integral in the displayed identity. Therefore the smooth real base-flow profile must have an interior [inflection point](../../../topology.md#inflection-point). This proves [Rayleigh's inflection-point theorem](../../../hydrodynamic-stability.md#rayleigh-s-inflection-point-theorem); it is a necessary condition, not a sufficiency test.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

For $k>0$, put $q=\sqrt{k^2+l^2}$ and define the [Squire transformation](../../../hydrodynamic-stability.md#squire-transformation)

$$
\boxed{k'=q,\qquad l'=0,\qquad R'=\frac{k}{q}R,\qquad c'=c,\qquad \omega'=qc.}
$$

The two-dimensional [Orr-Sommerfeld equation](../../../hydrodynamic-stability.md#orr-sommerfeld-equation) then has the same transverse operator because $k'^2=q^2$, and the same viscous coefficient because $k'R'=kR$. Its [boundary conditions](../../../differential-equation.md#boundary-condition) on $v$ and $v'$ are unchanged. Thus it has the same [eigenfunction](../../../linear-operator-theory.md#eigenfunction) and the same phase-speed [eigenvalue](../../../linear-operator-theory.md#eigenvalue).

If the original disturbance grows, $\operatorname{Im}c>0$, so the transformed disturbance also grows. Since $R'\leq R$, every unstable three-dimensional mode maps to an unstable two-dimensional mode at a no larger [Reynolds number](../../../fluid-mechanics.md#reynolds-number). It follows that **the minimum critical Reynolds number is attained among two-dimensional disturbances**. This is the [Squire theorem](../../../hydrodynamic-stability.md#squire-s-theorem) for temporal normal-mode onset, not a statement that three-dimensional transient amplification is impossible. The case $k=0$ is treated separately without dividing by $k$; its streamwise-uniform viscous [normal modes](../../../wave-equation.md#normal-mode) decay, although coupling can produce [transient growth](../../../linear-operator-theory.md#transient-growth).

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

Multiply the homogeneous [Squire equation](../../../hydrodynamic-stability.md#squire-equation) by $\bar\eta$ and integrate over the channel. The zero boundary values remove the [integration by parts](../../../calculus.md#integration-by-parts) boundary term, giving

$$
-i\omega\int_{-1}^{1}|\eta|^2dy+ik\int_{-1}^{1}U|\eta|^2dy+\frac1R\int_{-1}^{1}(|\eta'|^2+q^2|\eta|^2)dy=0.
$$

For real $U$ and $k$, the middle term is purely imaginary. Taking [real parts](../../../complex-analysis.md#real-part) yields the [dissipation identity for a homogeneous Squire mode](../../../hydrodynamic-stability.md#dissipation-identity-for-a-homogeneous-squire-mode):

$$
\boxed{\operatorname{Im}\omega=-\frac{\int_{-1}^{1}(|\eta'|^2+q^2|\eta|^2)dy}{R\int_{-1}^{1}|\eta|^2dy}<0.}
$$

The strict inequality holds for a nonzero mode with zero endpoint values and positive [Reynolds number](../../../fluid-mechanics.md#reynolds-number). Hence **all homogeneous Squire modes are temporally stable**. In the complete shear-flow [perturbation](../../../analysis.md#perturbation) system, the Squire variable can also be forced by the wall-normal velocity; this homogeneous-mode result does not rule out instability of that coupled system or its [transient growth](../../../linear-operator-theory.md#transient-growth).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Take the norm to be the [Euclidean norm](../../../functional-analysis.md#euclidean-norm). The solution is $\mathbf q(t)=e^{tA}\mathbf q(0)$, so optimal growth is the [operator norm](../../../continuous-dual-space.md#operator-norm) $G(t)=\|e^{tA}\|_2$, equivalently the largest [singular value](../../../linear-algebra.md#singular-value) of the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential). Let $s(A)$ be the [spectral abscissa](../../../linear-operator-theory.md#spectral-abscissa) and let $w(A)=\lambda_{\max}((A+A^*)/2)$ be the [numerical abscissa](../../../continuous-dual-space.md#euclidean-logarithmic-norm). The [Euclidean semigroup growth bounds](../../../continuous-dual-space.md#euclidean-semigroup-growth-bounds) are

$$
\boxed{e^{ts(A)}\leq G(t)\leq e^{tw(A)},\qquad t\geq0.}
$$

For the lower bound, the [spectral radius](../../../analysis.md#spectral-radius) of $e^{tA}$ is $e^{ts(A)}$ and is bounded by its [operator norm](../../../continuous-dual-space.md#operator-norm). For the upper bound, differentiating $\|\mathbf q\|_2^2$ gives $2\operatorname{Re}(\mathbf q^*A\mathbf q)\leq2w(A)\|\mathbf q\|_2^2$, and integration gives the result. A [non-normal matrix](../../../linear-operator-theory.md#non-normal-matrix) can have $w(A)>s(A)$, allowing transient amplification even when all its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) have negative [real parts](../../../complex-analysis.md#real-part).

For the triangular matrix, $s(M)=-1/R$. The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of its [Hermitian part](../../../hilbert-space.md#hermitian-part-of-a-matrix) are $-3/(2R)\pm\tfrac12\sqrt{1+R^{-2}}$, so

$$
\boxed{e^{-t/R}\leq G(t)\leq\exp\left[\left(-\frac{3}{2R}+\frac12\sqrt{1+\frac1{R^2}}\right)t\right].}
$$

The upper exponent becomes positive when $R>\sqrt8$, even though the long-time spectrum is stable.

The two equations are $q_1'=-q_1/R$ and $q_2'=q_1-2q_2/R$. Solve the first, then use an [integrating factor](../../../differential-equation.md#integrating-factor) in the second. Writing $s=t/R$, $a=e^{-s}$, $b=e^{-2s}$ and $c=R(a-b)$ gives

$$
\boxed{B(t)=e^{tM}=\begin{pmatrix}a&0\\c&b\end{pmatrix}.}
$$

The maximizing initial state is the unit [eigenvector](../../../linear-operator-theory.md#eigenvector) of $B^*B$ belonging to its largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue). Here

$$
B^*B=\begin{pmatrix}a^2+c^2&cb\\cb&b^2\end{pmatrix},\qquad G(t)^2=\frac{T+\sqrt{T^2-4a^2b^2}}2,\qquad T=a^2+b^2+c^2.
$$

For $t>0$, define

$$
d=\frac{a^2+c^2-b^2}{2cb}=\frac{e^s+1}{2R}+\frac R2(e^s-1),\qquad r=\sqrt{1+d^2}-d.
$$

The [optimal initial state for triangular stable shear](../../../linear-operator-theory.md#optimal-initial-state-for-triangular-stable-shear) is therefore

$$
\boxed{\mathbf q_{\rm opt}(0)=\frac1{\sqrt{1+r^2}}\begin{pmatrix}1\\r\end{pmatrix}.}
$$

Multiplication by any nonzero complex [scalar](../../../vector-space.md#scalar) gives the same growth ratio; at $t=0$, every nonzero initial state is optimal.

For $t\gg R$, $d\to\infty$ and $r\to0$. Thus **the optimal initial state tends to $(1,0)^T$**, and $G(t)\sim e^{-t/R}\sqrt{1+R^2}$. The initial first component excites the slower eigenmode and its amplified second component.

For $t\ll R$, the exact expression gives $d=(R^{-1}+t/2)[1+O(t/R)]$. Accordingly the [short-relative-time optimal state for triangular shear](../../../linear-operator-theory.md#short-relative-time-optimal-state-for-triangular-shear) uses

$$
\boxed{r\sim\sqrt{1+\left(\frac1R+\frac t2\right)^2}-\left(\frac1R+\frac t2\right).}
$$

This retains both the unequal damping rates and the shear. If $R\gg1$, it reduces to $r\sim(\sqrt{t^2+4}-t)/2$, the maximizing direction for the shear matrix $\begin{pmatrix}1&0\\t&1\end{pmatrix}$. If time also tends to zero at fixed $R$, it instead tends to $r=\sqrt{1+R^{-2}}-R^{-1}$, the largest-[eigenvalue](../../../linear-operator-theory.md#eigenvalue) direction of the [Hermitian part](../../../hilbert-space.md#hermitian-part-of-a-matrix) of $M$. Merely setting $t/R$ small does not justify setting $t$ small; the exact formula resolves both possibilities.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
