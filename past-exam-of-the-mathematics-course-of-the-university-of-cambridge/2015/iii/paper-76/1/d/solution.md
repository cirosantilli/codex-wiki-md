<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $m=\langle E\rangle$ and $L_0=i\partial_z^2/(2k)$. Substituting $n=1+\mu W$ into part (a), without prematurely replacing $n^2$ by its linear part, gives

$$
 E_x=L_0E+ik\mu WE+\frac{ik\mu^2}{2}W^2E.
$$

Taking the [expectation](../../../../../../expected-value.md) yields the exact mean equation within the [paraxial approximation](../../../../../../paraxial-approximation.md):

$$
\boxed{m_x=L_0m+ik\mu\langle WE\rangle+
\frac{ik\mu^2}{2}\langle W^2E\rangle,
\qquad m(x_0,z)=E_{\mathrm{free}}(x_0,z).}
$$

The correlation term cannot be discarded just because $\langle W\rangle=0$: the field depends on the same [random medium](../../../../../../random-medium.md) as $W$. Nor can $\langle W^2E\rangle$ be factored exactly from the given [variance](../../../../../../variance-split.md) alone. The printed statistics do not specify the [autocorrelation function of a random field](../../../../../../autocorrelation-function-of-a-random-field.md), so they do not determine a unique local closed equation for $m$.

A useful covariance-dependent equation follows to second order in $\mu$. Define

$$
 C(s,\eta)=\langle W(x,z)W(x-s,z-\eta)\rangle,\qquad C(0,0)=1,
$$

and let

$$
 G_s(\eta)=\sqrt{\frac{k}{2\pi is}}\exp\left(\frac{ik\eta^2}{2s}\right),\qquad s>0,
$$

be the [Fresnel propagator](../../../../../../fresnel-propagator.md) kernel for one transverse coordinate. The [Duhamel principle](../../../../../../duhamel-s-principle.md) applied to the linear fluctuation term gives

$$
 E(x,z)=E^{(0)}(x,z)+ik\mu\int_{x_0}^x\!\int_{\mathbb R}
 G_{x-s}(z-\zeta)W(s,\zeta)E^{(0)}(s,\zeta)\,d\zeta\,ds+O(\mu^2),
$$

where $E^{(0)}=E_{\mathrm{free}}$. Multiply by $W(x,z)$ and average. Also $\langle W(x,z)^2E(x,z)\rangle=E^{(0)}(x,z)+O(\mu)$. Since $m=E^{(0)}+O(\mu^2)$, replacing $E^{(0)}$ by $m$ in terms already multiplied by $\mu^2$ preserves second-order accuracy. We obtain the [weak-fluctuation memory equation for the coherent field](../../../../../../weak-fluctuation-memory-equation-for-the-coherent-field.md)

$$
\boxed{\begin{aligned}
 m_x(x,z)&=L_0m(x,z)+\frac{ik\mu^2}{2}m(x,z)\\
 &\quad-k^2\mu^2\int_{x_0}^x\!\int_{\mathbb R}
 C(x-s,z-\zeta)G_{x-s}(z-\zeta)m(s,\zeta)\,d\zeta\,ds+O(\mu^3).
\end{aligned}}
$$

This perturbation statement is for fixed propagation intervals with sufficient covariance regularity and moment bounds. The kernel is understood as an oscillatory integral. If the field is jointly Gaussian, odd perturbative contributions vanish and the remainder can be improved under the corresponding expansion hypotheses. Joint Gaussianity itself still leaves the covariance unspecified. The term $ik\mu^2m/2$ is the [quadratic refractive-index shift in the coherent field](../../../../../../quadratic-refractive-index-shift-in-the-coherent-field.md); it comes from the mean of $W^2$.

For the usual local answer, impose the additional [Markov approximation for a random medium](../../../../../../markov-approximation-for-a-random-medium.md). Its longitudinal [correlation length](../../../../../../correlation-length.md) must be much shorter than the distance on which the envelope varies, and [diffraction](../../../../../../diffraction.md) across that correlation distance must not resolve substantial transverse covariance variation. Away from the entry layer, replace the slowly varying factors in the memory integral by their local values and extend the longitudinal integral to infinity. Define the integrated covariance

$$
 B(\eta)=\int_{-\infty}^{\infty}C(s,\eta)\,ds,\qquad
 \gamma=\frac{k^2\mu^2}{2}B(0)=k^2\mu^2\int_0^\infty C(s,0)\,ds.
$$

For an integrable real stationary covariance, $C(s,0)$ is even, and $B(0)\geq0$ is its zero-longitudinal-frequency spectral density. The conventional leading weak-index model keeps only the linear random potential $ik\mu W$; in that model the local first-moment equation is

$$
\boxed{m_x=\frac{i}{2k}m_{zz}-\gamma m.}
$$

The factor $1/2$ can be checked independently in the white-noise model. If $\mathcal B_x(z)$ is a [Brownian field](../../../../../../longitudinal-brownian-field-with-transverse-covariance.md) with $\langle d\mathcal B_x(z)d\mathcal B_x(z')\rangle=B(z-z')\,dx$, write

$$
 dE=L_0E\,dx+ik\mu E\circ d\mathcal B_x(z).
$$

Converting the [Stratonovich integral](../../../../../../stratonovich-integral.md) to an [Itô integral](../../../../../../ito-integral.md) adds $-k^2\mu^2B(0)E\,dx/2$. The remaining stochastic integral has zero mean, giving the boxed equation and

$$
\boxed{m(x,z)=e^{-\gamma(x-x_0)}q(x)^{-1/2}
\exp\left(-\frac{Az^2}{q(x)}\right).}
$$

If the finite-correlation model retains $n^2$ consistently through order $\mu^2$, the local second-order expansion also has $+ik\mu^2m/2$, adding the phase factor $e^{ik\mu^2(x-x_0)/2}$. This phase is computed before the white-noise idealization: squaring ideal [Gaussian white noise](../../../../../../gaussian-white-noise.md) is not the finite-variance operation $W^2$.

The need for a correlation assumption can be seen without any closure argument. The stationary [Gaussian random field](../../../../../../gaussian-random-field.md) $W(x,z)=Z$, with a single standard normal variable $Z$, has all the printed one-point statistics. In the linear weak-index model it gives

$$
 E=e^{ik\mu Z(x-x_0)}E_{\mathrm{free}},\qquad
 m=e^{-k^2\mu^2(x-x_0)^2/2}E_{\mathrm{free}}.
$$

Its attenuation is quadratic in propagation distance, whereas the Markov model gives linear-distance exponential attenuation. **The local attenuation equation requires the additional correlation/Markov assumption; it does not follow from [statistical homogeneity](../../../../../../statistical-homogeneity.md) and unit [variance](../../../../../../variance-split.md) alone.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
