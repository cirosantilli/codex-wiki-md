# Paper 76

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_76.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_76.pdf)

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

## 1

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the [time-harmonic wave](../../../physics.md#time-harmonic-wave) convention $\operatorname{Re}(\psi e^{-i\omega t})$, with a positive background [wavenumber](../../../wave-equation.md#wavenumber) $k$. The scalar [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) for a constant-density acoustic model is

$$
 \psi_{xx}+\psi_{zz}+k^2n^2\psi=0.
$$

Writing $\psi=e^{ikx}E$ gives the exact envelope equation

$$
 E_{xx}+2ikE_x+E_{zz}+k^2(n^2-1)E=0.
$$

The [paraxial approximation](../../../partial-differential-equation.md#paraxial-approximation) neglects $E_{xx}$ relative to $2ikE_x$, giving the [parabolic wave equation](../../../partial-differential-equation.md#parabolic-wave-equation)

$$
\boxed{2ikE_x+E_{zz}+k^2(n^2-1)E=0,\qquad
E_x=\frac{i}{2k}E_{zz}+\frac{ik}{2}(n^2-1)E.}
$$

The choice of carrier and the direction of propagation matter: this is a forward, slowly varying envelope approximation. Sufficient scale conditions are $|E_{xx}|\ll2k|E_x|$, transverse spectral components $|p|\ll k$, and medium/envelope variation on longitudinal scales large compared with $1/k$. With the carrier fixed at the background $k$, small $|n-1|$ makes the refractive phase vary slowly too. Large-angle propagation, appreciable backscattering, or rapid longitudinal variation violates the approximation. Acoustic models with variable [mass density](../../../fluid-mechanics.md#density) can have additional gradient terms, so the scalar [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) itself is a model assumption. For the [Gaussian beam](../../../optics.md#gaussian-beam) in part (b), useful initial conditions are $kD\gg1$ and $D/|F|\ll1$, with the second condition absent for an initially uncurved beam. A narrow angular spectrum, rather than merely the label “Gaussian”, justifies the [paraxial approximation](../../../partial-differential-equation.md#paraxial-approximation).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put

$$
 A=\frac1{D^2}+\frac{ik}{2F},\qquad
 q(x)=1+\frac{2iAx}{k}=1-\frac xF+\frac{2ix}{kD^2}.
$$

In free space, the [parabolic wave equation](../../../partial-differential-equation.md#parabolic-wave-equation) is $E_x=iE_{zz}/(2k)$. Under the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat E(p)=\int E(z)e^{-ipz}\,dz$, it becomes

$$
 \partial_x\widehat E=-\frac{ip^2}{2k}\widehat E,\qquad
 \widehat E(0,p)=\sqrt{\frac\pi A}\exp\left(-\frac{p^2}{4A}\right).
$$

The [Gaussian integral](../../../calculus.md#gaussian-integral) is legitimate because $\operatorname{Re}A=1/D^2>0$. Invert the transform after multiplying by $e^{-ip^2x/(2k)}$. A second [Gaussian integral](../../../calculus.md#gaussian-integral), or equivalently [one-dimensional transverse Fresnel propagation](../../../partial-differential-equation.md#one-dimensional-transverse-fresnel-propagation), gives

$$
\boxed{E(x,z)=q(x)^{-1/2}\exp\left(-\frac{Az^2}{q(x)}\right).}
$$

Choose the square-root branch continuously from $q(0)^{-1/2}=1$; for real $x\geq0$ there is no zero of $q$. This gives the correct incident field at $x=0$, and direct differentiation verifies the free [parabolic wave equation](../../../partial-differential-equation.md#parabolic-wave-equation).

For clarity, the squared envelope magnitude is

$$
 |E(x,z)|^2=\frac1{|q(x)|}\exp\left(-\frac{2z^2}{D^2|q(x)|^2}\right),\qquad
 D(x)=D\sqrt{(1-x/F)^2+\left(\frac{2x}{kD^2}\right)^2}.
$$

The [Gaussian beam with one transverse coordinate](../../../optics.md#gaussian-beam-with-one-transverse-coordinate) remains Gaussian, with one-transverse-coordinate amplitude factor $q^{-1/2}$, not the $q^{-1}$ of a beam with two transverse coordinates. The negative initial quadratic phase produces focusing for $F>0$; [diffraction](../../../quantum-mechanics.md#diffraction) prevents a singularity at $x=F$. These expressions describe the [paraxial approximation](../../../partial-differential-equation.md#paraxial-approximation) to free propagation, rather than an exact unrestricted [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) beam.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**No: the first moment generally depends on the transverse coordinate.** At entry to the [random medium](../../../physics.md#random-medium), the initial data are deterministic, so

$$
 m_1(x_0,z)=E_{\mathrm{free}}(x_0,z),
$$

which is a nonconstant [Gaussian beam](../../../optics.md#gaussian-beam) profile. [Statistical homogeneity](../../../probability-and-statistics.md#statistical-homogeneity) of the medium says that shifting both the medium and the incident data gives correspondingly shifted field statistics. It does not make the response to fixed, localized incident data translation invariant.

In particular, [Gaussian coherent-field propagation in the Markov approximation](../../../physics.md#gaussian-coherent-field-propagation-in-the-markov-approximation), derived in part (d), gives

$$
 m_1(x,z)=e^{-\gamma(x-x_0)}E_{\mathrm{free}}(x,z)
$$

for the linear weak-index model. A homogeneous attenuation factor multiplies the varying beam profile. Thus spatially homogeneous medium statistics can coexist with a transversely inhomogeneous [coherent field](../../../physics.md#coherent-wave-field). The first moment is not the [mean wave intensity](../../../physics.md#ensemble-averaged-wave-intensity), and disappearance of the coherent component is not itself disappearance of the total [wave energy](../../../wave-equation.md#wave-energy).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Write $m=\langle E\rangle$ and $L_0=i\partial_z^2/(2k)$. Substituting $n=1+\mu W$ into part (a), without prematurely replacing $n^2$ by its linear part, gives

$$
 E_x=L_0E+ik\mu WE+\frac{ik\mu^2}{2}W^2E.
$$

Taking the [expectation](../../../probability-theory.md#expected-value) yields the exact mean equation within the [paraxial approximation](../../../partial-differential-equation.md#paraxial-approximation):

$$
\boxed{m_x=L_0m+ik\mu\langle WE\rangle+
\frac{ik\mu^2}{2}\langle W^2E\rangle,
\qquad m(x_0,z)=E_{\mathrm{free}}(x_0,z).}
$$

The correlation term cannot be discarded just because $\langle W\rangle=0$: the field depends on the same [random medium](../../../physics.md#random-medium) as $W$. Nor can $\langle W^2E\rangle$ be factored exactly from the given [variance](../../../variance.md) alone. The printed statistics do not specify the [autocorrelation function of a random field](../../../stochastic-process.md#autocorrelation-function-of-a-random-field), so they do not determine a unique local closed equation for $m$.

A useful covariance-dependent equation follows to second order in $\mu$. Define

$$
 C(s,\eta)=\langle W(x,z)W(x-s,z-\eta)\rangle,\qquad C(0,0)=1,
$$

and let

$$
 G_s(\eta)=\sqrt{\frac{k}{2\pi is}}\exp\left(\frac{ik\eta^2}{2s}\right),\qquad s>0,
$$

be the [Fresnel propagator](../../../partial-differential-equation.md#fresnel-propagator) kernel for one transverse coordinate. The [Duhamel principle](../../../diffusion-equation.md#duhamel-s-principle) applied to the linear fluctuation term gives

$$
 E(x,z)=E^{(0)}(x,z)+ik\mu\int_{x_0}^x\!\int_{\mathbb R}
 G_{x-s}(z-\zeta)W(s,\zeta)E^{(0)}(s,\zeta)\,d\zeta\,ds+O(\mu^2),
$$

where $E^{(0)}=E_{\mathrm{free}}$. Multiply by $W(x,z)$ and average. Also $\langle W(x,z)^2E(x,z)\rangle=E^{(0)}(x,z)+O(\mu)$. Since $m=E^{(0)}+O(\mu^2)$, replacing $E^{(0)}$ by $m$ in terms already multiplied by $\mu^2$ preserves second-order accuracy. We obtain the [weak-fluctuation memory equation for the coherent field](../../../physics.md#weak-fluctuation-memory-equation-for-the-coherent-field)

$$
\boxed{\begin{aligned}
 m_x(x,z)&=L_0m(x,z)+\frac{ik\mu^2}{2}m(x,z)\\
 &\quad-k^2\mu^2\int_{x_0}^x\!\int_{\mathbb R}
 C(x-s,z-\zeta)G_{x-s}(z-\zeta)m(s,\zeta)\,d\zeta\,ds+O(\mu^3).
\end{aligned}}
$$

This perturbation statement is for fixed propagation intervals with sufficient covariance regularity and moment bounds. The kernel is understood as an oscillatory integral. If the field is jointly Gaussian, odd perturbative contributions vanish and the remainder can be improved under the corresponding expansion hypotheses. Joint Gaussianity itself still leaves the covariance unspecified. The term $ik\mu^2m/2$ is the [quadratic refractive-index shift in the coherent field](../../../physics.md#quadratic-refractive-index-shift-in-the-coherent-field); it comes from the mean of $W^2$.

For the usual local answer, impose the additional [Markov approximation for a random medium](../../../stochastic-process.md#markov-approximation-for-a-random-medium). Its longitudinal [correlation length](../../../critical-phenomenon.md#correlation-length) must be much shorter than the distance on which the envelope varies, and [diffraction](../../../quantum-mechanics.md#diffraction) across that correlation distance must not resolve substantial transverse covariance variation. Away from the entry layer, replace the slowly varying factors in the memory integral by their local values and extend the longitudinal integral to infinity. Define the integrated covariance

$$
 B(\eta)=\int_{-\infty}^{\infty}C(s,\eta)\,ds,\qquad
 \gamma=\frac{k^2\mu^2}{2}B(0)=k^2\mu^2\int_0^\infty C(s,0)\,ds.
$$

For an integrable real stationary covariance, $C(s,0)$ is even, and $B(0)\geq0$ is its zero-longitudinal-frequency spectral density. The conventional leading weak-index model keeps only the linear random potential $ik\mu W$; in that model the local first-moment equation is

$$
\boxed{m_x=\frac{i}{2k}m_{zz}-\gamma m.}
$$

The factor $1/2$ can be checked independently in the white-noise model. If $\mathcal B_x(z)$ is a [Brownian field](../../../brownian-motion.md#longitudinal-brownian-field-with-transverse-covariance) with $\langle d\mathcal B_x(z)d\mathcal B_x(z')\rangle=B(z-z')\,dx$, write

$$
 dE=L_0E\,dx+ik\mu E\circ d\mathcal B_x(z).
$$

Converting the [Stratonovich integral](../../../stochastic-calculus.md#stratonovich-integral) to an [Itô integral](../../../stochastic-calculus.md#ito-integral) adds $-k^2\mu^2B(0)E\,dx/2$. The remaining stochastic integral has zero mean, giving the boxed equation and

$$
\boxed{m(x,z)=e^{-\gamma(x-x_0)}q(x)^{-1/2}
\exp\left(-\frac{Az^2}{q(x)}\right).}
$$

If the finite-correlation model retains $n^2$ consistently through order $\mu^2$, the local second-order expansion also has $+ik\mu^2m/2$, adding the phase factor $e^{ik\mu^2(x-x_0)/2}$. This phase is computed before the white-noise idealization: squaring ideal [Gaussian white noise](../../../stochastic-process.md#gaussian-white-noise) is not the finite-variance operation $W^2$.

The need for a correlation assumption can be seen without any closure argument. The stationary [Gaussian random field](../../../stochastic-process.md#gaussian-random-field) $W(x,z)=Z$, with a single standard normal variable $Z$, has all the printed one-point statistics. In the linear weak-index model it gives

$$
 E=e^{ik\mu Z(x-x_0)}E_{\mathrm{free}},\qquad
 m=e^{-k^2\mu^2(x-x_0)^2/2}E_{\mathrm{free}}.
$$

Its attenuation is quadratic in propagation distance, whereas the Markov model gives linear-distance exponential attenuation. **The local attenuation equation requires the additional correlation/Markov assumption; it does not follow from [statistical homogeneity](../../../probability-and-statistics.md#statistical-homogeneity) and unit [variance](../../../variance.md) alone.**

## 2

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Take the same $e^{-i\omega t}$ convention and an outgoing field. Define the [scattering potential](../../../inverse-problem.md#scattering-potential) with the positive-contrast sign,

$$
 Q(\mathbf r)=k^2[n(\mathbf r)^2-1],\qquad
 (\Delta+k^2)\psi=-Q\psi.
$$

The [outgoing Green function for the three-dimensional Helmholtz equation](../../../partial-differential-equation.md#outgoing-green-function-for-the-three-dimensional-helmholtz-equation) is

$$
 G_k(\mathbf r,\mathbf r')=\frac{e^{ik|\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|},\qquad
 (\Delta+k^2)G_k=-\delta.
$$

Thus the [Lippmann-Schwinger equation](../../../quantum-mechanics.md#lippmann-schwinger-equation) has a plus sign:

$$
 \psi=\psi_i+T\psi,\qquad
 (T\phi)(\mathbf r)=\int_VG_k(\mathbf r,\mathbf r')Q(\mathbf r')\phi(\mathbf r')\,d^3r'.
$$

Replacing the total field inside the integral by the incident field gives the [Born approximation for scalar wave scattering](../../../inverse-problem.md#born-approximation-for-scalar-wave-scattering)

$$
\boxed{\psi_s^{(1)}(\mathbf r)=\frac{k^2}{4\pi}\int_V
 [n(\mathbf r')^2-1]\frac{e^{ik|\mathbf r-\mathbf r'|}}{|\mathbf r-\mathbf r'|}
 e^{ik\widehat{\mathbf r}_0\cdot\mathbf r'}\,d^3r'.}
$$

More generally, iterating the integral equation gives the [Born series](../../../inverse-problem.md#born-series) $\psi_s=\sum_{j\geq1}T^j\psi_i$; its first term is the boxed expression. A sufficient convergence condition is $\|T\|<1$ on the chosen space of fields in $V$, and accurate single-scattering truncation needs the neglected terms to be small. Weak refractive contrast is useful, but for a sufficiently large or resonant scatterer it is not by itself a guarantee of negligible [multiple scattering](../../../physics.md#multiple-scattering).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $\mathbf r=R\widehat{\mathbf r}$ with the observation distance much larger than the scatterer, expand $|\mathbf r-\mathbf r'|=R-\widehat{\mathbf r}\cdot\mathbf r'+O(R^{-1})$. The [far-field pattern](../../../inverse-problem.md#far-field-pattern) in the [Born approximation for scalar wave scattering](../../../inverse-problem.md#born-approximation-for-scalar-wave-scattering) is consequently

$$
 \psi_s^{(1)}(R\widehat{\mathbf r})=\frac{e^{ikR}}R
 f_\infty^{(1)}(\widehat{\mathbf r},\widehat{\mathbf r}_0)+O(R^{-2}),
$$



$$
\boxed{f_\infty^{(1)}=\frac{k^2}{4\pi}\int_V[n(\mathbf r')^2-1]
 e^{-i\mathbf k_s\cdot\mathbf r'}\,d^3r',\qquad
 \mathbf k_s=k(\widehat{\mathbf r}-\widehat{\mathbf r}_0).}
$$

This convention includes the factor $1/(4\pi)$ in $f_\infty$; moving that factor into the outgoing-wave definition would change the pattern's normalization.

The absolute [energy flux](../../../physics.md#energy-flux) depends on what physical amplitude $\psi$ represents. For acoustic [pressure](../../../thermodynamics.md#pressure) in a homogeneous fluid of [mass density](../../../fluid-mechanics.md#density) $\rho_0$ and [wave speed](../../../wave-equation.md#wave-speed) $c_0$, the momentum equation gives the particle-velocity amplitude $\mathbf v=\nabla\psi/(i\rho_0\omega)$. The [time average of harmonic power](../../../linear-acoustics.md#time-average-of-harmonic-power) and [acoustic intensity](../../../continuum-mechanics.md#acoustic-energy-flux) then give

$$
 \langle\mathbf I\rangle=\frac12\operatorname{Re}(\psi\mathbf v^*)
 =\frac1{2\rho_0\omega}\operatorname{Im}(\psi^*\nabla\psi).
$$

The radial derivative of the outgoing factor is $(ik-1/R)e^{ikR}/R$. Its imaginary current is therefore $k|f_\infty|^2/R^2$ to leading order. The incident unit-amplitude [plane wave](../../../quantum-mechanics.md#plane-wave) has imaginary current $k\widehat{\mathbf r}_0$. Hence, with $k=\omega/c_0$,

$$
\boxed{E_s(R)=\frac{k}{2\rho_0\omega R^2}|f_\infty^{(1)}|^2+O(R^{-3}),\qquad
 E_i=\frac{k}{2\rho_0\omega}=\frac1{2\rho_0c_0}.}
$$

The scattered [energy flux](../../../physics.md#energy-flux) points along $\widehat{\mathbf r}$ at leading order, and the incident [energy flux](../../../physics.md#energy-flux) along $\widehat{\mathbf r}_0$. If $\psi$ is a velocity-potential amplitude instead, both leading expressions use the common prefactor $\rho_0\omega k/2$ in place of $k/(2\rho_0\omega)$. A normalized scalar current uses $k$ as the common prefactor. The paper does not specify this amplitude normalization; the ratio in part (c) is independent of that choice.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use the same physical normalization for both fields. Part (b) has $E_s=E_i|f_\infty^{(1)}|^2/R^2+O(R^{-3})$, so the common [energy flux](../../../physics.md#energy-flux) prefactor cancels. The [differential cross-section for scalar wave scattering](../../../physics.md#differential-cross-section-for-scalar-wave-scattering) is

$$
\boxed{\sigma_d^{(1)}(\widehat{\mathbf r},\widehat{\mathbf r}_0)
 =|f_\infty^{(1)}(\widehat{\mathbf r},\widehat{\mathbf r}_0)|^2
 =\frac{k^4}{16\pi^2}\left|\int_V(n^2-1)e^{-i\mathbf k_s\cdot\mathbf r}\,d^3r\right|^2.}
$$

The [far-field pattern](../../../inverse-problem.md#far-field-pattern) has dimensions of length in this normalization, so the [differential cross-section for scalar wave scattering](../../../physics.md#differential-cross-section-for-scalar-wave-scattering) has dimensions of area per unit [solid angle](../../../geometry-and-topology.md#solid-angle). Only the scattered field is used in this ratio; interference between the incident and scattered fields is a different contribution to the total field's [energy flux](../../../physics.md#energy-flux).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let the medium's [autocorrelation function of a random field](../../../stochastic-process.md#autocorrelation-function-of-a-random-field) and [power spectrum](../../../probability-and-statistics.md#power-spectrum) use the explicit convention

$$
 C(\mathbf s)=\langle W(\mathbf r+\mathbf s)W(\mathbf r)\rangle,\qquad
 S_W(\mathbf q)=\int_{\mathbb R^3}C(\mathbf s)e^{-i\mathbf q\cdot\mathbf s}\,d^3s,
$$



$$
 C(\mathbf s)=\frac1{(2\pi)^3}\int_{\mathbb R^3}S_W(\mathbf q)e^{i\mathbf q\cdot\mathbf s}\,d^3q.
$$

Since $n^2-1=2\mu W+\mu^2W^2$, only the linear term in $\mu$ is needed to obtain the cross-section through second order:

$$
 f_\infty^{(1)}=\frac{\mu k^2}{2\pi}\int_VW(\mathbf r)e^{-i\mathbf k_s\cdot\mathbf r}\,d^3r+O(\mu^2).
$$

Squaring and taking the [expectation](../../../probability-theory.md#expected-value) gives

$$
\boxed{\langle\sigma_d\rangle=
\frac{\mu^2k^4}{4\pi^2}\int_V\!\int_V
 C(\mathbf r-\mathbf r')e^{-i\mathbf k_s\cdot(\mathbf r-\mathbf r')}\,d^3r\,d^3r'
 +O(\mu^3).}
$$

This is the finite-volume formula in the [Born approximation for scalar wave scattering](../../../inverse-problem.md#born-approximation-for-scalar-wave-scattering); the zero mean of $W$ does not make its squared scattered amplitude vanish. For a jointly centered [Gaussian random field](../../../stochastic-process.md#gaussian-random-field), the third-order contribution is zero, so the next perturbative contribution is fourth order when that expansion is valid.

Introduce the overlap volume $H_V(\mathbf s)=|V\cap(V-\mathbf s)|$. Changing variables rewrites the double integral as

$$
 \int_{\mathbb R^3}H_V(\mathbf s)C(\mathbf s)e^{-i\mathbf k_s\cdot\mathbf s}\,d^3s.
$$

When the linear dimensions of a regular scattering volume are large compared with the [correlation length](../../../critical-phenomenon.md#correlation-length), and $C$ is integrable, $H_V(\mathbf s)\simeq|V|$ over the significant covariance range. This gives the [finite-volume random scattering spectrum](../../../physics.md#finite-volume-random-scattering-spectrum) result

$$
\boxed{\langle\sigma_d(\widehat{\mathbf r},\widehat{\mathbf r}_0)\rangle
 \simeq\frac{\mu^2k^4|V|}{4\pi^2}S_W(\mathbf k_s),\qquad
 \mathbf k_s=k(\widehat{\mathbf r}-\widehat{\mathbf r}_0).}
$$

There are two distinct approximations here: the weak-scattering expansion in $\mu$ and the negligible-boundary-overlap approximation in the volume-to-correlation-scale ratio. If $S$ instead denotes the [power spectrum](../../../probability-and-statistics.md#power-spectrum) of the index fluctuation $n-1=\mu W$, then $S=\mu^2S_W$ and the external factor $\mu^2$ is absorbed into $S$.

[Statistical homogeneity](../../../probability-and-statistics.md#statistical-homogeneity) alone allows an anisotropic spectrum, so its argument is generally the vector $\mathbf k_s$. If [statistical isotropy](../../../probability-and-statistics.md#statistical-isotropy) is additionally assumed, $S_W$ depends only on

$$
\boxed{k_s=|\mathbf k_s|=2k\sin(\theta/2),\qquad
 \cos\theta=\widehat{\mathbf r}\cdot\widehat{\mathbf r}_0.}
$$

The scalar notation $S(k_s)$ is valid in that isotropic case. For the alternative convention $S_{\mathrm{norm}}=(2\pi)^{-3}S_W$, the bulk formula is $2\pi\mu^2k^4|V|S_{\mathrm{norm}}(\mathbf k_s)$. Changing the sign of the scattering vector does not change the spectrum of a real stationary scalar field; changing the [Fourier transform](../../../analysis.md#fourier-transform) normalization does change the displayed $2\pi$ factors. Both conventions have therefore been stated explicitly.

## 3

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For noisy data, exact equality $Ax=y$ may be impossible: the data can have a component outside the [operator range](../../../topological-vector-space.md#range-of-a-bounded-linear-operator). A [least-squares solution of a linear inverse problem](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) instead minimizes

$$
 J(x)=\frac12\|Ax-y\|_Y^2.
$$

For any variation $h\in X$, the [adjoint operator](../../../hilbert-space.md#adjoint-operator) gives

$$
 DJ(x)[h]=\operatorname{Re}\langle Ax-y,Ah\rangle_Y
 =\operatorname{Re}\langle A^*(Ax-y),h\rangle_X.
$$

Thus [statistical homogeneity](../../../probability-and-statistics.md#statistical-homogeneity) in every direction is the [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem), $A^*Ax=A^*y$. It is also sufficient for a global minimum: when it holds,

$$
\boxed{J(x+h)-J(x)=\frac12\|Ah\|_Y^2\geq0.}
$$

The residual is orthogonal to the closure of the range, since it lies in $\ker A^*$. A normal-equation solution therefore fits the component of the data representable by the forward map, while leaving the perpendicular component unfitted. If there is more than one such solution, select the [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution), which lies in $(\ker A)^\perp$.

These facts explain the formulation, but do not make the inverse problem well posed. A [compact operator](../../../compact-operator.md) of infinite rank typically has nonclosed [operator range](../../../topological-vector-space.md#range-of-a-bounded-linear-operator), so even the least-squares infimum need not be attained. A [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) exists exactly when the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) of $y$ onto $\overline{\operatorname{Ran}A}$ belongs to $\operatorname{Ran}A$. In a [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator), this becomes the [Picard criterion](../../../inverse-problem.md#picard-criterion). Also, the nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $A^*A$ are the squares of the [singular values](../../../linear-algebra.md#singular-value) of $A$: solving the [operator normal equation](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) directly can worsen numerical conditioning. **The [operator normal equation](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) expresses least squares; it does not itself regularize the inverse problem.** The subsequent finite [Landweber iteration](../../../inverse-problem.md#landweber-iteration) and its stopping rule provide the [inverse-problem regularization](../../../inverse-problem.md#regularization-of-an-inverse-problem).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose a fixed positive [Landweber relaxation parameter](../../../inverse-problem.md#landweber-relaxation-parameter) $\tau$ and rearrange the [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) as the [fixed point](../../../function.md#fixed-point) equation

$$
 x=(I-\tau A^*A)x+\tau A^*y.
$$

Successive substitution gives [Landweber iteration](../../../inverse-problem.md#landweber-iteration)

$$
\boxed{x_{n+1}=x_n+\tau A^*(y-Ax_n),\qquad x_0=0.}
$$

Set $B=A^*A$ and $P=I-\tau B$. Induction yields the closed polynomial-operator expression

$$
\boxed{x_n=\tau\sum_{j=0}^{n-1}P^jA^*y
 =h_n(B)A^*y,\qquad
 h_n(t)=\begin{cases}\dfrac{1-(1-\tau t)^n}{t},&t\ne0,\\n\tau,&t=0.\end{cases}}
$$

For $n=0$ the sum is empty, giving zero. The expression is well defined without an inverse of $A^*A$, which can have a [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) and an unbounded inverse on its range. Each iterate lies in the closure of $\operatorname{Ran}A^*$, so initialization at zero eliminates the arbitrary null-space component of a solution. The unrelaxed choice $\tau=1$ gives $x_{n+1}=(I-A^*A)x_n+A^*y$ and the corresponding sum with $\tau=1$; it needs the convergence restriction in part (d).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the convention required by the printed expansion:

$$
 Av_i=\sigma_i u_i,\qquad A^*u_i=\sigma_i v_i,\qquad \sigma_i>0,
$$

where $u_i\in Y$ and $v_i\in X$ form the positive-singular-value parts of the [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator). Consequently $A^*Av_i=\sigma_i^2v_i$. Apply part (b)'s polynomial to each such [eigenvector](../../../linear-operator-theory.md#eigenvector), using noisy data:

$$
 x_n^{(\delta)}=\sum_i\tau\sigma_i\sum_{j=0}^{n-1}(1-\tau\sigma_i^2)^j
 \langle y^{(\delta)},u_i\rangle v_i.
$$

The [geometric series](../../../real-analysis.md#geometric-series) then gives the full inverse coefficient, or [Landweber full inverse filter](../../../inverse-problem.md#landweber-full-inverse-filter),

$$
\boxed{g_\alpha(\sigma)=\frac{1-(1-\tau\sigma^2)^{1/\alpha}}{\sigma},
\qquad \alpha=1/n,\quad n\in\mathbb N.}
$$

In particular, for the unrelaxed iteration $\tau=1$, $g_\alpha(\sigma)=[1-(1-\sigma^2)^{1/\alpha}]/\sigma$. The dimensionless [Landweber spectral filter](../../../inverse-problem.md#landweber-spectral-filter) is instead $\sigma g_\alpha(\sigma)$; the printed expression uses the full coefficient and therefore needs the denominator $\sigma$.

For each fixed finite $n$, the filter extends continuously at zero by $g_{1/n}(0)=0$, since $g_{1/n}(\sigma)=n\tau\sigma+O(\sigma^3)$ as $\sigma\to0$. Small [singular values](../../../linear-algebra.md#singular-value) are suppressed rather than immediately divided into noisy data. A component of $y^{(\delta)}$ in $\ker A^*$ contributes nothing. The parameter here is discrete: $1/\alpha$ is an integer. This matters when $1-\tau\sigma^2<0$; arbitrary real powers are not intended. A family for every $\alpha>0$ can use $n=\lfloor1/\alpha\rfloor$ instead.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For nonzero $A$, a sufficient step-size condition for [strong convergence of relaxed Landweber iteration](../../../inverse-problem.md#strong-convergence-of-relaxed-landweber-iteration) is

$$
\boxed{0<\tau<\frac2{\|A\|^2}.}
$$

For the unrelaxed iteration, this reads $\|A\|^2<2$. The data must also admit a [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution) $x^\dagger$; for the exact problem, $y\in\operatorname{Ran}A$ is sufficient. More generally, the projected-data condition in part (a), or the [Picard criterion](../../../inverse-problem.md#picard-criterion) $\sum_i|\langle y,u_i\rangle|^2/\sigma_i^2<\infty$, ensures the required solution.

Every positive [singular value](../../../linear-algebra.md#singular-value) satisfies $|1-\tau\sigma_i^2|<1$, so for fixed $\sigma_i>0$,

$$
\boxed{\lim_{\alpha\to0}g_\alpha(\sigma_i)=\frac1{\sigma_i}.}
$$

This is the correct inverse coefficient. For exact data with a [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem), the [norm](../../../functional-analysis.md#norm) error is

$$
 \|x_n-x^\dagger\|^2=\sum_i
 |1-\tau\sigma_i^2|^{2n}\frac{|\langle y,u_i\rangle|^2}{\sigma_i^2}\longrightarrow0.
$$

The summable majorant is precisely the [Picard criterion](../../../inverse-problem.md#picard-criterion), so the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) proves strong convergence, despite the absence of a uniform contraction constant when the [singular values](../../../linear-algebra.md#singular-value) approach zero. Initialization at zero selects the solution orthogonal to $\ker A$. At $\tau=2/\|A\|^2$, a top singular mode of a nonzero [compact operator](../../../compact-operator.md) has multiplier $-1$ and can oscillate indefinitely; the strict step bound avoids this failure.

Pointwise convergence of filters alone is not a full noisy-data [inverse-problem regularization](../../../inverse-problem.md#regularization-of-an-inverse-problem) proof. For each finite $n$, put $t=\tau\sigma^2$; the step restriction gives $|1-t|\leq1$, and

$$
 |1-(1-t)^n|\leq\min(nt,2),\qquad
 |g_{1/n}(\sigma)|\leq\min(n\tau\sigma,2/\sigma)\leq\sqrt{2n\tau}.
$$

This proves the [uniform noise bound for relaxed Landweber iteration](../../../inverse-problem.md#uniform-noise-bound-for-relaxed-landweber-iteration)

$$
 \|x_n^{(\delta)}-x_n\|\leq\delta\sqrt{2n\tau}.
$$

Together with the exact-data convergence,

$$
\boxed{\|x_n^{(\delta)}-x^\dagger\|
 \leq\delta\sqrt{2n\tau}+\|x_n-x^\dagger\|\longrightarrow0}
$$

whenever $n=n(\delta)\to\infty$ and $\delta\sqrt{n(\delta)}\to0$. Equivalently, the [a priori regularization parameter choice](../../../inverse-problem.md#a-priori-regularization-parameter-choice) satisfies $\alpha(\delta)\to0$ and $\delta/\sqrt{\alpha(\delta)}\to0$. For example, $n(\delta)=\lfloor\delta^{-1}\rfloor$ works as $\delta\to0$. The sharper familiar bound $\delta\sqrt{n\tau}$ is available when $\tau\|A\|^2\leq1$.

Thus **finite iteration followed by an appropriate stopping rule is a [convergent regularization of an inverse problem](../../../inverse-problem.md#convergent-regularization-of-an-inverse-problem)**. Taking $n\to\infty$ for fixed noisy data is not the same operation and can amplify the small-singular-value noise without bound. If $A=0$, the zero starting iterate stays zero and is the [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution) for every datum; the step restriction is needed only for nonzero $A$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
