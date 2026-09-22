# Bessel function

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bessel_function)

**Table of contents**

- [Bessel inverse-power expansion at infinity](#bessel-inverse-power-expansion-at-infinity)
- [Hankel function](#hankel-function)
  - [Hankel asymptotic sectors](#hankel-asymptotic-sectors)
- [Bessel function of the second kind](#bessel-function-of-the-second-kind)
  - [Spherical Bessel function of the second kind](#spherical-bessel-function-of-the-second-kind)
- [Spherical Bessel function](#spherical-bessel-function)
  - [Spherical Helmholtz matching to a decaying harmonic exterior](#spherical-helmholtz-matching-to-a-decaying-harmonic-exterior)
  - [Frobenius resonance in the spherical Bessel equation](#frobenius-resonance-in-the-spherical-bessel-equation)
  - [Logarithmic spherical Bessel square integral](#logarithmic-spherical-bessel-square-integral)
  - [Spherical Hankel function](#spherical-hankel-function)
    - [Fixed-argument growth of spherical Hankel functions](#fixed-argument-growth-of-spherical-hankel-functions)
  - [Spherical Bessel product integral](#spherical-bessel-product-integral)
- [Bessel function of the first kind](#bessel-function-of-the-first-kind)
  - [Integer-order Bessel reflection identity](#integer-order-bessel-reflection-identity)
  - [Bessel functions of order one half](#bessel-functions-of-order-one-half)
  - [Fourier transform of the Bessel function J0](#fourier-transform-of-the-bessel-function-j0)
  - [Jacobi-Anger expansion](#jacobi-anger-expansion)
    - [Bessel second-moment identity](#bessel-second-moment-identity)
  - [Quartic truncation of the Bessel function J0](#quartic-truncation-of-the-bessel-function-j0)
  - [Debye asymptotic for oscillatory Bessel functions](#debye-asymptotic-for-oscillatory-bessel-functions)
  - [Large-argument asymptotic expansion of the Bessel function of the first kind](#large-argument-asymptotic-expansion-of-the-bessel-function-of-the-first-kind)
- [Bessel differential equation](#bessel-differential-equation)
  - [Frobenius series for Bessel functions](#frobenius-series-for-bessel-functions)
  - [Sturm-Liouville formulation with Bessel order as eigenvalue](#sturm-liouville-formulation-with-bessel-order-as-eigenvalue)
- [Modified Bessel function](#modified-bessel-function)
  - [Large-argument asymptotic expansion of a modified Bessel function](#large-argument-asymptotic-expansion-of-a-modified-bessel-function)
  - [Modified Bessel function of the first kind](#modified-bessel-function-of-the-first-kind)
  - [Modified Bessel differential equation](#modified-bessel-differential-equation)
  - [Modified Bessel function of the second kind](#modified-bessel-function-of-the-second-kind)
    - [Fourier transform of the modified Bessel function K0](#fourier-transform-of-the-modified-bessel-function-k0)
    - [Integral representation of the modified Bessel function of the second kind](#integral-representation-of-the-modified-bessel-function-of-the-second-kind)
    - [Large-order asymptotic of the modified Bessel function of the second kind](#large-order-asymptotic-of-the-modified-bessel-function-of-the-second-kind)
  - [Laplace integral method for a differential equation](#laplace-integral-method-for-a-differential-equation)
    - [Laplace integral solution of a singular third-order equation](#laplace-integral-solution-of-a-singular-third-order-equation)
    - [Laguerre contour-integral amplitude](#laguerre-contour-integral-amplitude)
      - [Finite Laguerre contour solution](#finite-laguerre-contour-solution)
        - [Integer-parameter Laguerre contour residues](#integer-parameter-laguerre-contour-residues)
    - [Real integral representation of the modified Bessel function I0](#real-integral-representation-of-the-modified-bessel-function-i0)

## Bessel inverse-power expansion at infinity

↑ **Parent:** [Bessel function](bessel-function.md)

For $w''+[1-A/z^2]w=0$, with $A=n^2-1/4$, substitution gives $s=\pm i$, exponent zero and $c_{k+1}=[k(k+1)-A]c_k/[2s(k+1)]$. Thus the first correction is $c_1=sAc_0/2$. For integer $n$ no coefficient truncation occurs and coefficient ratios grow as $k/(2s)$; this is an [asymptotic expansion](asymptotic-expansion.md), not a convergent series at a finite $z$. The leading [Liouville–Green approximation](analysis.md#wkb-approximation) $q^{-1/4}e^{\pm i\int\sqrt q}$ has the same $1/z$ correction.

## Hankel function

↑ **Parent:** [Bessel function](bessel-function.md)

The two Hankel functions $H_\nu^{(1)}=J_\nu+iY_\nu$ and $H_\nu^{(2)}=J_\nu-iY_\nu$ solve the [Bessel differential equation](#bessel-differential-equation). Their large-argument forms distinguish outgoing and incoming oscillations and have sector-dependent [asymptotic expansions](asymptotic-expansion.md).

### Hankel asymptotic sectors

↑ **Parent:** [Hankel function](#hankel-function)

For fixed order, the standard [Hankel function](#hankel-function) expansions in $e^{\pm iz}z^{-1/2}$ are valid in different sectors on a chosen argument sheet. Analytic continuation can mix exponentials; the sectors must be specified rather than treating a formal inverse-power series as global.

## Bessel function of the second kind

↑ **Parent:** [Bessel function](bessel-function.md)

For noninteger order, $Y_\nu=(\cos(\pi\nu)J_\nu-J_{-\nu})/\sin(\pi\nu)$; the integer-order function is defined by a limit. It gives a second independent solution of the [Bessel differential equation](#bessel-differential-equation). At order zero, $Y_0(z)\sim(2/\pi)[\log(z/2)+\gamma]$ near positive zero and $Y_0(z)\sim\sqrt{2/(\pi z)}\sin(z-\pi/4)$ at large positive argument, where $\gamma$ is the [Euler--Mascheroni constant](complex-analysis.md#euler-s-constant).

### Spherical Bessel function of the second kind

↑ **Parent:** [Bessel function of the second kind](#bessel-function-of-the-second-kind)

The spherical second-kind function is $n_\ell(z)=\sqrt{\pi/(2z)}Y_{\ell+1/2}(z)$. Together with the first-kind [Spherical Bessel function](#spherical-bessel-function), it spans the radial free-wave solutions; $n_\ell(z)\sim-\cos(z-\ell\pi/2)/z$ at large positive $z$.

## Spherical Bessel function

↑ **Parent:** [Bessel function](bessel-function.md)

The spherical Bessel functions solve the radial wave equation in three dimensions. In particular,

$$
j_2(x)=\left(\frac3{x^3}-\frac1x\right)\sin x-\frac3{x^2}\cos x,
\qquad j_2(x)=\frac{x^2}{15}+O(x^4).
$$

The apparent singularity at the origin is removable, as follows from the power series of the [Bessel function of the first kind](#bessel-function-of-the-first-kind).

### Spherical Helmholtz matching to a decaying harmonic exterior

↑ **Parent:** [Spherical Bessel function](#spherical-bessel-function)

A scalar field solving the [Helmholtz equation](partial-differential-equation.md#helmholtz-equation) inside a sphere of radius $R$ and [Laplace's equation](partial-differential-equation.md#laplace-equation) outside has a regular interior mode $b\,j_\ell(\sqrt{s}\,r)P_\ell(\cos\theta)$ and a decaying exterior mode $a r^{-\ell-1}P_\ell(\cos\theta)$. Continuity of the field and its radial derivative gives, for $x=\sqrt{s}R>0$,

$$
xj_\ell'(x)+(\ell+1)j_\ell(x)=0.
$$

The [Spherical Bessel function](#spherical-bessel-function) recurrence turns this into $j_{\ell-1}(x)=0$, not $j_\ell(x)=0$. This elimination does not require division by a possibly vanishing boundary value.

For $\ell=0$, $j_0(x)=\sin x/x$ and $j_{-1}(x)=\cos x/x$, so the first positive root is $\pi/2$. For $\ell=1$, the matching condition is $j_0(x)=0$, whose first positive root is $\pi$. The distinction matters when a scalar model permits the monopole sector but a physical multipole model excludes it.

To compare angular sectors, put $u=rj_\ell(\sqrt{s}r)$. Its equation and boundary conditions are $-u''+\ell(\ell+1)u/r^2=su$, $u(0)=0$ and $u'(R)+\ell u(R)/R=0$. Its [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) is

$$
s=\frac{\int_0^R[|u'|^2+\ell(\ell+1)|u|^2/r^2]dr+\ell|u(R)|^2/R}{\int_0^R|u|^2dr}.
$$

Both added terms are nonnegative and increase with $\ell$. Thus the lowest scalar eigenvalue is $\pi^2/(4R^2)$ in the $\ell=0$ sector; if only $\ell\geq1$ is admitted, the lowest is $\pi^2/R^2$ in the $\ell=1$ sector. Zeros at $x=0$ caused by the vanishing normalization of $j_\ell$ are not additional eigenvalues.

### Frobenius resonance in the spherical Bessel equation

↑ **Parent:** [Spherical Bessel function](#spherical-bessel-function)

For $x^2y''+2xy'+[x^2-\ell(\ell+1)]y=0$ with integer $\ell\geq0$, the [Frobenius method](complex-analysis.md#frobenius-method) gives $\sigma=\ell$ or $-\ell-1$. The general coefficient equation is $[(j+\sigma)(j+\sigma+1)-\ell(\ell+1)]a_j=-a_{j-2}$, taking negative-index coefficients as zero. The regular branch has $a_1=0$ and $a_j=-a_{j-2}/[j(j+2\ell+1)]$. The singular branch has $a_j=-a_{j-2}/[j(j-2\ell-1)]$ except at $j=2\ell+1$. That resonant equation is compatible because its earlier odd coefficient vanishes; the newly free coefficient adds a multiple of the regular solution. Setting it to zero gives a pure even series times $x^{-\ell-1}$, independent of the regular branch, with no logarithmic term. For $\ell=0$ the resonance occurs already at $j=1$.

The normalization $a_0=2^\ell\ell!/(2\ell+1)!$ on the regular branch gives the [Spherical Bessel function](#spherical-bessel-function)

$$
j_\ell(x)=2^\ell x^\ell\sum_{s=0}^\infty\frac{(-1)^s(s+\ell)!}{s!(2s+2\ell+1)!}x^{2s}.
$$

In particular $j_0(x)=\sin x/x$, with removable value one at zero.

### Logarithmic spherical Bessel square integral

↑ **Parent:** [Spherical Bessel function](#spherical-bessel-function)

For integer $\ell\geq1$, put $I_\ell=\int_0^\infty j_\ell(x)^2\,dx/x$ and $J_\ell=\int_0^\infty j_\ell(x)j_{\ell-1}(x)\,dx$. Integrating $j_\ell'=j_{\ell-1}-(\ell+1)j_\ell/x$ gives $J_\ell=(\ell+1)I_\ell$. For $\ell>1$, integrating $j_{\ell-1}'=(\ell-1)j_{\ell-1}/x-j_\ell$ also gives $J_\ell=(\ell-1)I_{\ell-1}$. For $\ell=1$, the boundary values $j_0(0)=1$ and $j_0(\infty)=0$ give $J_1=1/2$, hence $I_1=1/4$. The recurrence proves the displayed identity. The integral without the square is different; for example $\int_0^\infty j_1(x)\,dx/x=\pi/4$.

### Spherical Hankel function

↑ **Parent:** [Spherical Bessel function](#spherical-bessel-function)

These combinations of [Spherical Bessel functions](#spherical-bessel-function) solve the radial [Helmholtz equation](partial-differential-equation.md#helmholtz-equation). For time dependence $e^{-i\omega t}$, $h_n^{(1)}(kr)$ is outgoing and $h_n^{(2)}(kr)$ incoming. At fixed order and large argument, $h_n^{(1)}(t)\sim(-i)^{n+1}e^{it}/t$. Their recurrence is $h_{n+1}=(2n+1)h_n/t-h_{n-1}$.

#### Fixed-argument growth of spherical Hankel functions

↑ **Parent:** [Spherical Hankel function](#spherical-hankel-function)

For fixed $t>0$ and large integer order, $y_n(t)\sim-(2n-1)!!/t^{n+1}$ while $j_n(t)$ is negligible. Stirling's formula gives $(2n-1)!!=(2n)!/(2^nn!)\sim\sqrt2(2n/e)^n$, proving the displayed asymptotic. In particular its magnitude is bounded above and below by constant multiples of $(2n/(et))^n$. This two-sided comparison is stronger than a one-sided big-O estimate and is what converts a finite spherical trace norm into a weighted condition on far-field coefficients.

### Spherical Bessel product integral

↑ **Parent:** [Spherical Bessel function](#spherical-bessel-function)

For integer $\ell\geq0$ and $r,R>0$, $r_<=\min(r,R)$ and $r_>=\max(r,R)$. A proof compares the [multipole expansion](electrostatics.md#electric-multipole-expansion) of $1/|\mathbf r-\mathbf R|$ with its [Fourier transform of inverse distance in three dimensions](fourier-transform.md#fourier-transform-of-inverse-distance-in-three-dimensions). Applying the [Rayleigh plane-wave expansion](analysis.md#rayleigh-plane-wave-expansion) to the Fourier representation gives coefficient $8\int_0^\infty j_\ell(kr)j_\ell(kR)\,dk$ multiplying $Y_{\ell m}(\hat r)Y_{\ell m}^*(\hat R)$; the Coulomb multipole coefficient is $4\pi r_<^\ell/[(2\ell+1)r_>^{\ell+1}]$. Equating the coefficients proves the identity. The powers also match continuously at $r=R$.

## Bessel function of the first kind

↑ **Parent:** [Bessel function](bessel-function.md)

The Bessel function of the first kind $J_\nu$ is the solution of the [Bessel differential equation](#bessel-differential-equation) selected by its regular power-series behavior at the origin. For $\operatorname{Re}\nu>-1/2$, it has the Poisson integral representation

$$
J_\nu(z)=\frac{(z/2)^\nu}{\Gamma(\nu+1/2)\sqrt\pi}
\int_{-1}^{1}e^{izt}(1-t^2)^{\nu-1/2}\,dt.
$$

### Integer-order Bessel reflection identity

↑ **Parent:** [Bessel function of the first kind](#bessel-function-of-the-first-kind)

For integer $m\geq0$, $J_{-m}(z)=(-1)^mJ_m(z)$. Thus negative integer orders remain regular at zero. The familiar $J_m(z)\sim z^m/(2^mm!)$ formula is used for nonnegative order; a negative factorial is not a valid continuation.

### Bessel functions of order one half

↑ **Parent:** [Bessel function of the first kind](#bessel-function-of-the-first-kind)

For $x>0$, the [Bessel differential equation](#bessel-differential-equation) of order $1/2$ has independent solutions $x^{-1/2}\sin x$ and $x^{-1/2}\cos x$. Substituting $y=x^{-1/2}u$ reduces it to $u''+u=0$. The normalization of the [Bessel function of the first kind](#bessel-function-of-the-first-kind) gives the displayed formulas for orders $1/2$ and $-1/2$. The [Frobenius method](complex-analysis.md#frobenius-method) obtains the same pair from exponents $1/2$ and $-1/2$: their even-coefficient series reduce to the sine and cosine [power series](sequence-and-series.md#power-series). In the negative-exponent recurrence, the free coefficient at the next exponent can add the positive-exponent solution, an example of an [undetermined coefficient at Frobenius resonance](complex-analysis.md#undetermined-coefficient-at-frobenius-resonance).

### Fourier transform of the Bessel function J0

↑ **Parent:** [Bessel function of the first kind](#bessel-function-of-the-first-kind)

With the [Fourier transform](fourier-transform.md) convention $\widehat f(\omega)=\int_{\mathbb R}f(t)e^{-i\omega t}\,dt$, the regular order-zero [Bessel function of the first kind](#bessel-function-of-the-first-kind) has the [tempered distribution](fourier-analysis.md#tempered-distribution) transform

$$
\boxed{\widehat{J_0}(\omega)=\frac{2\,\mathbf1_{(-1,1)}(\omega)}{\sqrt{1-\omega^2}}.}
$$

The density is [integrable](measure-theory.md#integrability) despite its endpoint singularities. [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) gives the equivalent [integral representation](integral.md#integral-representation)

$$
J_0(t)=\frac1\pi\int_{-1}^{1}\frac{e^{it\omega}}{\sqrt{1-\omega^2}}\,d\omega=\frac1\pi\int_0^\pi\cos(t\cos\theta)\,d\theta.
$$

The second formula follows by $\omega=\cos\theta$ and cancellation of the odd imaginary part. It is the standard real integral representation of $J_0$.[NIST Digital Library of Mathematical Functions, equation 10.9.1](https://dlmf.nist.gov/10.9.E1)

Indeed, transforming the order-zero [Bessel differential equation](#bessel-differential-equation) $t y''+y'+ty=0$ gives $(1-\omega^2)Y'-\omega Y=0$. Inside $(-1,1)$, its solutions are $C(1-\omega^2)^{-1/2}$. The compactly supported choice also solves the equation as a [distribution](distribution-theory.md#distribution-mathematical-analysis): rewrite it as $[(1-\omega^2)Y]'+\omega Y=0$, and observe that $(1-\omega^2)Y=C\sqrt{1-\omega^2}\,\mathbf1_{(-1,1)}$ is continuous and zero at the two endpoints. Its [distributional derivative](distribution-theory.md#distributional-derivative) has no endpoint [Dirac delta](distribution-theory.md#dirac-delta-function) terms. The inverse is regular at $t=0$, and $y(0)=1$ fixes $C=2$.

The transformed equation alone also allows separate constants on $\omega<-1$ and $\omega>1$. Selecting the compactly supported density amounts to selecting the solution regular at the origin, rather than every possible singular solution of the [Bessel differential equation](#bessel-differential-equation).

### Jacobi-Anger expansion

↑ **Parent:** [Bessel function of the first kind](#bessel-function-of-the-first-kind)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi–Anger_expansion)

A [Fourier series](fourier-series.md) expansion of a sinusoidally modulated complex [wave phase](wave.md#phase-waves) in [Bessel functions of the first kind](#bessel-function-of-the-first-kind).

#### Bessel second-moment identity

↑ **Parent:** [Jacobi-Anger expansion](#jacobi-anger-expansion)

For real $z$, the [probabilities](probability-theory.md#probability) $J_m(z)^2$ over integer angular-momentum modes satisfy $\sum_m m^2J_m(z)^2=z^2/2$. Differentiate the unit-modulus function $e^{iz\cos\theta}$ and use Parseval to obtain the identity; its zero first moment follows from the symmetry of opposite orders.

### Quartic truncation of the Bessel function J0

↑ **Parent:** [Bessel function of the first kind](#bessel-function-of-the-first-kind)

The regular power series has $J_0(\rho)=1-\rho^2/4+\rho^4/64-\cdots$. Its quartic truncation has a double zero at $\rho=\sqrt8$, giving a rough disc-well energy estimate $4\hbar^2/(\mu a^2)$. A truncation zero is not an exact Bessel zero or a rigorous eigenvalue bound. The double-root behavior particularly warns against treating a low-order local expansion as accurate far from its center.

### Debye asymptotic for oscillatory Bessel functions

↑ **Parent:** [Bessel function of the first kind](#bessel-function-of-the-first-kind)

For fixed $0<\alpha<\pi/2$, the [Bessel function of the first kind](#bessel-function-of-the-first-kind) has an interior nondegenerate [stationary point](calculus-of-variations.md#stationary-point) in its cosine integral. The [stationary phase method](analysis.md#stationary-phase-method) gives the displayed oscillatory leading term and an additive $O(n^{-3/2})$ remainder. The approximation loses uniformity near $\alpha=0$, where the [stationary point](calculus-of-variations.md#stationary-point) reaches the endpoint and the curvature vanishes. For negative integer-order arguments, parity supplies a factor $(-1)^n$.

### Large-argument asymptotic expansion of the Bessel function of the first kind

↑ **Parent:** [Bessel function of the first kind](#bessel-function-of-the-first-kind)

For fixed $\nu$, put

$$
\chi=z-\frac{\pi\nu}{2}-\frac\pi4,
\qquad
a_k(\nu)=\frac{\prod_{j=1}^k\left(4\nu^2-(2j-1)^2\right)}{k!8^k},
\qquad a_0=1.
$$

Then

$$
J_\nu(z)\sim\sqrt{\frac2{\pi z}}
\left[
\cos\chi\sum_{m=0}^{\infty}\frac{(-1)^ma_{2m}(\nu)}{z^{2m}}
-\sin\chi\sum_{m=0}^{\infty}\frac{(-1)^ma_{2m+1}(\nu)}{z^{2m+1}}
\right]
$$

as $|z|\to\infty$, uniformly for $|\arg z|\leq\pi-\delta$. In particular,

$$
J_\nu(z)\sim\sqrt{\frac2{\pi z}}
\left[
\cos\chi-\frac{4\nu^2-1}{8z}\sin\chi
-\frac{(4\nu^2-1)(4\nu^2-9)}{2!(8z)^2}\cos\chi+\cdots
\right].
$$

## Bessel differential equation

↑ **Parent:** [Bessel function](bessel-function.md)

The Bessel differential equation of order $\nu$ is

$$
x^2y''+xy'+(x^2-\nu^2)y=0.
$$

For noninteger $\nu$, $J_\nu$ and $J_{-\nu}$ form a linearly independent pair of solutions.

### Frobenius series for Bessel functions

↑ **Parent:** [Bessel differential equation](#bessel-differential-equation)

For the [Bessel differential equation](#bessel-differential-equation) $x^2y''+xy'+(x^2-\nu^2)y=0$, substitute $y=x^s\sum_{n\geq0}a_nx^n$. The [indicial equation](linear-ordinary-differential-equation.md#indicial-equation) is $s^2-\nu^2=0$, and coefficients obey $[(n+s)^2-\nu^2]a_n=-a_{n-2}$. For $s=\nu\geq0$, $a_1=0$ and all odd coefficients vanish. Iteration gives $a_{2m}=(-1)^ma_0\Gamma(\nu+1)/[4^mm!\Gamma(m+\nu+1)]$. Choosing $a_0=1/[2^\nu\Gamma(\nu+1)]$ gives the [Bessel function of the first kind](#bessel-function-of-the-first-kind) $J_\nu$.

For noninteger $\nu$, choosing the even-power series with $s=-\nu$ replaces $m+\nu$ by $m-\nu$ and yields $J_{-\nu}$ with its standard normalization. These solutions are independent. For integer $\nu\geq0$, the first solution has coefficients $(-1)^m/[2^{2m+\nu}m!(m+\nu)!]$ and defines an entire function: the term ratio tends to zero at every finite complex argument. For noninteger order, the even analytic series converges everywhere, while the prefactor $x^{\pm\nu}$ requires a branch off the positive real axis.

### Sturm-Liouville formulation with Bessel order as eigenvalue

↑ **Parent:** [Bessel differential equation](#bessel-differential-equation)

For fixed $\beta$, move the order term of the [Bessel equation](#bessel-differential-equation) to the right: $x^2y''+xy'+\beta^2x^2y=n^2y$. The [integrating factor](linear-ordinary-differential-equation.md#integrating-factor) for its leading differential expression is $1/x$, giving the displayed [Sturm-Liouville theory](sturm-liouville-theory.md) form with coefficient $p=x$, potential $q=\beta^2x$, weight $w=1/x$ and [eigenvalue](linear-operator-theory.md#eigenvalue) $n^2$. The origin is a singular endpoint. The [integrating factor](linear-ordinary-differential-equation.md#integrating-factor) must be normalized from a positive reference point; its defining logarithmic [integral](integral.md) cannot literally start at zero. [Boundary conditions](differential-equation.md#boundary-condition) are needed before this differential identity becomes a specified self-adjoint spectral problem.

## Modified Bessel function

↑ **Parent:** [Bessel function](bessel-function.md)

The modified Bessel equation of order zero is

$$
z^2y''+zy'-z^2y=0.
$$

Its solution regular at zero and normalized by $I_0(0)=1$ is the modified Bessel function $I_0$.

### Large-argument asymptotic expansion of a modified Bessel function

↑ **Parent:** [Modified Bessel function](#modified-bessel-function)

For fixed real $\nu$ as $z\to+\infty$, the [Modified Bessel function of the first kind](#modified-bessel-function-of-the-first-kind) and [Modified Bessel function of the second kind](#modified-bessel-function-of-the-second-kind) have [asymptotic expansions](asymptotic-expansion.md)

$$
I_\nu(z)\sim\frac{e^z}{\sqrt{2\pi z}}\sum_{j=0}^\infty\frac{(-1)^ja_j(\nu)}{z^j},\qquad
K_\nu(z)\sim\sqrt{\frac\pi{2z}}e^{-z}\sum_{j=0}^\infty\frac{a_j(\nu)}{z^j},\qquad
a_0=1,\quad a_{j+1}=\frac{4\nu^2-(2j+1)^2}{8(j+1)}a_j.
$$

The expansion and its error bounds establish actual growing and decaying solutions, beyond formal matching of a [differential equation](differential-equation.md). These formulas are documented in [NIST DLMF, equations 10.40.1–2](https://dlmf.nist.gov/10.40).

### Modified Bessel function of the first kind

↑ **Parent:** [Modified Bessel function](#modified-bessel-function)

The solution of the [Modified Bessel differential equation](#modified-bessel-differential-equation) with [power series](sequence-and-series.md#power-series) $I_\nu(z)=\sum_{j\geq0}(z/2)^{2j+\nu}/[j!\Gamma(j+\nu+1)]$, interpreted through the reciprocal [gamma function](complex-analysis.md#gamma-function) at its zeros. For fixed real order it grows exponentially along the positive real axis.

### Modified Bessel differential equation

↑ **Parent:** [Modified Bessel function](#modified-bessel-function)

The [differential equation](differential-equation.md) defining [modified Bessel functions](#modified-bessel-function) of order $\nu$. For real fixed $\nu$ and positive $z$, its independent standard solutions are $I_\nu(z)$ and $K_\nu(z)$.

### Modified Bessel function of the second kind

↑ **Parent:** [Modified Bessel function](#modified-bessel-function)

The modified Bessel function of the second kind is the solution $K_\nu(x)$ of the modified Bessel differential equation that decays exponentially as $x\to+\infty$.

#### Fourier transform of the modified Bessel function K0

↑ **Parent:** [Modified Bessel function of the second kind](#modified-bessel-function-of-the-second-kind)

The [integral representation of the modified Bessel function of the second kind](#integral-representation-of-the-modified-bessel-function-of-the-second-kind) gives $K_0(x)=\int_0^\infty e^{-x\cosh t}\,dt$ for $x>0$. Taking the [Fourier transform](fourier-transform.md) of the even continuation and setting $u=\sinh t$ gives $2\int_0^\infty(1+k^2+u^2)^{-1}du=\pi/\sqrt{1+k^2}$. The large-[wavenumber](wave-equation.md#wavenumber) terms $\pi/|k|-\pi/(2|k|^3)$ are also obtained from the local [logarithmic singularity](analysis.md#logarithmic-singularity) $-\log|x|-(x^2/4)\log|x|$ using the [Fourier transform of the absolute logarithm](fourier-analysis.md#fourier-transform-of-the-absolute-logarithm).

#### Integral representation of the modified Bessel function of the second kind

↑ **Parent:** [Modified Bessel function of the second kind](#modified-bessel-function-of-the-second-kind)

For real $x>0$ and $\nu$, one useful representation is

$$
K_\nu(x)=\frac12\int_{-\infty}^{\infty}e^{-x\cosh t+\nu t}\,dt.
$$

It turns large-order asymptotics into a [Laplace integral](asymptotic-expansion.md#laplace-integral) with a moving maximum.

#### Large-order asymptotic of the modified Bessel function of the second kind

↑ **Parent:** [Modified Bessel function of the second kind](#modified-bessel-function-of-the-second-kind)

For fixed $x>0$,

$$
K_\nu(x)\sim\left(\frac\pi{2\nu}\right)^{1/2}
\left(\frac{2\nu}{ex}\right)^\nu
$$

as $\nu\to+\infty$. Applying [Laplace's method](asymptotic-expansion.md#laplace-s-method) to the [integral representation of the modified Bessel function of the second kind](#integral-representation-of-the-modified-bessel-function-of-the-second-kind) proves the formula.

### Laplace integral method for a differential equation

↑ **Parent:** [Modified Bessel function](#modified-bessel-function)

Laplace's integral method seeks $y(z)=\int_Ce^{zt}f(t)\,dt$. Substitution into the differential equation and integration by parts transfer multiplication by $z$ into differentiation with respect to $t$, producing a first-order equation for $f$ and endpoint conditions for $C$.

#### Laplace integral solution of a singular third-order equation

↑ **Parent:** [Laplace integral method for a differential equation](#laplace-integral-method-for-a-differential-equation)

For $x>0$, substituting $y(x)=\int_\gamma e^{xt}f(t)\,dt$ into $xy^{(3)}+2y=0$ and integrating by parts gives

$$
[e^{xt}t^3f(t)]_{\partial\gamma}
+\int_\gamma e^{xt}\{2f-(t^3f)'\}\,dt=0.
$$

The amplitude equation $(t^3f)'=2f$ has solution $f(t)=Ct^{-3}e^{-1/t^2}$. On $\gamma=(-\infty,0)$ both endpoint terms vanish, and hence

$$
y(x)=C\int_{-\infty}^0e^{xt-t^{-2}}t^{-3}\,dt
=C_1\int_0^\infty u e^{-u^2-x/u}\,du.
$$

#### Laguerre contour-integral amplitude

↑ **Parent:** [Laplace integral method for a differential equation](#laplace-integral-method-for-a-differential-equation)

For the Laguerre equation

$$
zy''+(1-z)y'+\lambda y=0,
$$

the ansatz $y=\int_\gamma e^{zt}f(t)\,dt$ gives

$$
f(t)=t^{-\lambda-1}(t-1)^\lambda.
$$

The contour must make the endpoint contribution

$$
\left[e^{zt}t^{-\lambda}(t-1)^{\lambda+1}\right]_{\partial\gamma}
$$

vanish.

##### Finite Laguerre contour solution

↑ **Parent:** [Laguerre contour-integral amplitude](#laguerre-contour-integral-amplitude)

A finite contour based at an integrable branch point, or a closed contour around an integer-order pole, gives a solution analytic at $z=0$. It is therefore a constant multiple of the unique Frobenius power-series solution there.

###### Integer-parameter Laguerre contour residues

↑ **Parent:** [Finite Laguerre contour solution](#finite-laguerre-contour-solution)

For $\lambda=N\geq0$, the amplitude $(t-1)^N/t^{N+1}$ has a pole at zero whose contour residue is a degree-$N$ Laguerre polynomial in $z$. For $\lambda=-m<0$, the amplitude $t^{m-1}/(t-1)^m$ has a pole at one whose residue is $e^z$ times a polynomial of degree $m-1$.

#### Real integral representation of the modified Bessel function I0

↑ **Parent:** [Laplace integral method for a differential equation](#laplace-integral-method-for-a-differential-equation)

The normalized order-zero function has the representation

$$
I_0(z)=\frac1\pi\int_{-1}^1\frac{e^{zs}}{\sqrt{1-s^2}}\,ds.
$$

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (19)

- [Abel regularization of an oscillatory integral](distribution-theory.md#abel-regularization-of-an-oscillatory-integral)
- [Bessel density modes during exponential expansion](linear-cosmological-density-perturbation.md#bessel-density-modes-during-exponential-expansion)
- [Bessel transition for an exponentially decaying oscillator](analysis.md#bessel-transition-for-an-exponentially-decaying-oscillator)
- [Focal ratio](optical-instrument.md#focal-ratio)
- [Hankel representation of thin-disk gravity](astrophysical-disk.md#hankel-representation-of-thin-disk-gravity)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-69.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-74.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-66.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80.md#4/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-59.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-336.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1.md#14b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2.md#16c/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-314.md#2/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-355.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1.md#6/a/ii/solution)
- [Solution](past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2019/paper-ne1.md#2/c/i/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022.md#section-a/3/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2.md#section-d/d12/solution)
