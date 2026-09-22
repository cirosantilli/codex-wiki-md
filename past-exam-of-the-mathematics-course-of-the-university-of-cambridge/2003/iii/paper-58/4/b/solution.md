<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use one [Fourier mode](../../../../../../fourier-mode.md), with $\mu=\widehat{\mathbf k}\cdot\widehat{\mathbf n}$ and unperturbed ray $\mathbf x(\tau)=\widehat{\mathbf n}(\tau_0-\tau)$. Put $E(\tau)=e^{ik\mu(\tau_0-\tau)}$, and let $\tau_*$ denote last scattering. In the supplied branch $h'=h_s'$, the scalar decomposition gives

$$
h_{ij}'n_in_j=h'/3+h_s'(\mu^2-1/3)=\mu^2h_s'.
$$

Since $E''=-k^2\mu^2E$, two [integrations by parts](../../../../../../integration-by-parts.md) give the exact endpoint decomposition of the metric contribution:

$$
-\frac{\mu^2}{2}\int_{\tau_*}^{\tau_0}h_s'E\,d\tau
=\frac{[h_s'E'-h_s''E]_{\tau_*}^{\tau_0}}{2k^2}
+\frac1{2k^2}\int_{\tau_*}^{\tau_0}h_s'''E\,d\tau.
$$

For the matter-era growing mode, $h_s$ is quadratic in $\tau$, so the last integral vanishes. With $E'=-ik\mu E$, the emission endpoint is

$$
E_*\left(\frac{h_s''}{2k^2}+\frac{i\mu h_s'}{2k}\right)_*,
$$

and the observer endpoint is $-h_s''(\tau_0)/(2k^2)-i\mu h_s'(\tau_0)/(2k)$. The observer terms are only a [angular monopole](../../../../../../angular-monopole.md) and [angular dipole](../../../../../../angular-dipole.md); they are removed when studying the anisotropy multipoles $\ell\geq2$.

For an adiabatic growing mode outside the horizon at last scattering, $\delta_\gamma=4\delta_m/3$, $\delta_m=-h/2$ after fixing the constant trace convention, and $h\propto\tau^2$. Hence the intrinsic emission term is smaller than $h_s''/(2k^2)$ by order $(k\tau_*)^2$. The derivative emission endpoint is smaller by order $k\tau_*$. [Stress-energy conservation](../../../../../../stress-energy-conservation.md) also makes the peculiar emission velocity subleading; its leading synchronous contribution cancels in $\delta_\gamma'+2h'/3$, with gradients supplying the remaining small term. Keeping the Fourier phase, which need not be small over the observer's distance, gives

$$
\boxed{\Theta(\widehat{\mathbf n})\simeq\frac{h_s''(\tau_*)}{2k^2}e^{i\mathbf k\cdot\widehat{\mathbf n}\chi_*},\qquad \chi_*=\tau_0-\tau_*.}
$$

Here $\Theta=\delta T/T$, and the sum over modes is understood. The derivative is the **second derivative of $h_s$**, as printed in the original PDF. This approximation assumes matter-era growing adiabatic modes and neglects late evolving potentials; large wavelength alone does not remove the last integral in a general cosmology. The equality $h'=h_s'$ is used as the supplied synchronous condition, rather than as a general identity for every fluid solely from vanishing anisotropic stress.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
