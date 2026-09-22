<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

To first order, propagate along the unperturbed ray $\mathbf x(\eta)=\mathbf x_0-(\eta_0-\eta)\mathbf e$ and keep its [orthonormal tetrad](../../../../../../orthonormal-frame-in-spacetime.md) direction fixed. Corrections to direction or trajectory multiply an already first-order temperature source and are second order. Define the angular scattering source

$$
S(\eta,\mathbf x,\mathbf e)=\frac{3}{16\pi}\int d\Omega_{\mathbf m}\,\Theta(\eta,\mathbf x,\mathbf m)[1+(\mathbf e\cdot\mathbf m)^2].
$$

Using the [photon energy redshift from a tensor metric perturbation](../../../../../../photon-energy-redshift-from-a-tensor-metric-perturbation.md), the [Photon Boltzmann equation with Thomson scattering](../../../../../../photon-boltzmann-equation-with-thomson-scattering.md) along this ray becomes

$$
\frac{d\Theta}{d\eta}-\dot\tau\Theta=-\frac12\dot h_{ij}e^ie^j-\dot\tau S.
$$

Multiply by the survival probability $e^{-\tau}$. The [cosmological visibility function](../../../../../../cosmological-visibility-function.md) is $g(\eta)=-\dot\tau e^{-\tau}$, so integration gives

$$
\Theta_0=e^{-\tau_i}\Theta_i+\int_{\eta_i}^{\eta_0}gS\,d\eta-\frac12\int_{\eta_i}^{\eta_0}e^{-\tau}\dot h_{ij}e^ie^j\,d\eta.
$$

Every source here is evaluated on the same ray, and $\tau(\eta_0)=0$.

The instantaneous-visibility approximation makes $e^{-\tau}$ a step from zero to one at $\eta_*$. It suppresses the early boundary term and localizes the scattering source to $S_*$. To obtain only the requested [tensor CMB line-of-sight source](../../../../../../tensor-cmb-line-of-sight-source.md), additionally neglect this last-scattering angular source: in leading [tight coupling](../../../../../../tight-coupling-approximation.md), the tensor-induced incident quadrupole is small, and a tensor mode has no scalar monopole or dipole. Ignore later [reionization](../../../../../../reionization.md) and its scattering as well. Then

$$
\boxed{\Theta(\eta_0,\mathbf x_0,\mathbf e)\simeq-\frac12\int_{\eta_*}^{\eta_0}\dot h_{ij}(\eta,\mathbf x_0-(\eta_0-\eta)\mathbf e)e^ie^j\,d\eta.}
$$

**Instantaneous visibility alone would leave the term $S_*$; neglect of that term is an additional approximation.** The time derivative on $h$ is essential and is present in the PDF, although it was lost in the extracted TeX.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
