# Paper 335

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_335.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_335.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the time convention $e^{-i\omega t}$. The free-space [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation), with $\psi=e^{ikx}E$, gives the exact reduced equation

$$
E_{xx}+2ikE_x+E_{zz}=0.
$$

For a forward [plane wave](../../../quantum-mechanics.md#plane-wave) at angle $\alpha$, $E_x=O(k\alpha^2E)$ and $E_{zz}=O(k^2\alpha^2E)$, whereas $E_{xx}=O(k^2\alpha^4E)$. Thus the [paraxial approximation](../../../partial-differential-equation.md#paraxial-approximation) neglects $E_{xx}$ relative to $2ikE_x$. **The reduced field satisfies the [parabolic wave equation](../../../partial-differential-equation.md#parabolic-wave-equation)**

$$
\boxed{2ikE_x+E_{zz}=0,\qquad E_x=\frac{i}{2k}E_{zz}.}
$$

With the [Fourier transform](../../../analysis.md#fourier-transform) convention used below and its inverse, this becomes an [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) for each transverse [wavenumber](../../../wave-equation.md#wavenumber):

$$
\partial_x\widehat E(x,\nu)=-\frac{i\nu^2}{2k}\widehat E(x,\nu),\qquad
\boxed{\widehat E(x,\nu)=e^{-i\nu^2x/(2k)}\widehat E(0,\nu).}
$$

Consequently the initial-value solution is

$$
E(x,z)=\int_{\mathbb R}\widehat E(0,\nu)e^{i\nu z-i\nu^2x/(2k)}\,d\nu.
$$

Equivalently, evaluating the oscillatory [Gaussian integral](../../../calculus.md#gaussian-integral) gives the [one-dimensional transverse Fresnel propagation](../../../partial-differential-equation.md#one-dimensional-transverse-fresnel-propagation) formula

$$
\boxed{E(x,z)=\sqrt{\frac{k}{2\pi ix}}\int_{\mathbb R}
\exp\!\left(\frac{ik(z-z')^2}{2x}\right)E(0,z')\,dz',\qquad x>0.}
$$

The square-root branch has $\sqrt{1/i}=e^{-i\pi/4}$. The formula is an [oscillatory integral](../../../distribution-theory.md#oscillatory-integral) for general data, or the [Fresnel propagator](../../../partial-differential-equation.md#fresnel-propagator) acting on [square-integrable functions](../../../measure-theory.md#square-integrable-function). It approaches the initial field as $x\downarrow0$. A [plane wave](../../../quantum-mechanics.md#plane-wave) has transverse [wavenumber](../../../wave-equation.md#wavenumber) $\nu=k\sin\alpha$; the reduced axial phase $-\nu^2x/(2k)$ agrees with $k(\cos\alpha-1)x$ through order $\alpha^2$. This also checks the sign. The [paraxial approximation](../../../partial-differential-equation.md#paraxial-approximation) applies to $|\nu|\ll k$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $\beta=k\xi\mu$. The [random phase screen](../../../partial-differential-equation.md#random-phase-screen) produces

$$
E(0,z)=e^{i\beta W(z)},\qquad
\widehat E(x,\nu)=e^{-i\nu^2x/(2k)}\widehat E(0,\nu).
$$

Interpret the normality assumption as a jointly [Gaussian process](../../../stochastic-process.md#gaussian-process), not merely Gaussian one-point [marginal distributions](../../../probability-theory.md#marginal-distribution). Write its normalized [autocorrelation](../../../time-series.md#autocorrelation) as $\rho(\zeta)=\langle W(z+\zeta)W(z)\rangle$. The difference $W(z+\zeta)-W(z)$ is a zero-mean [Gaussian random variable](../../../probability-theory.md#gaussian-random-variable) with [variance](../../../variance.md) $2(1-\rho(\zeta))$. Its [characteristic function](../../../probability-theory.md#characteristic-function) therefore gives the [Gaussian phase-screen correlation](../../../partial-differential-equation.md#gaussian-phase-screen-correlation)

$$
\boxed{C_E(\zeta):=\langle E(0,z+\zeta)\overline{E(0,z)}\rangle
=\exp\{-\beta^2[1-\rho(\zeta)]\}.}
$$

Without joint Gaussianity the [autocorrelation](../../../time-series.md#autocorrelation) alone does not determine this expectation.

For an acoustic pressure amplitude $\psi$, with background mass density $\rho_0$, the time-averaged [acoustic energy flux](../../../continuum-mechanics.md#acoustic-energy-flux) is

$$
I_x=\frac{1}{2\rho_0\omega}\operatorname{Im}(\overline\psi\,\partial_x\psi).
$$

An acoustic potential convention changes the dimensional prefactor. The physical field includes the carrier $e^{ikx}$: a transverse [Fourier transform](../../../analysis.md#fourier-transform) mode has axial [wavenumber](../../../wave-equation.md#wavenumber) $\kappa_\nu=k-\nu^2/(2k)$ in the [parabolic wave equation](../../../partial-differential-equation.md#parabolic-wave-equation). Thus its [spectral acoustic flux](../../../continuum-mechanics.md#spectral-acoustic-flux) is proportional to $\kappa_\nu|\widehat E(x,\nu)|^2$, or to $k|\widehat E(x,\nu)|^2$ at leading paraxial order. Differentiating the reduced field alone would omit the carrier contribution.

The infinite stationary illumination has a [spectral measure of a stationary random field](../../../time-series.md#spectral-measure-of-a-stationary-random-field), rather than a finite ordinary value of $\langle|\widehat E|^2\rangle$ at each $\nu$. To specify the normalization, truncate the screen to an aperture of length $L$, propagate this truncated initial field, and set

$$
\widehat E_L(0,\nu)=\frac1{2\pi}\int_{-L/2}^{L/2}E(0,z)e^{-i\nu z}\,dz.
$$

The propagation multiplier has modulus one. Using the [Gaussian phase-screen correlation](../../../partial-differential-equation.md#gaussian-phase-screen-correlation) and the overlap of the two aperture intervals gives

$$
\boxed{\langle|\widehat E_L(x,\nu)|^2\rangle
=\frac1{4\pi^2}\int_{-L}^{L}(L-|\zeta|)
e^{-\beta^2[1-\rho(\zeta)]}e^{-i\nu\zeta}\,d\zeta,\qquad x>0.}
$$

Multiplication by $\kappa_\nu/(2\rho_0\omega)$ gives the ensemble-averaged pressure-normalized modal [acoustic energy flux](../../../continuum-mechanics.md#acoustic-energy-flux) for this finite-aperture convention.

The [infinite-aperture spectral normalization](../../../time-series.md#infinite-aperture-spectral-normalization) consistent with the specified [Fourier transform](../../../analysis.md#fourier-transform) is

$$
\boxed{S_E(\nu)=\lim_{L\to\infty}\frac{2\pi}{L}
\langle|\widehat E_L(x,\nu)|^2\rangle
=\frac1{2\pi}\int_{\mathbb R}e^{-\beta^2[1-\rho(\zeta)]}e^{-i\nu\zeta}\,d\zeta.}
$$

The integral and limit are understood as [spectral measures of a stationary random field](../../../time-series.md#spectral-measure-of-a-stationary-random-field) when necessary. By [Parseval's identity](../../../fourier-analysis.md#parseval-identity), this is power per unit transverse length: $\int_{\mathbb R}S_E(d\nu)=C_E(0)=1$. **The ensemble-averaged axial [spectral acoustic flux](../../../continuum-mechanics.md#spectral-acoustic-flux) is independent of $x$:**

$$
\boxed{\frac{d\langle I_x\rangle}{d\nu}
=\frac{\kappa_\nu}{2\rho_0\omega}S_E(\nu)
\simeq I_{\rm inc}S_E(\nu),\qquad I_{\rm inc}=\frac{k}{2\rho_0\omega}.}
$$

Here the notation includes [Dirac delta distributions](../../../distribution-theory.md#dirac-delta-function) in the [spectral measure of a stationary random field](../../../time-series.md#spectral-measure-of-a-stationary-random-field); the leading-order total flux is $I_{\rm inc}$. The $\kappa_\nu$ correction is meaningful within $|\nu|\ll k$, the range of the [paraxial approximation](../../../partial-differential-equation.md#paraxial-approximation).

If $\rho(\zeta)\to0$ and $e^{\beta^2\rho(\zeta)}-1$ is integrable, the [stationary phase-screen power spectrum](../../../partial-differential-equation.md#stationary-phase-screen-power-spectrum) separates into [coherent and diffuse wave fields](../../../partial-differential-equation.md#coherent-and-diffuse-wave-fields):

$$
S_E(\nu)=e^{-\beta^2}\delta(\nu)
+\frac{e^{-\beta^2}}{2\pi}\int_{\mathbb R}
[e^{\beta^2\rho(\zeta)}-1]e^{-i\nu\zeta}\,d\zeta.
$$

The coherent fraction is $e^{-\beta^2}$ and the diffuse fraction is $1-e^{-\beta^2}$. If additionally $|\beta|\ll1$, the [stationary phase-screen power spectrum](../../../partial-differential-equation.md#stationary-phase-screen-power-spectrum) is $(1-\beta^2)\delta+\beta^2\widehat\rho+O(\beta^4)$ with the same [Fourier transform](../../../analysis.md#fourier-transform) convention. Small $\mu$ alone does not imply small accumulated phase $k\xi\mu$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At each point the [Gaussian process](../../../stochastic-process.md#gaussian-process) has a standard normal [marginal distribution](../../../probability-theory.md#marginal-distribution). Its [characteristic function](../../../probability-theory.md#characteristic-function) gives the coherent screen field

$$
m=\langle e^{i\beta W(z)}\rangle=e^{-\beta^2/2}.
$$

It is constant in $z$, so its [Fourier transform](../../../analysis.md#fourier-transform) is $m\delta(\nu)$. Applying the [Fresnel propagator](../../../partial-differential-equation.md#fresnel-propagator) to this zero-transverse-[wavenumber](../../../wave-equation.md#wavenumber) component gives **the ensemble-averaged reduced spectrum**

$$
\boxed{\langle\widehat E(x,\nu)\rangle
=e^{-i\nu^2x/(2k)}e^{-\beta^2/2}\delta(\nu)
=e^{-\beta^2/2}\delta(\nu).}
$$

Thus the reduced mean is independent of $x$. The physical mean $\langle\psi(x,z)\rangle=e^{ikx}e^{-\beta^2/2}$ still has its carrier phase. The [coherent attenuation by a Gaussian phase screen](../../../partial-differential-equation.md#coherent-attenuation-by-a-gaussian-phase-screen) takes place at the screen, with no further coherent attenuation in homogeneous space.

The full [spectral acoustic flux](../../../continuum-mechanics.md#spectral-acoustic-flux) depends on the second moment, not the square of this mean. For a [stationary process](../../../time-series.md#stationary-process), the generalized cross-spectral correlation is

$$
\langle\widehat E(x,\nu)\overline{\widehat E(x,\nu')}\rangle
=\delta(\nu-\nu')S_E(\nu).
$$

Indeed its propagation factors cancel on $\nu=\nu'$. This explains why the ensemble-averaged [spectral acoustic flux](../../../continuum-mechanics.md#spectral-acoustic-flux) in (b) is also independent of $x$, even for nonzero transverse [wavenumbers](../../../wave-equation.md#wavenumber) whose individual complex amplitudes change phase. The coherent atom has weight $|m|^2=e^{-\beta^2}$; the full [stationary phase-screen power spectrum](../../../partial-differential-equation.md#stationary-phase-screen-power-spectrum) also contains fluctuations. Under the decay assumptions in (b), their integrated weight is $1-e^{-\beta^2}$. One must use these weights in a [spectral measure of a stationary random field](../../../time-series.md#spectral-measure-of-a-stationary-random-field), rather than square a [Dirac delta distribution](../../../distribution-theory.md#dirac-delta-function). A phase-only screen preserves the leading-order total [acoustic energy flux](../../../continuum-mechanics.md#acoustic-energy-flux), although it reduces its coherent part.

## 2

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Choose the time convention $e^{-i\omega t}$ and the outgoing [Sommerfeld radiation condition](../../../inverse-problem.md#sommerfeld-radiation-condition). Define the [outgoing Green function for the three-dimensional Helmholtz equation](../../../partial-differential-equation.md#outgoing-green-function-for-the-three-dimensional-helmholtz-equation) by

$$
G_k(\mathbf r,\mathbf r')=\frac{e^{ik|\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|},\qquad
(\Delta_{\mathbf r}+k^2)G_k=-\delta(\mathbf r-\mathbf r').
$$

Away from $\mathbf r'$ it solves the homogeneous [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation). Integrating its radial derivative over a small sphere gives $-1$ in the zero-radius limit, verifying the sign of the [Dirac delta distribution](../../../distribution-theory.md#dirac-delta-function). At infinity it satisfies $(\partial_R-ik)G_k=o(R^{-1})$.

**For the positive source on the right-hand side, the outgoing field is**

$$
\boxed{\psi(\mathbf r,k)=-\int_A
\frac{e^{ik|\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|}
Q(\mathbf r')\,d^3\mathbf r'.}
$$

Applying the [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) operator under this source representation gives $Q$. The minus sign is essential with the displayed [Green function](../../../analysis.md#green-s-function) convention; defining the [Green function](../../../analysis.md#green-s-function) to satisfy $LG=+\delta$ instead would absorb it. Here $A$ is the solid ball of radius $r_0$, as required by the volume source equation. Its finite volume and $Q\in L^2(A)$ make $Q$ integrable. The [Sommerfeld radiation condition](../../../inverse-problem.md#sommerfeld-radiation-condition) specifies the outgoing solution; without it one could add a homogeneous [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) solution.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Write $\mathbf r=R\boldsymbol\theta$, $|\boldsymbol\theta|=1$. Uniformly for $\mathbf r'$ in the source ball,

$$
|\mathbf r-\mathbf r'|=R-\boldsymbol\theta\cdot\mathbf r'+O(r_0^2/R),\qquad
|\mathbf r-\mathbf r'|^{-1}=R^{-1}+O(r_0/R^2).
$$

For fixed $k$ and $r_0$, the [outgoing Green function for the three-dimensional Helmholtz equation](../../../partial-differential-equation.md#outgoing-green-function-for-the-three-dimensional-helmholtz-equation) therefore has the [far-field approximation for an outgoing source](../../../inverse-problem.md#far-field-approximation-for-an-outgoing-source)

$$
G_k(R\boldsymbol\theta,\mathbf r')
=\frac{e^{ikR}}{4\pi R}e^{-ik\boldsymbol\theta\cdot\mathbf r'}+O(R^{-2}).
$$

Substitution into the source integral yields

$$
\psi(R\boldsymbol\theta,k)=\frac{e^{ikR}}R f_\infty(\boldsymbol\theta,k)+O(R^{-2}),\qquad
\boxed{f_\infty(\boldsymbol\theta,k)
=-\frac1{4\pi}\int_A Q(\mathbf r')e^{-ik\boldsymbol\theta\cdot\mathbf r'}\,d^3\mathbf r'.}
$$

Thus the [source-to-far-field operator at fixed frequency](../../../physics.md#source-to-far-field-operator-at-fixed-frequency) is

$$
\boxed{T:L^2(A)\longrightarrow L^2(S_1),\qquad
(TQ)(\boldsymbol\theta)=-\frac1{4\pi}\int_AQ(\mathbf r')e^{-ik\boldsymbol\theta\cdot\mathbf r'}\,d^3\mathbf r'.}
$$

It samples the [Fourier transform](../../../analysis.md#fourier-transform) of the source on the sphere of radius $k$. Its square-integrable kernel makes it a [Hilbert-Schmidt operator](../../../compact-operator.md#hilbert-schmidt-operator), hence a [compact operator](../../../compact-operator.md). In fact

$$
\|T\|_{\rm HS}^2=\frac{|A||S_1|}{16\pi^2}
=\frac{|A|}{4\pi}=\frac{r_0^3}{3}.
$$

Use complex [inner products](../../../linear-algebra.md#inner-product) linear in the first argument: $(f,g)=\int f\overline g$. Interchanging the volume and surface integrals gives

$$
(TQ,g)_{L^2(S_1)}
=\int_A Q(\mathbf r')\overline{\left[
-\frac1{4\pi}\int_{S_1}g(\boldsymbol\theta)e^{ik\boldsymbol\theta\cdot\mathbf r'}\,dS(\boldsymbol\theta)\right]}\,d^3\mathbf r'.
$$

Hence **the [adjoint source-to-far-field operator](../../../physics.md#adjoint-source-to-far-field-operator) is**

$$
\boxed{(T^*g)(\mathbf r')=-\frac1{4\pi}\int_{S_1}
g(\boldsymbol\theta)e^{ik\boldsymbol\theta\cdot\mathbf r'}\,dS(\boldsymbol\theta).}
$$

This is a normalized [Herglotz wave function](../../../inverse-problem.md#herglotz-wave-function); the change in exponential sign comes from the [complex conjugation](../../../complex-analysis.md#complex-conjugation) in the [adjoint operator](../../../hilbert-space.md#adjoint-operator).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Seeking a [least-squares solution of a linear inverse problem](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) for the [acoustic inverse source problem](../../../physics.md#acoustic-inverse-source-problem) means minimizing $\|TQ-f_\infty\|^2$. **Its [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) is**

$$
\boxed{T^*TQ=T^*f_\infty.}
$$

For compatible data, the formal minimum-norm solution can be written with the [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator):

$$
\boxed{Q^\dagger=T^\dagger f_\infty
=\left[(T^*T)|_{(\ker T)^\perp}\right]^{-1}T^*f_\infty,\qquad
Q=Q^\dagger+h,\quad h\in\ker T.}
$$

The inverse in this expression is defined on the range of the restricted operator, not as a bounded everywhere-defined inverse. The unrestricted expression $(T^*T)^{-1}T^*f_\infty$ is only formal because $T$ has a nontrivial [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map).

The [normal kernel of the source-to-far-field operator](../../../physics.md#normal-kernel-of-the-source-to-far-field-operator) can be computed explicitly:

$$
(T^*TQ)(\mathbf r)=\frac1{16\pi^2}\int_AQ(\mathbf r')
\left[\int_{S_1}e^{ik\boldsymbol\theta\cdot(\mathbf r-\mathbf r')}\,dS(\boldsymbol\theta)\right]d^3\mathbf r'
=\frac1{4\pi}\int_A\frac{\sin(k|\mathbf r-\mathbf r'|)}{k|\mathbf r-\mathbf r'|}Q(\mathbf r')\,d^3\mathbf r'.
$$

The quotient is $1$ at coincidence. This smooth kernel already exhibits the loss of information.

There are two distinct causes of [ill-posedness](../../../partial-differential-equation.md#ill-posed-problem). First, a [fixed-frequency nonradiating source](../../../physics.md#fixed-frequency-nonradiating-source) gives exact nonuniqueness. For any $\chi\in C_c^\infty(A)$, put

$$
Q_\chi=(\Delta+k^2)\chi.
$$

The outgoing solution is $\psi=\chi$, which vanishes outside $A$, so $TQ_\chi=0$. Equivalently, integration by parts in the [source-to-far-field operator at fixed frequency](../../../physics.md#source-to-far-field-operator-at-fixed-frequency) gives

$$
\int_A e^{-ik\boldsymbol\theta\cdot\mathbf r}(\Delta+k^2)\chi(\mathbf r)\,d^3\mathbf r=0,
$$

since the exponential solves the homogeneous [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) and the boundary terms vanish. This provides an infinite-dimensional family of invisible sources. Single-frequency data determine only the spherical restriction of a three-dimensional [Fourier transform](../../../analysis.md#fourier-transform).

Second, the [compact operator](../../../compact-operator.md) $T$ has arbitrarily small nonzero [singular values](../../../linear-algebra.md#singular-value). To see that its rank is infinite, choose a source $Q_{\ell m}(r\boldsymbol\eta)=q_\ell(r)Y_\ell^m(\boldsymbol\eta)$, with a [spherical harmonic](../../../analysis.md#spherical-harmonic) $Y_\ell^m$. The plane-wave angular integral gives

$$
(TQ_{\ell m})(\boldsymbol\theta)=-(-i)^\ell Y_\ell^m(\boldsymbol\theta)\int_0^{r_0}q_\ell(r)j_\ell(kr)r^2\,dr.
$$

The [Spherical Bessel function](../../../analysis.md#spherical-bessel-function) $j_\ell(kr)$ is not identically zero, so choose $q_\ell(r)=j_\ell(kr)$ to obtain a nonzero far-field coefficient for every $\ell$. The mutually orthogonal angular modes prove infinite rank. The inverse on $(\ker T)^\perp$ is therefore unbounded, and division by these small [singular values](../../../linear-algebra.md#singular-value) amplifies noise. Its range is not closed; arbitrary noisy $L^2(S_1)$ data need not be the [far-field pattern](../../../inverse-problem.md#far-field-pattern) of a source, and a [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) need not exist without [regularization of an inverse problem](../../../inverse-problem.md#regularization-of-an-inverse-problem). For example, [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization) gives $(T^*T+\lambda I)^{-1}T^*f^\delta_\infty$. It stabilizes the recovered visible component but cannot identify the missing [fixed-frequency nonradiating source](../../../physics.md#fixed-frequency-nonradiating-source) component.

## 3

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [regularization of an inverse problem](../../../inverse-problem.md#regularization-of-an-inverse-problem) replaces the possibly unbounded inverse by a family of continuous reconstruction operators $R_\alpha:Y\to X$. For compatible exact data it must recover the minimum-norm solution $x^\dagger\in(\ker A)^\perp$ as $\alpha\downarrow0$. For noisy data $\|y^\delta-y\|\leq\delta$, a parameter rule $\alpha=\alpha(\delta)$ must make both bias and amplified noise tend to zero. The target is the minimum-norm solution because data cannot determine a component in the [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map).

[Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization) minimizes

$$
J_\alpha(x)=\|Ax-y^\delta\|_Y^2+\alpha\|x\|_X^2,\qquad \alpha>0.
$$

The [quadratic norm penalty](../../../inverse-problem.md#quadratic-norm-penalty) makes this [functional](../../../calculus-of-variations.md#functional) [strictly convex](../../../real-analysis.md#strictly-convex-function) and a [coercive function](../../../real-analysis.md#coercive-function). Its first variation, applied to arbitrary real and imaginary perturbations, gives

$$
(A^*A+\alpha I)x_\alpha^\delta=A^*y^\delta.
$$

The [positive operator](../../../hilbert-space.md#positive-operator) $A^*A+\alpha I$ is bounded below by $\alpha I$ and has a bounded inverse. **The unique [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization) solution is**

$$
\boxed{x_\alpha^\delta=R_\alpha y^\delta,\qquad
R_\alpha=(A^*A+\alpha I)^{-1}A^*.}
$$

The [Tikhonov stability bound](../../../inverse-problem.md#tikhonov-stability-bound) follows from the singular-value gain:

$$
\|R_\alpha\|\leq\sup_{\sigma\geq0}\frac{\sigma}{\sigma^2+\alpha}
=\frac1{2\sqrt\alpha},\qquad
\boxed{\|x_\alpha^\delta-x_\alpha\|\leq\frac{\delta}{2\sqrt\alpha}.}
$$

Thus reconstruction is stable for each fixed positive $\alpha$. Stability is not uniform as $\alpha\downarrow0$: that limit restores the unbounded inverse. For exact compatible data,

$$
x_\alpha-x^\dagger=-\alpha(A^*A+\alpha I)^{-1}x^\dagger\longrightarrow0.
$$

The [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator) makes this strong convergence transparent: each positive singular-value coefficient tends to zero and is bounded by the corresponding coefficient of $x^\dagger$. Consequently

$$
\|x_\alpha^\delta-x^\dagger\|
\leq\|x_\alpha-x^\dagger\|+\frac{\delta}{2\sqrt\alpha}\longrightarrow0
$$

whenever $\alpha(\delta)\downarrow0$ and $\delta/\sqrt{\alpha(\delta)}\to0$, for example $\alpha(\delta)=\delta$. This is a convergent [regularization of an inverse problem](../../../inverse-problem.md#regularization-of-an-inverse-problem), not merely a bounded formula.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator) consists of positive [singular values](../../../linear-algebra.md#singular-value) $\sigma_i$ and [orthonormal](../../../linear-algebra.md#orthonormal-set) vectors $v_i\in X$, $u_i\in Y$, with

$$
\boxed{Av_i=\sigma_i u_i,\qquad A^*u_i=\sigma_i v_i.}
$$

The $v_i$ form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $(\ker A)^\perp$, and the $u_i$ form one of $\overline{\operatorname{ran}A}$. There are finitely many positive [singular values](../../../linear-algebra.md#singular-value) for finite-rank $A$; otherwise $\sigma_i\to0$. Obtain the system by applying the [spectral theorem for compact self-adjoint operators](../../../compact-operator.md#spectral-theorem-for-compact-hermitian-operators) to $A^*A$, choosing $A^*Av_i=\sigma_i^2v_i$, and setting $u_i=Av_i/\sigma_i$. The [inner product](../../../linear-algebra.md#inner-product) identities verify orthonormality and the displayed relations.

With [inner products](../../../linear-algebra.md#inner-product) linear in the first argument,

$$
Ax=\sum_i\sigma_i(x,v_i)u_i,\qquad
A^*y=\sum_i\sigma_i(y,u_i)v_i.
$$

The [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) with the [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization) penalty acts separately on each $v_i$. Hence the [singular-system Tikhonov filter](../../../inverse-problem.md#singular-system-tikhonov-filter) gives **the regularized solution**

$$
\boxed{x_\alpha=\sum_i\frac{\sigma_i}{\sigma_i^2+\alpha}(y,u_i)v_i.}
$$

This norm-convergent series follows from [Bessel's inequality](../../../hilbert-space.md#bessel-s-inequality) and the bound $\sigma_i/(\sigma_i^2+\alpha)\leq1/(2\sqrt\alpha)$. Data orthogonal to $\overline{\operatorname{ran}A}$ are annihilated by $A^*$, and the minimizing solution has no component in $\ker A$. The same formula with $y^\delta$ reconstructs noisy data. In contrast, the unregularized inverse would divide $(y,u_i)$ by $\sigma_i$, with convergence governed by the [Picard criterion](../../../inverse-problem.md#picard-criterion).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the recurrence exactly as printed. Set $B=A^*A$ and $R=I-B/\alpha$. It gives

$$
x_{n+1}=Rx_n+\frac1\alpha A^*y,\qquad
x_0=(B+\alpha I)^{-1}A^*y.
$$

Repeated substitution yields a function of $A^*y$ alone:

$$
\boxed{x_n=R^n(B+\alpha I)^{-1}A^*y+
\frac1\alpha\sum_{j=0}^{n-1}R^jA^*y.}
$$

The empty sum is zero for $n=0$. This is [Landweber iteration with a Tikhonov initial value](../../../inverse-problem.md#landweber-iteration-with-a-tikhonov-initial-value). In the [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator), $Rv_i=r_i v_i$, where $r_i=1-\sigma_i^2/\alpha$. Thus

$$
x_n=\sum_i\left[
r_i^n\frac{\sigma_i}{\sigma_i^2+\alpha}
+\frac{\sigma_i}{\alpha}\sum_{j=0}^{n-1}r_i^j\right](y,u_i)v_i.
$$

For every positive [singular value](../../../linear-algebra.md#singular-value), the finite geometric sum gives

$$
\frac{\sigma_i}{\alpha}\sum_{j=0}^{n-1}r_i^j
=\frac{1-r_i^n}{\sigma_i}.
$$

Therefore **the [closed form of a Tikhonov-initialized Landweber iterate](../../../inverse-problem.md#closed-form-of-a-tikhonov-initialized-landweber-iterate) is**

$$
\boxed{x_n=\sum_i g_{\alpha,n}(\sigma_i)(y,u_i)v_i,\qquad
g_{\alpha,n}(\sigma)=\frac1{\sigma}\left[
1-\frac{\alpha}{\alpha+\sigma^2}\left(1-\frac{\sigma^2}{\alpha}\right)^n
\right].}
$$

In the printed notation, $g_\alpha(y,u_i)$ means the coefficient $g_{\alpha,n}(\sigma_i)(y,u_i)$; its dependence on $n$ and $\sigma_i$ is implicit. At $n=0$, the formula reduces to $\sigma/(\sigma^2+\alpha)$, exactly the [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization) initial value. At fixed $n$, its apparent singularity at $\sigma=0$ is removable:

$$
g_{\alpha,n}(\sigma)=\frac{(n+1)\sigma}{\alpha}+O(\sigma^3).
$$

Thus each fixed iterate is a bounded reconstruction operator and the series converges in norm.

The terminology in the question requires care. The printed recurrence is explicit [Landweber iteration](../../../inverse-problem.md#landweber-iteration) with step $1/\alpha$. Convergence of its nonzero modes requires $|1-\sigma_i^2/\alpha|<1$; a sufficient uniform step condition is

$$
\boxed{\alpha>\frac{\|A\|^2}{2}.}
$$

With exact compatible data and this condition, $x_n\to x^\dagger$. At equality the largest singular-value mode can alternate, and smaller $\alpha$ can produce growing modes. With noisy data, [early stopping of Landweber iteration](../../../inverse-problem.md#early-stopping-of-landweber-iteration) is needed to prevent recovery of arbitrarily unstable small-singular-value components.

Conventional [Iterated Tikhonov regularization](../../../inverse-problem.md#iterated-tikhonov-regularization) instead uses the implicit update

$$
(B+\alpha I)x_{n+1}=\alpha x_n+A^*y.
$$

With the same [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization) initial value its filter would be $[1-(\alpha/(\alpha+\sigma^2))^{n+1}]/\sigma$, not the filter derived above. The solution here retains the authoritative printed update rather than silently changing it.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
