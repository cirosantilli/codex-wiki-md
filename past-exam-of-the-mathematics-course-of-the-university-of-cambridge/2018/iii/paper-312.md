# Paper 312

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_312.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_312.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
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
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $\varphi_G=\varphi_{G,L}+\varphi_{G,s}$. In the [local-type primordial non-Gaussianity](../../../cosmology.md#local-type-primordial-non-gaussianity) expansion, the term linear in the short field is $\varphi_{G,s}+2f_{\rm NL}\varphi_{G,L}\varphi_{G,s}$. The long-field square contributes to the long background, the mean subtraction is spatially homogeneous, and the short-field square is excluded at the order requested. Hence

$$
\boxed{\varphi_s=(1+2f_{\rm NL}\varphi_{G,L})\varphi_{G,s}}.
$$

This is the long-short coupling measured by a [squeezed bispectrum configuration](../../../cosmology.md#squeezed-bispectrum-configuration).

Because the long potential is constant over the short-scale region, multiplication by $1+2f_{\rm NL}\varphi_{G,L}$ commutes with the linear [cosmological Poisson equation](../../../linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) and any fixed linear smoothing filter. Thus the short [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) satisfies $\delta_s=(1+2f_{\rm NL}\varphi_{G,L})\delta_{G,s}$. Taking the conditional [expected value](../../../probability-theory.md#expected-value) over the short [Gaussian random field](../../../stochastic-process.md#gaussian-random-field) gives

$$
\langle\delta_s^2\rangle_s=(1+2f_{\rm NL}\varphi_{G,L})^2\sigma_{G,s}^2,
\qquad
\boxed{\sigma_s^2=\sigma_{G,s}^2(1+4f_{\rm NL}\varphi_{G,L})+O((f_{\rm NL}\varphi_{G,L})^2)}.
$$

The [short-scale variance modulation by local non-Gaussianity](../../../cosmology.md#short-scale-variance-modulation-by-local-non-gaussianity) is conditional on the long mode; averaging over that mode as well would erase the term linear in its zero mean.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Evaluate all derivatives at zero long perturbation, where $\nu=\delta_c/\sigma_{G,s}$, and write $\bar n(\nu)$ for the unperturbed abundance. The [peak-background split](../../../large-scale-structure-of-the-universe.md#peak-background-split) changes the [halo peak height](../../../large-scale-structure-of-the-universe.md#halo-peak-height) to

$$
\nu_{\rm loc}=\frac{\delta_c-\delta_L}{\sigma_{G,s}(1+2f_{\rm NL}\varphi_{G,L})}
=\nu-\frac{\nu}{\delta_c}\delta_L-2f_{\rm NL}\nu\varphi_{G,L}+\cdots.
$$

The [chain rule](../../../calculus.md#chain-rule) in the specified [bias expansion](../../../large-scale-structure-of-the-universe.md#bias-expansion) therefore gives

$$
\boxed{b_{10}=-\frac{\nu}{\delta_c}\frac{d\log\bar n}{d\nu},\qquad
b_{01}=-2f_{\rm NL}\nu\frac{d\log\bar n}{d\nu}
=2f_{\rm NL}\delta_c b_{10}}.
$$

No explicit abundance law is specified, so these derivatives are the general answer. For example, if $\bar n$ has the [Press-Schechter halo mass function](../../../large-scale-structure-of-the-universe.md#press-schechter-halo-mass-function) dependence $\nu e^{-\nu^2/2}$, then $b_{10}=(\nu^2-1)/\delta_c$ and $b_{01}=2f_{\rm NL}(\nu^2-1)$.

For the linear long mode, the [cosmological Poisson equation](../../../linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) gives $\varphi_{G,L}(\mathbf k)=\delta_{G,L}(\mathbf k)/\alpha(k)$. Consequently the deterministic [galaxy bias](../../../large-scale-structure-of-the-universe.md#galaxy-bias) and [power spectrum](../../../probability-and-statistics.md#power-spectrum) are

$$
\delta_g(\mathbf k)=\left[b_{10}+\frac{b_{01}}{\alpha(k)}\right]\delta_{G,L}(\mathbf k),
\qquad
\boxed{P_g(k)=b_{10}^2\left[1+\frac{2f_{\rm NL}\delta_c}{\alpha(k)}\right]^2P_m(k)}.
$$

Here $P_m$ is the linear [cosmological density power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum); stochastic tracer noise has been omitted. This [scale-dependent halo bias from local non-Gaussianity](../../../large-scale-structure-of-the-universe.md#scale-dependent-halo-bias-from-local-non-gaussianity) is proportional to $k^{-2}$ in the specified $\alpha(k)=2k^2/(3H^2\Omega_m)$ convention.

For $b_{10}\ne0$, plot the ratio $P_g/(b_{10}^2P_m)$ to separate the effect from the shape of $P_m$. Positive $f_{\rm NL}$ increases the ratio as $k$ decreases. Negative $f_{\rm NL}$ first suppresses it, gives a zero when $\alpha(k)=2|f_{\rm NL}|\delta_c$, and then makes it rise again after the effective [galaxy bias](../../../large-scale-structure-of-the-universe.md#galaxy-bias) changes sign. The auto-[power spectrum](../../../probability-and-statistics.md#power-spectrum) never becomes negative. A truncation $P_g\simeq b_{10}^2[1+4f_{\rm NL}\delta_c/\alpha(k)]P_m$ is valid only when $|2f_{\rm NL}\delta_c/\alpha(k)|\ll1$ and must not be extrapolated through the zero. Within the deterministic expression, both signs give $P_g\propto k^{-4}P_m$ at sufficiently small $k$. For a nearly scale-invariant primordial spectrum, $P_m\propto k^{n_s}$ in the large-scale transfer limit, so this formal asymptote is $k^{n_s-4}$.

<a id="1/ii/image-scale-dependent-galaxy-bias"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-312-bias-sketch.png)

**[Figure 1](#1/ii/image-scale-dependent-galaxy-bias). Scale-dependent galaxy bias**. Schematic deterministic power ratio for equal positive and negative coupling magnitudes, with $\alpha\propto k^2$. The negative-coupling cancellation scale defines $k_{\rm cancel}$; the vertical axis is logarithmic away from a small linear region around zero.

There is a convention issue in calling the specified abundance response an observed galaxy overdensity. The threshold response is naturally a [linear Lagrangian halo bias](../../../large-scale-structure-of-the-universe.md#linear-lagrangian-halo-bias). If $b_{10}$ instead denotes the physical [linear Eulerian halo bias](../../../large-scale-structure-of-the-universe.md#linear-eulerian-halo-bias), the [Lagrangian-to-Eulerian linear bias relation](../../../large-scale-structure-of-the-universe.md#lagrangian-to-eulerian-linear-bias-relation) adds one to the density coefficient: $b_{01}=2f_{\rm NL}\delta_c(b_{10}-1)$, and $P_g=[b_{10}+b_{01}/\alpha]^2P_m$. The boxed formulas follow the abundance expansion explicitly supplied in the paper. The Newtonian treatment also cannot be extrapolated beyond its physical large-scale domain without relativistic projection effects.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Use $\langle\varphi_G(\mathbf k)\varphi_G(\mathbf k')\rangle=(2\pi)^3\delta^{(3)}(\mathbf k+\mathbf k')P_\varphi(k)$. For nonzero external momenta, the quadratic term in [local-type primordial non-Gaussianity](../../../cosmology.md#local-type-primordial-non-gaussianity) is

$$
f_{\rm NL}\int\frac{d^3q}{(2\pi)^3}\varphi_G(\mathbf q)\varphi_G(\mathbf k-\mathbf q).
$$

Insert it in one of the three external fields. [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) supplies two connected [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) at each insertion, whereas the mean subtraction removes the disconnected zero-mode contribution. Thus the leading [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) is

$$
B_\varphi(k_1,k_2,k_3)=2f_{\rm NL}\bigl[P_\varphi(k_1)P_\varphi(k_2)+P_\varphi(k_2)P_\varphi(k_3)+P_\varphi(k_3)P_\varphi(k_1)\bigr].
$$

Linear propagation by the [cosmological Poisson equation](../../../linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) gives $P_m(k)=\alpha(k)^2P_\varphi(k)$ and multiplies the [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) by $\alpha_1\alpha_2\alpha_3$. Defining the matter three-point function by its momentum-conserving [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) times $B_m$, the [primordial contribution to the matter bispectrum](../../../cosmology.md#primordial-contribution-to-the-matter-bispectrum) is

$$
\boxed{B_m^{\rm prim}=2f_{\rm NL}\left[\frac{\alpha_3}{\alpha_1\alpha_2}P_m(k_1)P_m(k_2)+\frac{\alpha_1}{\alpha_2\alpha_3}P_m(k_2)P_m(k_3)+\frac{\alpha_2}{\alpha_3\alpha_1}P_m(k_3)P_m(k_1)\right]}.
$$

The nonlinear gravitational contribution from [standard perturbation theory in cosmology](../../../large-scale-structure-of-the-universe.md#standard-perturbation-theory-in-cosmology) is excluded here.

In a [squeezed bispectrum configuration](../../../cosmology.md#squeezed-bispectrum-configuration), $k_1=k_L\ll k_2\simeq k_3=k_S$, so

$$
B_m^{\rm prim}\simeq4f_{\rm NL}\frac{P_m(k_L)P_m(k_S)}{\alpha(k_L)}
+2f_{\rm NL}\frac{\alpha(k_L)}{\alpha(k_S)^2}P_m(k_S)^2.
$$

For a nearly scale-invariant potential, $P_\varphi(k_L)\gg P_\varphi(k_S)$, so the second term is subleading and

$$
\boxed{B_m^{\rm prim}(k_L,k_S,k_S)\simeq\frac{4f_{\rm NL}}{\alpha(k_L)}P_m(k_L)P_m(k_S)}.
$$

Relative to the product of matter [power spectra](../../../probability-and-statistics.md#power-spectrum), the squeezed response is enhanced by $k_L^{-2}$. Its sign is the sign of $f_{\rm NL}$. This is the three-point counterpart of the conditional [short-scale variance modulation by local non-Gaussianity](../../../cosmology.md#short-scale-variance-modulation-by-local-non-gaussianity).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

For an attractor with one adiabatic clock and a regular [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum), a long [comoving curvature perturbation](../../../cosmic-inflation.md#comoving-curvature-perturbation) $\zeta_L$ acts at leading order as a spatial dilation. The [single-field inflation squeezed-limit consistency relation](../../../cosmology.md#single-field-inflation-squeezed-limit-consistency-relation) therefore fixes

$$
\lim_{k_L/k_S\to0}\frac{B_\zeta(k_L,k_S,k_S)}{P_\zeta(k_L)P_\zeta(k_S)}=-(n_s-1).
$$

For the local convention $\zeta=\zeta_G+(3/5)f_{\rm NL}(\zeta_G^2-\langle\zeta_G^2\rangle)$, comparison with its squeezed [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) gives

$$
\boxed{f_{\rm NL}^{\rm squeezed}=\frac5{12}(1-n_s)}.
$$

The matter-era negative gravitational potential is $\varphi=3\zeta/5$, so this is also the conventional $f_{\rm NL}$ of part (i). In [single-field slow-roll inflation](../../../cosmic-inflation.md#single-field-slow-roll-inflation), the [spectral tilt](../../../cosmic-inflation.md#scalar-spectral-index) is small and the effective local coupling is of slow-roll size, typically of order $10^{-2}$ for a tilt of a few percent. This is a statement about the normalized coupling: the squeezed [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) still contains the large long-mode [power spectrum](../../../probability-and-statistics.md#power-spectrum).

Formally putting this small coupling into the local template of part (ii) predicts only a tiny correction on accessible scales, rather than an order-unity local signal. For a physical halo abundance there is a stronger qualification. The consistency-relation modulation at fixed coordinate wavelength is a dilation; the coordinate size of a fixed physical halo must be dilated too. Those responses cancel. This is the [absence of primordial scale-dependent halo bias in single-clock inflation](../../../cosmology.md#absence-of-primordial-scale-dependent-halo-bias-in-single-clock-inflation): the leading consistency-relation term produces no physical $k^{-2}$ halo bias. The first physical long-mode response contains two spatial derivatives, so dividing it by $\delta_L\propto k_L^2\varphi_L$ does not produce the local-template enhancement. Thus the leading primordial large-scale galaxy [power spectrum](../../../probability-and-statistics.md#power-spectrum) remains the Gaussian-bias result, apart from ordinary transfer, bias, and projection effects.

The cancellation can be seen with a [top-hat filter](../../../large-scale-structure-of-the-universe.md#top-hat-filter). At fixed local time, a constant long curvature rescales physical lengths by $e^{\zeta_L}$, so the coordinate radius of a fixed physical halo is $R_c=e^{-\zeta_L}R_0$, and the coordinate short [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) is $\delta_s(\mathbf x)=\delta_s^{(0)}(e^{\zeta_L}\mathbf x)$. Changing variables $\mathbf y=e^{\zeta_L}\mathbf x$ gives

$$
\frac{3}{4\pi R_c^3}\int_{|\mathbf x|<R_c}d^3x\,\delta_s^{(0)}(e^{\zeta_L}\mathbf x)
=\frac{3}{4\pi R_0^3}\int_{|\mathbf y|<R_0}d^3y\,\delta_s^{(0)}(\mathbf y).
$$

Thus the smoothed field and its [variance](../../../variance.md) at fixed physical mass are unchanged by the constant long mode.

The assumptions matter: a non-attractor such as [ultra-slow-roll inflation](../../../cosmic-inflation.md#ultra-slow-roll-inflation), additional fluctuating fields, or an excited initial state need not obey this squeezed-limit conclusion. A sizable physical local modulation would test the stated single-clock attractor assumptions, rather than every possible one-field model.

## 2

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The background [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe) satisfies $a'=\mathcal H a$ and $\mathcal H'=-\mathcal H^2/2$. Introduce $\mathcal F_n$ and $\mathcal G_n$ for the spatial [convolutions](../../../fourier-analysis.md#convolution) in the [Fourier transform](../../../analysis.md#fourier-transform) representation with kernels $F_n$ and $G_n$, respectively, so $\delta^{(n)}=a^n\mathcal F_n$ and $\theta^{(n)}=-\mathcal H a^n\mathcal G_n$. Differentiation gives

$$
(\delta^{(n)})'=n\mathcal H a^n\mathcal F_n,\qquad
(\theta^{(n)})'=-\left(n-\frac12\right)\mathcal H^2a^n\mathcal G_n.
$$

At first order the [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) yields $F_1-G_1=0$, while the [cosmological Euler equation](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation) gives $3F_1/2-3G_1/2=0$. The growing-mode normalization therefore gives $\boxed{G_1=F_1=1}$.

At second order, take the unsymmetrized order of the inputs printed in the paper. Matching the [alpha mode-coupling kernel](../../../large-scale-structure-of-the-universe.md#alpha-mode-coupling-kernel) and [beta mode-coupling kernel](../../../large-scale-structure-of-the-universe.md#beta-mode-coupling-kernel) terms gives

$$
2F_2-G_2=\alpha(q_1,q_2),\qquad
\frac52G_2-\frac32F_2=\beta(q_1,q_2).
$$

Hence

$$
F_2=\frac57\alpha+\frac27\beta,\qquad
G_2=\frac37\alpha+\frac47\beta.
$$

With the paper's unsymmetrized convention $\alpha=\beta=(q_1+q_2)/q_1$, one possible unsymmetrized representation is

$$
\boxed{F_2(q_1,q_2)=G_2(q_1,q_2)=\frac{q_1+q_2}{q_1}}.
$$

Only the symmetric part enters a [convolution](../../../fourier-analysis.md#convolution) of two identical linear fields. Symmetrizing gives

$$
F_{2,s}=G_{2,s}=\frac12\left[\frac{q_1+q_2}{q_1}+\frac{q_1+q_2}{q_2}\right]
=\boxed{\frac{(q_1+q_2)^2}{2q_1q_2}}.
$$

This is the [one-dimensional cosmological density kernel](../../../large-scale-structure-of-the-universe.md#one-dimensional-cosmological-density-kernel). The physical symmetric one-dimensional Euler kernel is also $(q_1+q_2)^2/(2q_1q_2)$: symmetrizing the printed $\beta$ reproduces it, so its apparently different unsymmetrized form is not a contradiction. Unsymmetrized kernels themselves are not unique, since antisymmetric parts integrate to zero. Zero input momenta require the usual separate treatment of the homogeneous background.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Use signed one-dimensional external momenta $k_1+k_2+k_3=0$, with nonzero $k_i$. Let $P_L(k)=P_L(-k)$ be the linear [cosmological density power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum) at the time of evaluation, normalized by $\langle\delta^{(1)}(k)\delta^{(1)}(k')\rangle=2\pi\delta^{(D)}(k+k')P_L(k)$. Using $P_L$ absorbs the factor $a^6$ multiplying a product of three initial [power spectra](../../../probability-and-statistics.md#power-spectrum). All kernels below are symmetrized [one-dimensional cosmological density kernels](../../../large-scale-structure-of-the-universe.md#one-dimensional-cosmological-density-kernel).

The connected [B222 contribution to the one-loop matter bispectrum](../../../large-scale-structure-of-the-universe.md#b222-contribution-to-the-one-loop-matter-bispectrum) has a triangular [Feynman diagram](../../../perturbative-quantum-field-theory.md#feynman-diagram): each second-order external field has two Gaussian inputs, joined pairwise to the other two vertices. The connected [B411 contribution to the one-loop matter bispectrum](../../../large-scale-structure-of-the-universe.md#b411-contribution-to-the-one-loop-matter-bispectrum) has a fourth-order vertex joined to both linear external fields, with its remaining two inputs contracted into a loop at that vertex. External stubs indicate the measured momenta; blue internal lines represent linear [power spectra](../../../probability-and-statistics.md#power-spectrum).

<a id="2/ii/image-one-loop-triangle-and-fourth-order-vertex-diagrams"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-312-loop-diagrams.png)

**[Figure 2](#2/ii/image-one-loop-triangle-and-fourth-order-vertex-diagrams). One-loop triangle and fourth-order-vertex diagrams**. The two connected one-loop topologies. Vertex labels are perturbative orders, not numbers of external measured fields. The $B_{411}$ diagram must be summed over the three choices of the fourth-order field.

There are $2^3=8$ connected [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) in the triangle, giving

$$
\boxed{B_{222}=8\int\frac{dq}{2\pi}\,F_2(q,k_1-q)F_2(-q,k_2+q)F_2(q-k_1,-k_2-q)
P_L(q)P_L(k_1-q)P_L(k_2+q)}.
$$

For a fixed fourth-order external field, attaching the two labelled linear fields gives $4\times3=12$ choices; the remaining pair contracts uniquely. Therefore

$$
\boxed{B_{411}=12P_L(k_1)P_L(k_2)\int\frac{dq}{2\pi}F_4(-k_1,-k_2,q,-q)P_L(q)+\text{two cyclic terms}}.
$$

These are contributions to the reduced connected [one-loop matter bispectrum](../../../large-scale-structure-of-the-universe.md#one-loop-matter-bispectrum), with its external momentum-conserving [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) removed. Disconnected contractions have a zero external momentum and are excluded.

For the ultraviolet behaviour, the three $F_2$ denominators multiply to a negative square. In fact

$$
8F_2(q,k_1-q)F_2(-q,k_2+q)F_2(q-k_1,-k_2-q)
=-\frac{k_1^2k_2^2k_3^2}{q^2(k_1-q)^2(k_2+q)^2}.
$$

Thus for $|q|\gg |k_i|$ and a smoothly varying high-momentum spectrum,

$$
B_{222}^{\rm UV}\simeq-k_1^2k_2^2k_3^2\int_{\rm hard}\frac{dq}{2\pi}\frac{P_L(q)^3}{q^6}.
$$

Each second-order vertex exhibits the [ultraviolet softness of the second-order density kernel](../../../large-scale-structure-of-the-universe.md#ultraviolet-softness-of-the-second-order-density-kernel), so this term contains six powers of external momentum.

The fourth-order kernel is even simpler:

$$
F_4(-k_1,-k_2,q,-q)=-\frac{k_3^4}{24k_1k_2q^2}.
$$

With a hard-loop cutoff $q_h<|q|<\Lambda$, define

$$
I_\Lambda=\int_{q_h<|q|<\Lambda}\frac{dq}{2\pi}\frac{P_L(q)}{q^2}.
$$

The [B411 contribution to the one-loop matter bispectrum](../../../large-scale-structure-of-the-universe.md#b411-contribution-to-the-one-loop-matter-bispectrum) from this range is exactly

$$
B_{411}^{\rm hard}=-\frac12\sum_{\rm cyclic}\frac{k_3^4}{k_1k_2}P_L(k_1)P_L(k_2)I_\Lambda
=-\sum_{\rm cyclic}k_3^2F_2(k_1,k_2)P_L(k_1)P_L(k_2)I_\Lambda.
$$

For fixed momentum ratios, it has two external derivative powers multiplying two long-mode [power spectra](../../../probability-and-statistics.md#power-spectrum), rather than the six-derivative stochastic structure of $B_{222}$. It is the leading deterministic UV-sensitive contribution for external modes below the [nonlinear wavenumber](../../../large-scale-structure-of-the-universe.md#nonlinear-wavenumber). This is a comparison of derivative orders and generic cutoff sensitivity; an arbitrary specially chosen spectrum or vanishing shape can change their numerical ranking. A convergent integral can still depend on nonperturbative short scales. For a high-$q$ power law $P_L(q)\propto |q|^n$, the $B_{411}$ integral diverges for $n\geq1$, whereas the $B_{222}$ integral diverges only for $n\geq5/3$, with logarithmic divergences at the thresholds.

At the field level, there are six ways to contract a hard pair within $\delta^{(4)}$. Comparing $6F_4$ with $F_2$ gives

$$
\delta^{(4)}_{\rm hard}(k)=-\frac{I_\Lambda}{2}k^2\delta^{(2)}(k).
$$

The appropriate [second-order density Laplacian counterterm](../../../large-scale-structure-of-the-universe.md#second-order-density-laplacian-counterterm) is therefore

$$
\boxed{\delta_{\rm ct}^{(2)}(x)=C(\Lambda)\partial_x^2\delta^{(2)}(x),\qquad
C(\Lambda)=-\frac12 I_\Lambda+C_{\rm finite}}.
$$

Indeed its contribution with two linear fields is $-2C(\Lambda)\sum_{\rm cyclic}k_3^2F_2P_L(k_1)P_L(k_2)$, which cancels the displayed hard-loop term. The [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) sign follows from $\partial_x^2\leftrightarrow-k^2$. Its finite coefficient must be matched to short-scale dynamics, as in the [effective field theory of large-scale structure](../../../large-scale-structure-of-the-universe.md#effective-field-theory-of-large-scale-structure). A term proportional to $\partial_x^2\delta^{(1)}$ similarly renormalizes a linear response, but a purely linear insertion cannot by itself cancel this $\langle\delta^{(4)}\delta^{(1)}\delta^{(1)}\rangle$ shape, since an odd Gaussian three-point function vanishes.

## 3

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For one [Fourier mode](../../../fourier-analysis.md#fourier-mode), put $\mu=\hat{\mathbf k}\cdot\mathbf e$. The collisionless equation becomes

$$
\dot\Theta+ik\mu\Theta=\dot\phi-ik\mu\psi.
$$

Use the unweighted [Legendre polynomial](../../../differential-equation.md#legendre-polynomial) expansion specified in the paper: $\Theta=\sum_{j\ge0}(-i)^j\Theta_jP_j(\mu)$. The [Legendre polynomial recurrence relation](../../../differential-equation.md#legendre-polynomial-recurrence-relation) says

$$
\mu P_j=\frac{j+1}{2j+1}P_{j+1}+\frac{j}{2j+1}P_{j-1}.
$$

The coefficient of $P_\ell$ in $ik\mu\Theta$ receives contributions from $j=\ell-1$ and $j=\ell+1$. Dividing by $(-i)^\ell$ gives respectively $-k\ell\Theta_{\ell-1}/(2\ell-1)$ and $k(\ell+1)\Theta_{\ell+1}/(2\ell+3)$. The metric sources are $\dot\phi P_0$ and $-ik\psi P_1$, the latter becoming $k\psi$ after division by $(-i)$. Hence the [neutrino Boltzmann hierarchy](../../../linear-cosmological-density-perturbation.md#neutrino-boltzmann-hierarchy) is

$$
\boxed{\dot\Theta_\ell+k\left(\frac{\ell+1}{2\ell+3}\Theta_{\ell+1}-\frac{\ell}{2\ell-1}\Theta_{\ell-1}\right)
=\delta_{\ell0}\dot\phi+\delta_{\ell1}k\psi}.
$$

The lower-neighbour term is absent for $\ell=0$. The low moments are

$$
\dot\Theta_0+\frac{k}{3}\Theta_1=\dot\phi,\qquad
\dot\Theta_1+k\left(\frac25\Theta_2-\Theta_0\right)=k\psi,\qquad
\dot\Theta_2+k\left(\frac37\Theta_3-\frac23\Theta_1\right)=0.
$$

These coefficients depend on the expansion convention. In the convention with a $(2\ell+1)$ factor, the temperature multipoles are $\Theta_\ell/(2\ell+1)$; using those multipoles without converting them would give incorrect factors in the [scalar neutrino anisotropic stress](../../../linear-cosmological-perturbation-theory.md#scalar-neutrino-anisotropic-stress).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $Q^{ij}=\hat k^i\hat k^j-\delta^{ij}/3$. Rotations around $\hat{\mathbf k}$ and the vanishing trace imply that the angular integral in the [scalar neutrino anisotropic stress](../../../linear-cosmological-perturbation-theory.md#scalar-neutrino-anisotropic-stress) has the form $A_\ell Q^{ij}$. Contract with $\hat k_i\hat k_j$ and use $\mu^2-1/3=(2/3)P_2(\mu)$. By the [Orthogonality of Legendre polynomials](../../../differential-equation.md#orthogonality-of-legendre-polynomials),

$$
\frac23 A_\ell=\frac12\int_{-1}^{1}P_\ell(\mu)\left(\mu^2-\frac13\right)d\mu
=\frac23\frac{\delta_{\ell2}}5,
\qquad A_\ell=\frac{\delta_{\ell2}}5.
$$

Only the quadrupole in the [neutrino Boltzmann hierarchy](../../../linear-cosmological-density-perturbation.md#neutrino-boltzmann-hierarchy) contributes. Its phase factor is $(-i)^2=-1$, so the supplied stress definition becomes

$$
\Pi^{\hat i\hat j}(\eta,\mathbf x)
=\frac45\bar\rho_\nu\int\frac{d^3\mathbf k}{(2\pi)^{3/2}}\Theta_2(\eta,\mathbf k)Q^{ij}e^{i\mathbf k\cdot\mathbf x}.
$$

Comparing with the chosen normalization $-(4/3)\bar\rho_\nu\Pi Q^{ij}$ gives

$$
\boxed{\Pi(\eta,\mathbf k)=-\frac35\Theta_2(\eta,\mathbf k)}.
$$

The sign and factor here follow jointly from the stress convention and the unweighted [Legendre polynomial](../../../differential-equation.md#legendre-polynomial) coefficients; they should not be transferred unchanged to a differently normalized hierarchy.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Write $\psi_0=\psi(0,\mathbf k)$. For regular [adiabatic initial conditions](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) during [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), use $\Theta_0=-\psi_0/2+O(k\eta)$, $\Theta_2=O((k\eta)^2)$, and constant potentials. The dipole equation in the [neutrino Boltzmann hierarchy](../../../linear-cosmological-density-perturbation.md#neutrino-boltzmann-hierarchy) gives

$$
\dot\Theta_1=k(\Theta_0+\psi_0)-\frac{2k}{5}\Theta_2
=\frac12 k\psi_0+O(k^2\eta).
$$

Regularity removes a constant dipole, and integration yields

$$
\boxed{\Theta_1=\frac12\psi_0 k\eta+O((k\eta)^2)}.
$$

Then the quadrupole equation gives

$$
\dot\Theta_2=\frac{2k}{3}\Theta_1-\frac{3k}{7}\Theta_3
=\frac13\psi_0 k^2\eta+O(k^3\eta^2).
$$

Its regular initial value is zero, so

$$
\boxed{\Theta_2=\frac16\psi_0(k\eta)^2+O((k\eta)^3)}.
$$

For the usual regular growing solution, the monopole has no linear correction and parity improves the dipole and quadrupole errors to $O((k\eta)^3)$ and $O((k\eta)^4)$, respectively. The weaker bounds above already follow from the assumptions explicitly given. Although the quadrupole is small on [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale), the trace-free [Einstein field equations](../../../general-relativity.md#einstein-field-equations) divide its stress by $k^2$, allowing a finite leading potential difference.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

For one [Fourier mode](../../../fourier-analysis.md#fourier-mode), the trace-free differential operator in the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) is $-k^2Q_{ij}$, with $Q_{ij}=\hat k_i\hat k_j-\delta_{ij}/3$. Part (ii) gives $\Pi_{ij}=(4/5)\bar\rho_\nu\Theta_2Q_{ij}$. The two minus signs in the field equation therefore imply

$$
k^2(\phi-\psi)=\frac{32\pi G}{5}a^2\bar\rho_\nu\Theta_2.
$$

Insert $\Theta_2=\psi_0 k^2\eta^2/6$. During [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), $a\propto\eta$, $\mathcal H=1/\eta$, and the [Friedmann equation](../../../cosmology.md#friedmann-equations) gives $8\pi Ga^2\bar\rho=3\mathcal H^2$. Thus

$$
\phi_0-\psi_0=\frac{16\pi G}{15}a^2\bar\rho_\nu\eta^2\psi_0
=\frac25 f_\nu\psi_0,
\qquad
\boxed{\phi_0=\left(1+\frac25f_\nu\right)\psi_0}.
$$

These are the [radiation-era adiabatic potentials with free-streaming neutrinos](../../../linear-cosmological-perturbation-theory.md#radiation-era-adiabatic-potentials-with-free-streaming-neutrinos); photons are taken to have negligible [scalar anisotropic stress](../../../linear-cosmological-perturbation-theory.md#scalar-anisotropic-stress).

To normalize the potentials, use $\bar P=\bar\rho/3$. The denominator in the [comoving curvature perturbation](../../../cosmic-inflation.md#comoving-curvature-perturbation) becomes

$$
4\pi Ga^2(\bar\rho+\bar P)=\frac{16\pi G}{3}a^2\bar\rho=2\mathcal H^2.
$$

With $\dot\phi=0$, the conserved curvature therefore obeys $\mathcal R=-\phi_0-\psi_0/2$. Combining it with the potential ratio gives

$$
\boxed{\psi_0(\mathbf k)=-\frac{10}{15+4f_\nu}\mathcal R(\mathbf k),\qquad
\phi_0(\mathbf k)=-\frac{10+4f_\nu}{15+4f_\nu}\mathcal R(\mathbf k)}.
$$

As a sign and normalization check, $f_\nu=0$ gives $\phi_0=\psi_0=-2\mathcal R/3$. Increasing the free-streaming radiation fraction increases $\phi_0/\psi_0$ while preserving the supplied curvature convention. The TeX's malformed definition of $\mathcal H$ is restored by the PDF: $\mathcal H=\dot a/a$.

## 4

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Put $\Gamma(\eta)=a\bar n_e\sigma_T\ge0$, the [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) rate per unit [conformal time](../../../cosmology.md#conformal-time). The [cosmological optical depth](../../../cosmic-microwave-background-anisotropy.md#cosmological-optical-depth) is the integrated scattering rate from emission time to observation, so a Poisson scattering process has survival probability

$$
\boxed{E(\eta)=e^{-\tau(\eta)}=\Pr(\text{no further scattering between }\eta\text{ and }\eta_0)}.
$$

Since $\dot\tau=-\Gamma$, the [cosmological visibility function](../../../cosmic-microwave-background-anisotropy.md#cosmological-visibility-function) is

$$
\boxed{g(\eta)=\Gamma(\eta)e^{-\tau(\eta)}=\frac{dE}{d\eta}}.
$$

A photon scatters in an interval $d\eta$ with rate factor $\Gamma d\eta$ and then reaches us without another scattering with probability $E$, so $g\,d\eta$ is its probability of last scattering in that interval. For an optically thick initial epoch,

$$
\int_{\eta_i}^{\eta_0}g(\eta)d\eta=1-e^{-\tau(\eta_i)}\simeq1.
$$

If the initial optical depth is finite, the missing weight represents photons that have already stopped scattering before $\eta_i$.

Before [cosmological recombination](../../../cosmology.md#recombination-cosmology), the optical depth to the present is enormous: $E\simeq0$, and $g$ is also small because almost every scattering is followed by another. Through [photon decoupling](../../../cosmology.md#photon-decoupling), $E$ rises rapidly and $g$ has its dominant positive peak. After decoupling, without [reionization](../../../cosmology.md#reionization), $E$ is close to one and reaches exactly one at $\eta_0$, while $g$ is small because the remaining electron density and scattering rate are small. Residual ionization can give a weak tail; there is no second reionization peak. The peak marks the [Cosmic microwave background last-scattering surface](../../../cosmology.md#cosmic-microwave-background-last-scattering-surface).

<a id="4/i/image-the-photon-visibility-function-during-recombination"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-312-visibility-sketch.png)

**[Figure 3](#4/i/image-the-photon-visibility-function-during-recombination). The photon visibility function during recombination**. Normalized schematic without reionization. The right curve is the derivative of the left curve and has unit area; the horizontal scale and width are illustrative, not a numerical recombination calculation.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Let $\Gamma=-\dot\tau=a\bar n_e\sigma_T$ and let $D=\partial_\eta+\mathbf e\cdot\nabla$ differentiate along the unperturbed photon trajectory. Use $1+(\mathbf e\cdot\hat{\mathbf m})^2=4/3+(2/3)P_2(\mathbf e\cdot\hat{\mathbf m})$ to decompose the [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) gain term:

$$
\frac{3\Gamma}{16\pi}\int d\hat{\mathbf m}\,\Theta(\hat{\mathbf m})[1+(\mathbf e\cdot\hat{\mathbf m})^2]
=\Gamma[\Theta_0+Q(\mathbf e)],
\quad
Q(\mathbf e)=\frac12\int\frac{d\hat{\mathbf m}}{4\pi}\Theta(\hat{\mathbf m})P_2(\mathbf e\cdot\hat{\mathbf m}).
$$

The [Orthogonality of Legendre polynomials](../../../differential-equation.md#orthogonality-of-legendre-polynomials) identifies $Q$ as a pure [photon quadrupole](../../../cosmic-microwave-background-anisotropy.md#photon-quadrupole). Dropping $Q$ is an approximation, justified when [tight coupling](../../../cosmic-microwave-background-anisotropy.md#tight-coupling-approximation) makes the scattering quadrupole small; the supplied unpolarized equation already neglects polarization corrections. The [Cosmic microwave background line-of-sight solution](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-line-of-sight-solution) requested here omits that quadrupole source.

Set $Y=\Theta+\psi$. Adding $D\psi=\dot\psi+\mathbf e\cdot\nabla\psi$ to the [Photon Boltzmann equation with Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#photon-boltzmann-equation-with-thomson-scattering) yields

$$
DY+\Gamma Y\simeq\dot\phi+\dot\psi+\Gamma(\Theta_0+\psi+\mathbf e\cdot\mathbf v_b).
$$

Along $\mathbf x(\eta)=\mathbf x_0-(\eta_0-\eta)\mathbf e$, the integrating factor is $e^{-\tau}$ because $d e^{-\tau}/d\eta=\Gamma e^{-\tau}$. Consequently

$$
\frac{d}{d\eta}[e^{-\tau}Y(\eta,\mathbf x(\eta),\mathbf e)]
\simeq e^{-\tau}(\dot\phi+\dot\psi)+g(\Theta_0+\psi+\mathbf e\cdot\mathbf v_b).
$$

An early optically thick boundary makes $e^{-\tau}Y$ vanish for finite initial perturbations, and $e^{-\tau(\eta_0)}=1$. Therefore

$$
\boxed{\begin{aligned}
\Theta(\eta_0,\mathbf x_0,\mathbf e)+\psi(\eta_0,\mathbf x_0)
&\simeq\int_{\eta_i}^{\eta_0}g(\eta)(\Theta_0+\psi+\mathbf e\cdot\mathbf v_b)(\eta,\mathbf x_0-\chi\mathbf e)d\eta\\
&\quad+\int_{\eta_i}^{\eta_0}e^{-\tau}(\dot\phi+\dot\psi)(\eta,\mathbf x_0-\chi\mathbf e)d\eta,
\end{aligned}}\qquad\chi=\eta_0-\eta.
$$

Here $\dot\phi$ and $\dot\psi$ are partial time derivatives, not total derivatives along the ray. We work at first order in [scalar cosmological perturbations](../../../linear-cosmological-perturbation-theory.md#scalar-cosmological-perturbation), evaluate sources along the background [radial null geodesic in FLRW spacetime](../../../cosmology.md#radial-null-geodesic-in-flrw-spacetime), and ignore observer peculiar velocity. Perturbed paths and lensing affect this first-order source solution only at higher perturbative order. A moving observer adds its local Doppler dipole.

The original PDF, unlike the transcribed TeX, also asks for the instantaneous-last-scattering limit and its interpretation. For $g(\eta)=\delta^{(D)}(\eta-\eta_*)$ with no later scattering, and a matter-era growing mode with constant $\phi$ and $\psi$, the [Integrated Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#integrated-sachs-wolfe-effect) vanishes. Hence

$$
\boxed{\Theta_{\rm obs}(\mathbf e)\simeq\Theta_0(\eta_*,\mathbf x_*)+\psi(\eta_*,\mathbf x_*)-\psi(\eta_0,\mathbf x_0)
+\mathbf e\cdot\mathbf v_b(\eta_*,\mathbf x_*),\quad\mathbf x_*=\mathbf x_0-\chi_*\mathbf e}.
$$

The four terms are the intrinsic emission temperature, the gravitational potential at emission, the observer's potential, and the [Doppler CMB anisotropy](../../../cosmic-microwave-background-anisotropy.md#doppler-cmb-anisotropy). The two potentials describe the gravitational redshift; the observer term is independent of direction and is absorbed into the measured temperature monopole. The intrinsic temperature and emission potential form the [Sachs-Wolfe combination](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-combination). On [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale) for [adiabatic initial conditions](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) in [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination), $\Theta_0=-2\psi/3$, giving the ordinary [Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-effect) $\Theta_0+\psi=\psi/3$. The Doppler sign is positive with the paper's propagation direction $\mathbf e$; the viewing direction is $-\mathbf e$.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Write $S_*(\mathbf x)=(\Theta_0+\psi)(\eta_*,\mathbf x)$ and $E=e^{-\tau_{\rm re}}$. Under the stated matter-era growing-mode approximation, $\dot\phi+\dot\psi=0$, and ignoring velocities removes the [Doppler CMB anisotropy](../../../cosmic-microwave-background-anisotropy.md#doppler-cmb-anisotropy). The two peaks of the [cosmological visibility function](../../../cosmic-microwave-background-anisotropy.md#cosmological-visibility-function) give the [Cosmic microwave background line-of-sight solution](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-line-of-sight-solution)

$$
Y_{\rm obs}(\mathbf e)=E S_*(\mathbf x_0-\chi_*\mathbf e)
+(1-E)(\Theta_0+\psi)(\eta_{\rm re},\mathbf x_0-\chi_{\rm re}\mathbf e),
\quad Y=\Theta+\psi.
$$

Apply the same solution with observation time $\eta_{\rm re}$, just before the thin [reionization](../../../cosmology.md#reionization) screen. Between recombination and that screen there is no further scattering, so free propagation gives

$$
Y(\eta_{\rm re},\mathbf x,\hat{\mathbf m})=S_*(\mathbf x-\Delta\chi\hat{\mathbf m}),
\qquad\Delta\chi=\eta_{\rm re}-\eta_*.
$$

A direction-independent potential commutes with the angular average. Thus the incoming [photon monopole](../../../cosmic-microwave-background-anisotropy.md#photon-monopole) plus the potential at the screen is

$$
(\Theta_0+\psi)(\eta_{\rm re},\mathbf x)
=\int\frac{d\hat{\mathbf m}}{4\pi}S_*(\mathbf x-\Delta\chi\hat{\mathbf m}).
$$

Substitution gives

$$
\boxed{Y_{\rm obs}(\mathbf e)=E S_*(\mathbf x_0-\chi_*\mathbf e)
+(1-E)\int\frac{d\hat{\mathbf m}}{4\pi}S_*(\mathbf x_0-\chi_{\rm re}\mathbf e-\Delta\chi\hat{\mathbf m})}.
$$

This derivation inherits the neglected scattering quadrupole and polarization assumptions of part (ii); the screen is an idealized isotropizing approximation.

For a plane [Fourier mode](../../../fourier-analysis.md#fourier-mode) $S_*(\mathbf x)=S_{\mathbf k}e^{i\mathbf k\cdot\mathbf x}$, the angular average is explicit:

$$
\frac12\int_{-1}^{1}e^{-ik\Delta\chi\mu}d\mu
=j_0(k\Delta\chi)=\frac{\sin(k\Delta\chi)}{k\Delta\chi},
$$

where $j_0$ is the zeroth [Spherical Bessel function](../../../analysis.md#spherical-bessel-function). The mode's observed transfer is

$$
Y_{\rm obs}=S_{\mathbf k}e^{i\mathbf k\cdot\mathbf x_0}
\left[E e^{-i\mathbf k\cdot\mathbf e\chi_*}+(1-E)j_0(k\Delta\chi)e^{-i\mathbf k\cdot\mathbf e\chi_{\rm re}}\right].
$$

If $k\Delta\chi\gg1$, the rescattered monopole is suppressed by at least $1/(k\Delta\chi)$, because the incoming directions sample incoherent phases. If $k\Delta\chi\ll1$, $j_0=1+O((k\Delta\chi)^2)$ and the two propagation phases agree to leading order. The two weights then sum to one. Consequently

$$
\boxed{Y_{\rm obs}(\mathbf e)\simeq\begin{cases}
 e^{-\tau_{\rm re}}S_*(\mathbf x_0-\chi_*\mathbf e),&k\Delta\chi\gg1,\\
 S_*(\mathbf x_0-\chi_*\mathbf e),&k\Delta\chi\ll1.
\end{cases}}
$$

These are the small-scale damping and large-scale coherence limits of [reionization damping of cosmic microwave background temperature anisotropy](../../../cosmology.md#reionization-damping-of-cosmic-microwave-background-temperature-anisotropy).

Each small-scale primary temperature amplitude is multiplied by $e^{-\tau_{\rm re}}$, so its [Cosmic microwave background power spectrum](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-power-spectrum) is multiplied by $e^{-2\tau_{\rm re}}$. Holding transfer parameters fixed,

$$
\boxed{C_\ell^{TT,\rm primary}\propto A_s e^{-2\tau_{\rm re}}\quad\text{on the damped angular scales}}.
$$

Many measured high-$\ell$ modes determine this combination accurately. Their derivatives $\partial\log C_\ell/\partial\log A_s=1$ and $\partial\log C_\ell/\partial\tau_{\rm re}=-2$ are degenerate: a change $d\log A_s=2d\tau_{\rm re}$ leaves the leading temperature spectrum unchanged. The undamped large-scale modes can distinguish the parameters, but there are few of them and [cosmic variance](../../../cosmic-microwave-background-anisotropy.md#cosmic-variance) gives fractional full-sky uncertainty $\sqrt{2/(2\ell+1)}$ per multipole. This explains the [primordial-amplitude–optical-depth degeneracy](../../../cosmology.md#primordial-amplitude-optical-depth-degeneracy). Polarization from reionization, lensing, and more complete late-time effects partly break it. The TeX's final $\tau_e$ is a transcription mismatch; the PDF uses $\tau_{\rm re}$ consistently.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
