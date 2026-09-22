# Paper 70

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper70.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper70.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)

## 1

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use a [Fourier transform](../../../analysis.md#fourier-transform) parallel to the boundary. Splitting its traces into right- and left-supported parts gives [Half-range Fourier transforms](../../../analysis.md#half-range-fourier-transform) $F_+$ and $F_-$, analytic respectively above and below a common inversion contour. A small positive imaginary part of the [wavenumber](../../../wave-equation.md#wavenumber) implements the [limiting absorption principle](../../../gravity-wave.md#limiting-absorption-principle) and separates the incident [poles](../../../isolated-singularity.md#pole) and outgoing [branch points](../../../complex-analysis.md#branch-point). Solve the transformed differential equation normal to the boundary using its outgoing or decaying solution. The boundary conditions then yield a [Wiener-Hopf equation](../../../differential-equation.md#wiener-hopf-equation) of the form

$$
K(\alpha)F_+(\alpha)=F_-(\alpha)+H(\alpha).
$$

Factor its [Wiener-Hopf kernel](../../../differential-equation.md#wiener-hopf-kernel) as $K=K_+K_-$, with each factor analytic and nonzero in its designated half-plane. Divide by $K_-$ and split $H/K_-=H_++H_-$, allocating [poles](../../../isolated-singularity.md#pole) according to the incident-wave prescription. Then

$$
K_+F_+-H_+=F_-/K_-+H_-.
$$

The two sides continue to a common [entire function](../../../complex-analysis.md#entire-function). Their growth at infinity, inherited from the field's edge behavior, determines that [function](../../../function.md), usually a constant or a [polynomial](../../../polynomial.md); in a decaying case it is zero. Solve for the unknown transforms and apply [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem), preserving the outgoing contour prescription.

The principal analytic results used are as follows. The [Paley–Wiener theorem](../../../distribution-theory.md#paley-wiener-theorem) and its half-line Laplace-transform version relate support on a half-line to holomorphy in a half-plane, with growth or square-integrability bounds. The [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) and [Sokhotski–Plemelj theorem](../../../complex-analysis.md#sokhotski-plemelj-theorem) provide additive splitting: a Cauchy [integral](../../../calculus.md#integral) of a sufficiently decaying jump has upper and lower boundary values with that prescribed difference. Applying the same construction to a continuous logarithm of a nonvanishing scalar [Wiener-Hopf kernel](../../../differential-equation.md#wiener-hopf-kernel) gives [Wiener-Hopf factorization](../../../differential-equation.md#wiener-hopf-factorization) when its [winding number](../../../complex-analysis.md#winding-number) is zero; a nonzero index requires an explicit index factor. The [identity theorem](../../../complex-analysis.md#identity-theorem) gives [analytic continuation](../../../complex-analysis.md#analytic-continuation) across the common strip. Finally [Liouville's theorem](../../../complex-analysis.md#liouville-theorem) makes a bounded [entire function](../../../complex-analysis.md#entire-function) constant; its polynomial-growth extension bounds the possible degree. The physical edge and [radiation conditions](../../../gravity-wave.md#radiation-condition) select the remaining constants. Zeros, [branch cuts](../../../analysis.md#branch-cut), nonzero index and insufficient decay must be accounted for rather than discarded during splitting.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Work above the plane, with $e^{-i\omega t}$ time dependence and $0<\theta<\pi$ away from grazing incidence. Put $a=k\cos\theta$ and $b=k\sin\theta$. The incident field and its chosen flat Dirichlet reflection cancel in value at the plane, while their [normal derivative](../../../differential-geometry.md#normal-derivative) is $-2ib e^{iax}$. Thus the diffracted correction has zero trace on the negative half-line and prescribed [normal derivative](../../../differential-geometry.md#normal-derivative) $2ib e^{iax}$ on the positive half-line.

There is an incompatibility in the stated edge data: a [normal derivative](../../../differential-geometry.md#normal-derivative) that is identically zero on the Neumann half-line cannot diverge as that half-line approaches the junction. **The inverse-square-root normal-derivative singularity belongs to the Dirichlet side, $x\to0^-$; on $x>0$ the total [normal derivative](../../../differential-geometry.md#normal-derivative) remains zero.** The following solution satisfies the mixed conditions and bounded-field edge behavior, with that corrected side.

Take the transform and its inverse as

$$
\widehat f(\alpha)=\int_{\mathbb R}f(x)e^{i\alpha x}dx,\qquad
f(x)=\frac1{2\pi}\int_C\widehat f(\alpha)e^{-i\alpha x}d\alpha.
$$

Let $U_+$ be the transform of the diffracted boundary value, and $V_-$ the transform of its unknown [normal derivative](../../../differential-geometry.md#normal-derivative) on the negative half-line. The outgoing transformed field is $U_+(\alpha)e^{i\beta(\alpha)y}$, where

$$
\beta=\sqrt{k^2-\alpha^2}=\beta_+\beta_-,\qquad\beta_+=\sqrt{k+\alpha},\quad\beta_-=\sqrt{k-\alpha}.
$$

Continue $k$ into the upper half-plane. Choose branches so that $\beta(0)=k$, outgoing propagating waves have positive vertical [wavenumber](../../../wave-equation.md#wavenumber), and [evanescent waves](../../../continuum-mechanics.md#evanescent-wave) decay. The [branch point](../../../complex-analysis.md#branch-point) $-k$ lies below $C$ and belongs to $\beta_+$; $k$ lies above $C$ and belongs to $\beta_-$. Since $\int_0^\infty e^{i(\alpha+a)x}dx=i/(\alpha+a)$, the boundary transform equation is

$$
i\beta_+U_+=\frac{V_-}{\beta_-}-\frac{2b}{(\alpha+a)\beta_-}.
$$

The forcing splits by subtracting its numerator at the incident [pole](../../../isolated-singularity.md#pole):

$$
H_+=-\frac{2b}{\beta_-(-a)(\alpha+a)},\qquad
H_-=-\frac{2b}{\alpha+a}\left(\frac1{\beta_-(\alpha)}-\frac1{\beta_-(-a)}\right).
$$

The [pole](../../../isolated-singularity.md#pole) in $H_-$ is removable; $H_-$ is analytic below $C$, while $H_+$ is analytic above it. Hence $i\beta_+U_+-H_+=V_-/\beta_-+H_-$ is entire. The bounded mixed-boundary edge solution has $U_+=O(\alpha^{-3/2})$ and $V_-=O(\alpha^{-1/2})$, making both sides decay at infinity. These orders can also be obtained locally from the leading wedge solution $r^{1/2}\cos(\varphi/2)$, which is Neumann at $\varphi=0$ and Dirichlet at $\varphi=\pi$. [Liouville's theorem](../../../complex-analysis.md#liouville-theorem) sets the entire remainder to zero. Therefore

$$
\boxed{U_+(\alpha)=\frac{2ib}{\sqrt{k+a}\,(\alpha+a)\sqrt{k+\alpha}}.}
$$

The solution of [mixed Dirichlet-Neumann half-plane diffraction](../../../differential-equation.md#mixed-dirichlet-neumann-half-plane-diffraction) is consequently

$$
\boxed{\phi_d(x,y)=\frac{ib}{\pi\sqrt{k+a}}\int_C\frac{e^{-i\alpha x+i\sqrt{k^2-\alpha^2}\,y}}{(\alpha+a)\sqrt{k+\alpha}}\,d\alpha,\qquad
\phi_t=e^{iax-iby}-e^{iax+iby}+\phi_d.}
$$

For $k=k_0+i\varepsilon$, take $C$ from left to right inside $-\varepsilon<\operatorname{Im}\alpha<\varepsilon$ and above the incident [pole](../../../isolated-singularity.md#pole) $-a$. Cuts from $-k$ run into the lower half-plane and cuts from $k$ into the upper half-plane, without crossing $C$. For example choose $\operatorname{Im}\alpha=c$ with $\max(-\varepsilon,-\varepsilon\cos\theta)<c<\varepsilon$. Then let $\varepsilon\downarrow0$, keeping the contour above $-a$ and $-k$ and below $k$. Any subsequent deformation for asymptotic evaluation must preserve these bypasses or include the [residues](../../../analysis.md#residue) of crossed [poles](../../../isolated-singularity.md#pole). This prescription fixes the reflected-wave contributions and the [radiation condition](../../../gravity-wave.md#radiation-condition); a principal-value [integral](../../../calculus.md#integral) alone would not do so.

As a boundary check, $i\beta U_+=-2b\beta_-/[\sqrt{k+a}(\alpha+a)]$. On the positive half-line the lower-contour [residue](../../../analysis.md#residue) gives $2ib e^{iax}$, cancelling the incident-plus-reflected [derivative](../../../calculus.md#derivative). The boundary trace vanishes on the negative half-line by upper-half-plane analyticity. Finally $U_+=O(\alpha^{-3/2})$ gives a square-root boundary value and hence a bounded field at the junction; the singular [derivative](../../../calculus.md#derivative) occurs on its Dirichlet side.

## 2

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $\mathbf r=(y,z)$ and prescribe a deterministic entrance field $E_0(\mathbf r)$. Substitution of the carrier into the [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) gives

$$
2ikE_x+E_{xx}+\Delta_\perp E+k^2(n^2-1)E=0.
$$

The usual weak-index paraxial model drops $E_{xx}$ and linearizes $n^2-1=2\mu W+O(\mu^2)$, giving

$$
E_x=DE+iaWE,\qquad D=\frac{i}{2k}\Delta_\perp,\quad a=k\mu.
$$

All the mean-field formulas below use this model. If the $\mu^2W^2$ term in $n^2$ is retained, its extra mean and fluctuations must also be included; Gaussian averaging of the linear random potential alone is then insufficient.

For a colored medium, taking [expectations](../../../probability-theory.md#expected-value) gives the exact propagation identity

$$
\boxed{m_x=Dm+ia\langle WE\rangle,\qquad m(0)=E_0,\qquad m=\langle E\rangle.}
$$

[Stationarity](../../../time-series.md#stationary-process) and Gaussianity alone do not close the last term. To make its dependence precise, let $C(s,\mathbf r)=\langle W(x+s,\mathbf r_0+\mathbf r)W(x,\mathbf r_0)\rangle$ and let $U_W(x,s;\mathbf r,\mathbf r')$ be the random paraxial propagator. Assuming a jointly [Gaussian random field](../../../stochastic-process.md#gaussian-random-field), rather than only Gaussian one-point marginals, the [functional derivative](../../../calculus-of-variations.md#functional-derivative) of the solution is

$$
\frac{\delta E(x,\mathbf r)}{\delta W(s,\mathbf r')}=ia\,U_W(x,s;\mathbf r,\mathbf r')E(s,\mathbf r'),\qquad0<s<x.
$$

The [Furutsu–Novikov formula](../../../stochastic-process.md#novikov-s-theorem) therefore yields

$$
\boxed{m_x(x,\mathbf r)=Dm(x,\mathbf r)-a^2\int_0^x ds\int_{\mathbb R^2}d\mathbf r'\,C(x-s,\mathbf r-\mathbf r')\left\langle U_W(x,s;\mathbf r,\mathbf r')E(s,\mathbf r')\right\rangle.}
$$

This is a propagation equation for the mean, with the remaining correlation displayed rather than silently replacing it by a product of means.

The general solution can be written explicitly as a Gaussian-averaged phase-screen product. Put $\Delta=x/N$, $x_j=j\Delta$, $\mathbf r_N=\mathbf r$ and let

$$
K_\Delta(\mathbf r)=\frac{k}{2\pi i\Delta}\exp\left(\frac{ik|\mathbf r|^2}{2\Delta}\right)
$$

be the [integral](../../../calculus.md#integral) kernel of the [Fresnel propagator](../../../partial-differential-equation.md#fresnel-propagator). Successive free-propagation and random-phase steps, followed by Gaussian averaging, give the [colored Gaussian paraxial mean propagator](../../../partial-differential-equation.md#colored-gaussian-paraxial-mean-propagator)

$$
\boxed{m(x,\mathbf r)=\lim_{N\to\infty}\int_{(\mathbb R^2)^N}E_0(\mathbf r_0)\prod_{j=1}^N K_\Delta(\mathbf r_j-\mathbf r_{j-1})\,
\exp\left[-\frac{a^2\Delta^2}{2}\sum_{j,l=1}^N C(x_j-x_l,\mathbf r_j-\mathbf r_l)\right]\prod_{j=0}^{N-1}d\mathbf r_j.}
$$

For smooth colored media this is the time-slicing representation, with oscillatory [integrals](../../../calculus.md#integral) understood by the usual Fresnel regularization. At finite $N$ the exponential follows directly from the [characteristic function](../../../probability-theory.md#characteristic-function) of the jointly Gaussian phase sum. It exhibits why a general transverse [covariance](../../../variance.md#covariance) cannot be replaced by its value at zero separation along every diffraction path.

For completeness, the unlinearized paraxial model has $E_x=DE+iaWE+i(k\mu^2/2)W^2E$ and the corresponding mean equation includes $i(k\mu^2/2)\langle W^2E\rangle$. Its colored-medium solution uses the same time-slicing [integral](../../../calculus.md#integral), replacing the Gaussian factor by

$$
\det\bigl(I-ik\mu^2\Delta\mathsf C\bigr)^{-1/2}\exp\left[-\frac{a^2\Delta^2}{2}\mathbf1^T\bigl(I-ik\mu^2\Delta\mathsf C\bigr)^{-1}\mathsf C\mathbf1\right],\qquad
\mathsf C_{jl}=C(x_j-x_l,\mathbf r_j-\mathbf r_l).
$$

This follows by completing the square in the finite-dimensional [Gaussian integral](../../../calculus.md#gaussian-integral), with the determinant branch continuous from $\mu=0$. It supplies the generic colored-medium mean when the $W^2$ term is retained. A square of ideal [white noise](../../../time-series.md#white-noise) is not defined by the [covariance](../../../variance.md#covariance) in part (b); that limit uses the linear random-potential model and its stated drift.

If transverse diffraction of the fluctuations is neglected, the simpler straight-ray approximation gives

$$
\boxed{m(x,\mathbf r)=E_0(\mathbf r)\exp\left[-a^2\int_0^x(x-s)C(s,\mathbf0)\,ds\right],\qquad m_x=-a^2\left[\int_0^x C(s,\mathbf0)ds\right]m.}
$$

Indeed $E=E_0\exp[ia\int_0^xW(s,\mathbf r)ds]$ and the [variance](../../../variance.md) of its phase is $2a^2\int_0^x(x-s)C(s,\mathbf0)ds$. If $W$ is constant transversely, this formula is exact with $E_0$ replaced by the free diffracted field $e^{xD}E_0$. For example $W=Z$, a single standard normal variable constant throughout space, satisfies [stationarity](../../../time-series.md#stationary-process) and unit [variance](../../../variance.md) but gives $m=e^{-a^2x^2/2}e^{xD}E_0$. Thus **a constant-rate exponential attenuation is not a consequence of part (a)'s assumptions alone**. It becomes the closed paraxial result under the longitudinal white-noise assumption in the next part.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Interpret the longitudinal delta [covariance](../../../variance.md#covariance) as a white-noise limit. It is a generalized random field, not a pointwise unit-variance [function](../../../function.md). Let $B_x(\mathbf r)$ have independent longitudinal increments with

$$
\langle dB_x(\mathbf r)dB_x(\mathbf r')\rangle=A(\mathbf r-\mathbf r')dx.
$$

The smooth-medium limit gives the Stratonovich equation $dE=DE\,dx+iaE\circ dB$. Conversion to Itô form contributes the local [variance](../../../variance.md) drift:

$$
dE=\left(DE-\frac{a^2A(0)}2E\right)dx+iaE\,dB.
$$

The Itô [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) has zero mean, so [coherent attenuation in a white-noise random medium](../../../partial-differential-equation.md#coherent-attenuation-in-a-white-noise-random-medium) satisfies

$$
\boxed{m_x=\frac{i}{2k}\Delta_\perp m-\gamma m,\qquad\gamma=\frac{k^2\mu^2A(0)}2,\qquad
m(x,\mathbf r)=e^{-\gamma x}(U_xE_0)(\mathbf r).}
$$

Here $U_x=e^{ix\Delta_\perp/(2k)}$ is the [Fresnel propagator](../../../partial-differential-equation.md#fresnel-propagator). Equivalently,

$$
m(x,\mathbf r)=e^{-\gamma x}\frac{k}{2\pi ix}\int_{\mathbb R^2}\exp\left(\frac{ik|\mathbf r-\mathbf r'|^2}{2x}\right)E_0(\mathbf r')d\mathbf r'.
$$

For a constant entrance envelope this is simply its constant value times $e^{-\gamma x}$.

Put $B_n(r)=\mu^2A(r)$, the transverse [covariance](../../../variance.md#covariance) coefficient of the refractive-index fluctuations. The spectrum required here is the transverse spectrum of that longitudinal [covariance](../../../variance.md#covariance) coefficient, or equivalently the longitudinal-zero-frequency slice of a prelimit stationary medium. Radial symmetry refers to the transverse plane; exact [white noise](../../../time-series.md#white-noise) in one direction is not full three-dimensional isotropy. With the Cartesian Fourier convention,

$$
S_F(\boldsymbol\nu)=\int_{\mathbb R^2}B_n(\mathbf r)e^{-i\boldsymbol\nu\cdot\mathbf r}d\mathbf r,
$$

angular integration gives $S_F(\nu)=2\pi\int_0^\infty B_n(r)J_0(\nu r)r\,dr$. Its inverse gives

$$
B_n(0)=\frac1{2\pi}\int_0^\infty S_F(\nu)\nu\,d\nu,\qquad
\boxed{m(x)=\exp\left[-\frac{k^2x}{4\pi}\int_0^\infty S_F(\nu)\nu\,d\nu\right]U_xE_0.}
$$

The printed transform hint mixes two different normalizations. Its radial transform and inverse constitute the self-reciprocal Hankel pair, whose spectrum is $S_H=S_F/(2\pi)$, rather than the unnormalized Cartesian transform also displayed there. Using that Hankel convention consistently yields instead

$$
\boxed{m(x)=\exp\left[-\frac{k^2x}{2}\int_0^\infty S_H(\nu)\nu\,d\nu\right]U_xE_0.}
$$

These are the same physical solution after converting spectra. The distinction is [Fourier-Hankel normalization for an isotropic spectrum](../../../analysis.md#fourier-hankel-normalization-for-an-isotropic-spectrum); $J_0(0)=1$ fixes the zero-separation [covariance](../../../variance.md#covariance) in either convention.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For the given Gaussian radial spectrum, the only needed [integral](../../../calculus.md#integral) is

$$
\int_0^\infty \mu^2L^3e^{-\nu^2L^2/4}\nu\,d\nu=2\mu^2L.
$$

If $S$ is interpreted with the self-reciprocal Hankel pair in the supplied hint, the coherent field is

$$
\boxed{m(x,\mathbf r)=e^{-k^2\mu^2Lx}(U_xE_0)(\mathbf r).}
$$

In this convention $B_n(r)=2\mu^2L e^{-r^2/L^2}$ and hence $B_n(0)=2\mu^2L$, directly verifying the attenuation coefficient. If instead the stated spectrum is the unnormalized Cartesian [Fourier transform](../../../analysis.md#fourier-transform), use its inverse normalization and obtain

$$
\boxed{m(x,\mathbf r)=e^{-k^2\mu^2Lx/(2\pi)}(U_xE_0)(\mathbf r).}
$$

Its transverse [covariance](../../../variance.md#covariance) coefficient is then $B_n(r)=\mu^2L\,e^{-r^2/L^2}/\pi$. The apparent difference is precisely the inconsistent Fourier/Hankel normalization in the printed hint, not a difference in stochastic propagation. For a unit constant entrance field the Fresnel factor is one; coherent intensity is the square of the displayed mean amplitude.

## 3

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Take $e^{-i\omega t}$ time dependence and measure angles from the upward normal. Write $p_i=k\sin\theta_i$, $q_i=k\cos\theta_i>0$ and choose incident amplitude $A_i$. Separate the flat Dirichlet reflection from the rough correction:

$$
\psi^{[0]}=A_i e^{ip_ix-iq_iz}-A_i e^{ip_ix+iq_iz},\qquad
\psi=\psi^{[0]}+\psi_s^{[1]}+O(h^2).
$$

[Taylor expansion](../../../calculus.md#taylor-expansion) of the boundary condition about $z=0$ gives

$$
0=\psi^{[0]}(x,0)+h(x)\partial_z\psi^{[0]}(x,0)+\psi_s^{[1]}(x,0)+O(h^2).
$$

Since $\partial_z\psi^{[0]}(x,0)=-2iq_iA_ie^{ip_ix}$, the induced trace is

$$
\boxed{\psi_s^{[1]}(x,0)=2iq_iA_ih(x)e^{ip_ix}.}
$$

Use $\widehat h(Q)=\int h(x)e^{-iQx}dx$ and $\beta(\xi)=\sqrt{k^2-\xi^2}$ with the outgoing branch: $\beta>0$ for $|\xi|<k$ and $\operatorname{Im}\beta>0$ outside. The [outgoing angular spectrum](../../../physics.md#outgoing-angular-spectrum) solves the [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) with that trace, giving the [first-order rough-surface scattered field](../../../physics.md#first-order-rough-surface-scattered-field)

$$
\boxed{\psi_s^{[1]}(x,z)=\frac{iq_iA_i}{\pi}\int_{\mathbb R}\widehat h(\xi-p_i)e^{i\xi x+i\beta(\xi)z}d\xi.}
$$

If “[scattered field](../../../physics.md#scattered-wave)” includes the specular reflection, add $-A_i e^{ip_ix+iq_iz}$ to this rough correction. [Fourier transforms](../../../analysis.md#fourier-transform) of an infinite random surface are generalized objects; finite-window transforms give an ordinary [integral](../../../calculus.md#integral) and are also needed for its far-field intensity. The expansion assumes a fixed regular surface shape scaled to small height. Highly oscillatory profiles can require additional control of slopes and spectral moments; small height alone is not a uniform error estimate for every profile.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Illuminate a surface window of length $D$, and define $\widehat h_D(Q)=\int_{-D/2}^{D/2}h(x)e^{-iQx}dx$. In the far field put $(x,z)=r(\sin\theta_s,\cos\theta_s)$, with $|\theta_s|<\pi/2$ away from grazing. The spectral phase $\xi\sin\theta_s+\beta(\xi)\cos\theta_s$ has stationary point $\xi_s=k\sin\theta_s$, value $k$, and second [derivative](../../../calculus.md#derivative) $-1/(k\cos^2\theta_s)$. [Stationary phase](../../../analysis.md#stationary-phase-method) therefore gives

$$
\psi_s^{[1]}\sim iq_iA_i\sqrt{\frac{2k}{\pi r}}\cos\theta_s\,
\widehat h_D(Q)e^{ikr-i\pi/4},\qquad Q=k\sin\theta_s-p_i.
$$

Let $C_h(s)=\langle h(x+s)h(x)\rangle$ and $S_h(Q)=\int C_h(s)e^{-iQs}ds$. Statistical [stationarity](../../../time-series.md#stationary-process) gives exactly

$$
\left\langle|\widehat h_D(Q)|^2\right\rangle
=\int_{-D}^D(D-|s|)C_h(s)e^{-iQs}ds.
$$

If $C_h$ is integrable, division by $D$ and [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) yield $\langle|\widehat h_D(Q)|^2\rangle/D\to S_h(Q)$. Thus the leading [rough-surface far-field intensity per illuminated length](../../../physics.md#rough-surface-far-field-intensity-per-illuminated-length) is

$$
\boxed{\frac{\langle|\psi_s^{[1]}(r,\theta_s)|^2\rangle}{D}
\sim\frac{2kq_i^2|A_i|^2\cos^2\theta_s}{\pi r}\,S_h(k\sin\theta_s-p_i).}
$$

This uses the field-intensity convention $I=|\psi|^2$; if $\psi$ is acoustic pressure, multiply by $1/(2\rho c)$ for physical far-field energy flux. The [variance](../../../variance.md) normalization is $\sigma^2=C_h(0)=(2\pi)^{-1}\int S_h(Q)dQ$. Consequently the diffuse intensity is of order $\sigma^2$ and samples the surface spectrum at the tangential momentum transfer. Its value is not determined by the r.m.s. height alone.

The finite window must first be in its far field, for example $r\gg kD^2$, before interpreting the large-window intensity density. An infinitely long stationary surface has infinite illuminated power and no finite total far-field intensity at a fixed point. For nonintegrable correlations the analogous result is a spectral measure, possibly with atoms. Zero mean height makes the linear rough mean field zero, but does not make its mean intensity zero; the flat specular reflection remains separate.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Translation invariance in $y$, together with a $y$-independent incident field, permits a $y$-independent solution. In homogeneous space Maxwell's equations then separate into two scalar sectors.

For a [TE wave](../../../electromagnetism.md#transverse-electric-polarization), set $\mathbf E=\widehat{\mathbf y}E_y(x,z)$. Its component satisfies $(\partial_x^2+\partial_z^2+k^2)E_y=0$. The $y$ direction is tangent to the conducting surface, so vanishing tangential [electric field](../../../electromagnetism.md#electric-field) imposes $E_y(x,h(x))=0$. Therefore **TE scattering is exactly the two-dimensional Dirichlet scalar problem**, with $E_y$ replacing the acoustic scalar. Its first-order boundary expansion and angular-spectrum formula are those above.

For a [TM wave](../../../electromagnetism.md#transverse-magnetic-polarization), set $\mathbf H=\widehat{\mathbf y}H_y(x,z)$. Maxwell's equation $\nabla\times\mathbf H=-i\omega\epsilon\mathbf E$ gives

$$
\mathbf E=\frac{i}{\omega\epsilon}(-\partial_zH_y,0,\partial_xH_y).
$$

A surface tangent is $(1,0,h')$, so vanishing tangential [electric field](../../../electromagnetism.md#electric-field) gives

$$
\boxed{(\partial_z-h'\partial_x)H_y(x,h(x))=0,\quad\text{equivalently }\partial_nH_y=0.}
$$

Thus **TM also reduces to two dimensions, but to a Neumann problem, not the [Dirichlet problem](../../../analysis.md#dirichlet-problem) in part (a)**. This is [scalar polarization reduction at a conducting corrugation](../../../electromagnetism.md#scalar-polarization-reduction-at-a-conducting-corrugation).

For example the flat TM reflection has positive sign, $H^{[0]}=A_i e^{ip_ix}(e^{-iq_iz}+e^{iq_iz})$. Its linearized rough forcing is

$$
\partial_zH_s^{[1]}(x,0)=2A_i e^{ip_ix}\bigl(q_i^2h+ip_i h'\bigr).
$$

In the transform domain this becomes $2A_i(k^2-p_i\xi)\widehat h(\xi-p_i)$, and propagation divides by $i\beta(\xi)$ rather than prescribing the electric Dirichlet trace. The explicit slope term and different reflection sign show why simply reusing the TE boundary formula for TM would be incorrect.

## 4

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Choose the scattering-potential convention $V(\mathbf r)=k^2[n(\mathbf r)^2-1]$. Let $G_k(\mathbf r,\mathbf r')=e^{ik|\mathbf r-\mathbf r'|}/(4\pi|\mathbf r-\mathbf r'|)$, so $(\Delta+k^2)G_k=-\delta$. Since $(\Delta+k^2)\psi=-V\psi$, the outgoing Green representation is the [Lippmann-Schwinger equation](../../../quantum-mechanics.md#lippmann-schwinger-equation)

$$
\psi=\psi_i+T\psi,\qquad (Tf)(\mathbf r)=\int_DG_k(\mathbf r,\mathbf r')V(\mathbf r')f(\mathbf r')d\mathbf r'.
$$

Iterating it produces the [Born series](../../../inverse-problem.md#born-series)

$$
\boxed{\psi_s=\sum_{j=1}^\infty T^j\psi_i.}
$$

For example its first two terms are

$$
\psi_s^{[1]}(\mathbf r)=\int_DG_k(\mathbf r,\mathbf r_1)V(\mathbf r_1)\psi_i(\mathbf r_1)d\mathbf r_1,
$$



$$
\psi_s^{[2]}(\mathbf r)=\int_D\int_DG_k(\mathbf r,\mathbf r_2)V(\mathbf r_2)G_k(\mathbf r_2,\mathbf r_1)V(\mathbf r_1)\psi_i(\mathbf r_1)d\mathbf r_1d\mathbf r_2.
$$

The first term describes one scattering event driven by the incident field. The second propagates its first scattered wave to another interaction before reaching the observer. Higher terms contain more successive interactions, including repeated visits to the same region; they account for multiple scattering rather than additional incident waves.

A sufficient convergence condition on an appropriate field [norm](../../../functional-analysis.md#norm) is $\|T\|=\rho<1$. Then the first-Born remainder is bounded by $\rho^2\|\psi_i\|/(1-\rho)$, while $\|T\psi_i\|\le\rho\|\psi_i\|$. A simple concrete sufficient condition on the bounded scatterer, using the supremum [norm](../../../functional-analysis.md#norm), is

$$
\sup_{\mathbf r\in D}\int_D|G_k(\mathbf r,\mathbf r')V(\mathbf r')|d\mathbf r'\ll1.
$$

This makes the field inside the inhomogeneity close to the incident field. Physically weak index contrast with small accumulated phase shift, such as $k\ell|n-1|\ll1$ for a smooth weak scatterer of thickness $\ell$, is a common first-Born regime, provided resonant enhancement and multiple reflections are negligible. Weak local contrast alone is not sufficient for an arbitrarily thick scatterer. If the opposite sign convention for $V$ is used, the [integral](../../../calculus.md#integral) operator changes sign and the same consistent iteration applies.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In first Born order the unknown potential enters linearly. Let $M_i$ multiply by the known incident field, $\mathcal G$ be the outgoing Green [integral](../../../calculus.md#integral) over the known support $D$, and $\mathcal R$ restrict the resulting field to the measurement set. With $y$ the measured scattered data,

$$
\boxed{y=AV,\qquad A=\mathcal R\mathcal G M_i.}
$$

The formal least-squares, [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution) is $V=A^\dagger y$, or $V=(A^*A)^{-1}A^*y$ on a domain where that inverse is meaningful. The [refractive index](../../../electromagnetism.md#refractive-index) is then

$$
\boxed{n(\mathbf r)=\sqrt{1+V(\mathbf r)/k^2},}
$$

choosing the physical branch approaching one outside the scatterer. At weak contrast $n-1\simeq V/(2k^2)$.

A noisy stable reconstruction uses [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization):

$$
V_\alpha^\delta=\operatorname*{arg\,min}_V\left\{\|AV-y^\delta\|_Y^2+\alpha\|V\|_X^2\right\},\qquad
\boxed{V_\alpha^\delta=(A^*A+\alpha I)^{-1}A^*y^\delta,\quad\alpha>0.}
$$

A smoothness penalty $\alpha\|LV\|^2$ may be substituted when appropriate, giving $A^*A+\alpha L^*L$ in the [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem), under the corresponding [coercivity](../../../real-analysis.md#coercive-function) assumptions. The parameter balances noise amplification and smoothing bias.

The data geometry matters: knowing a [scattered field](../../../physics.md#scattered-wave) on a measurement surface does not automatically mean knowing it throughout the support. A single incident wave and fixed-frequency far field sample only a shifted sphere of the potential's [Fourier transform](../../../analysis.md#fourier-transform), and in general do not determine an arbitrary three-dimensional potential uniquely. [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization) stabilizes a selected [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution); it cannot create missing information or guarantee uniqueness from inadequate data. If the total field and its [derivatives](../../../calculus.md#derivative) were known throughout $D$, the first-Born equation could instead be inverted formally as $V\simeq-(\Delta+k^2)\psi_s/\psi_i$ where $\psi_i\ne0$, but differentiation still amplifies measurement noise.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [adjoint operators](../../../hilbert-space.md#adjoint-operator), orthonormal [singular vectors](../../../semisimple-lie-algebra.md#singular-vector) and squared-norm [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) conditions require [Hilbert spaces](../../../hilbert-space.md). For arbitrary [normed spaces](../../../functional-analysis.md#normed-vector-space) the [Banach-space adjoint](../../../continuous-dual-space.md#transpose-of-a-bounded-linear-operator) takes values in the dual spaces and need not produce this formula. Interpret the given [singular value system](../../../inverse-problem.md#singular-system-of-a-compact-operator) in [Hilbert spaces](../../../hilbert-space.md), with $u_j$ in the unknown space and $v_j$ in the data space, as in the printed identities. Positive [singular values](../../../linear-algebra.md#singular-value) tending to zero provide the compact ill-posed case. A general [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) need not have this property; the [identity operator](../../../vector-space.md#identity-operator) is a well-conditioned counterexample. Components in the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) must be fixed by a minimum-norm convention, and the unregularized inverse is defined only for data satisfying the corresponding range condition.

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

Using the [singular value system](../../../inverse-problem.md#singular-system-of-a-compact-operator) with $Au_j=\sigma_jv_j$ and $A^*v_j=\sigma_ju_j$, the formal minimum-norm inverse is

$$
x=\sum_j\frac{(y,v_j)}{\sigma_j}u_j.
$$

It defines an element of the unknown [Hilbert space](../../../hilbert-space.md) only if $\sum_j|(y,v_j)|^2/\sigma_j^2<\infty$, the [Picard criterion](../../../inverse-problem.md#picard-criterion). A null-space component is undetermined by the data.

Adding an error along a single [left singular vector](../../../linear-algebra.md#left-singular-vector) changes precisely one coefficient:

$$
x_\delta-x=\frac\delta{\sigma_j}u_j,\qquad
\boxed{\|x_\delta-x\|=\frac\delta{\sigma_j}.}
$$

Although this perturbation has data [norm](../../../functional-analysis.md#norm) $\delta$, its amplification factor is $1/\sigma_j$. If $\sigma_j\to0$, these factors are unbounded. More explicitly choose $y^{(j)}=\sigma_jv_j$, tending to zero, while the minimum-norm inverse is $u_j$, of [norm](../../../functional-analysis.md#norm) one. Thus the inverse is discontinuous at zero. It may also fail to exist for data outside its nonclosed range, so merely minimizing a residual does not guarantee that the formal inverse exists. This is **[ill-posedness](../../../partial-differential-equation.md#ill-posed-problem) by unbounded small-singular-value amplification**, not a claim that every finite-dimensional or bounded forward map has an unstable inverse.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

For $\alpha>0$, minimize $J_\alpha(x)=\|Ax-y\|^2+\alpha\|x\|^2$. Its first variation in every direction gives

$$
(A^*A+\alpha I)x_\alpha=A^*y.
$$

The [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) on the left has lower bound $\alpha I$, so it is invertible and the minimizer is unique. The regularized solution has the singular expansion

$$
\boxed{x_\alpha=\sum_j\frac{\sigma_j}{\sigma_j^2+\alpha}(y,v_j)u_j.}
$$

Since $\sigma^2+\alpha\ge2\sigma\sqrt\alpha$, its gain is at most $1/(2\sqrt\alpha)$. Consequently

$$
\boxed{\|x_\alpha(y^\delta)-x_\alpha(y)\|\le\frac{\|y^\delta-y\|}{2\sqrt\alpha}.}
$$

This proves existence, uniqueness and continuous data dependence at fixed positive parameter. For the particular perturbation from part (i), the error is $\delta\sigma_j/(\sigma_j^2+\alpha)$ instead of $\delta/\sigma_j$. To recover a minimum-norm exact solution as noise tends to zero, choose $\alpha\to0$ while $\delta/\sqrt\alpha\to0$; [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) of the exact-data singular coefficients removes the bias.

To connect this with the provided inverse expansion, put $B=AA^*$ and $C=A^*A$. The exact intertwining identity is

$$
(A^*A+\alpha I)^{-1}A^*=A^*(\alpha I+AA^*)^{-1}.
$$

It follows by multiplying $(C+\alpha I)A^*=A^*(B+\alpha I)$ on either side by the appropriate [resolvent](../../../functional-analysis.md#resolvent-of-an-operator). A useful exact inverse identity is

$$
(\alpha I+B)^{-1}=\alpha^{-1}I-\alpha^{-2}A(I+\alpha^{-1}C)^{-1}A^*.
$$

Expanding $(I+\alpha^{-1}C)^{-1}$ to two terms gives the printed approximation, namely

$$
R_{\alpha,2}=\alpha^{-1}I-\alpha^{-2}B+\alpha^{-3}B^2.
$$

This is the [truncated Tikhonov resolvent](../../../inverse-problem.md#truncated-tikhonov-resolvent). Multiplication gives $(\alpha I+B)R_{\alpha,2}=I+\alpha^{-3}B^3$, so the expression is not an exact inverse. For example $A=1$ and $\alpha=1$ give the approximate value $1$ instead of the exact $1/2$. Its exact remainder is

$$
R_{\alpha,2}-(\alpha I+B)^{-1}=\alpha^{-3}B^3(\alpha I+B)^{-1},\qquad
\|R_{\alpha,2}-(\alpha I+B)^{-1}\|\le\frac{\|B\|^3}{\alpha^4}.
$$

In the regime $\|C\|/\alpha<1$ it is a controlled Neumann expansion. Using it to reconstruct gives

$$
x_{\alpha,2}=\left(\alpha^{-1}I-\alpha^{-2}C+\alpha^{-3}C^2\right)A^*y.
$$

For each fixed $\alpha>0$ this is a bounded [polynomial](../../../polynomial.md) in bounded operators, with

$$
\|x_{\alpha,2}(y^\delta)-x_{\alpha,2}(y)\|
\le\left(\frac{\|A\|}{\alpha}+\frac{\|A\|^3}{\alpha^2}+\frac{\|A\|^5}{\alpha^3}\right)\|y^\delta-y\|.
$$

Thus the supplied approximation also has continuous data dependence in its domain of use. It must not be extrapolated to $\alpha\downarrow0$ with $A$ fixed: its gain on any nonzero singular mode diverges, so it would not define a convergent regularization family there. **The exact Tikhonov filter supplies the well-posed regularized problem; the truncated formula is only a controlled computational approximation.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
