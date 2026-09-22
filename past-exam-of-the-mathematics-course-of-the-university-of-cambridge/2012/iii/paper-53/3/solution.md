<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A general [scalar cosmological perturbation](../../../../../scalar-cosmological-perturbation.md) has four scalar metric functions: a lapse perturbation, a scalar shift, a spatial curvature perturbation and a scalar spatial shear. The two scalar functions in a [cosmological gauge transformation](../../../../../gauge-transformation-in-cosmological-perturbation-theory.md) can set the shift and shear to zero. For nondegenerate spatial modes this gives [conformal Newtonian gauge](../../../../../newtonian-gauge.md), leaving the two potentials $\psi$ and $\phi$. The scalar traceless spatial Einstein equation makes their difference proportional to [scalar anisotropic stress](../../../../../scalar-anisotropic-stress.md). In general relativity, with no [scalar anisotropic stress](../../../../../scalar-anisotropic-stress.md) and the usual boundary conditions, **$\psi=\phi$**. Pressure alone does not spoil equality; free-streaming relativistic species can do so through their anisotropic stress.

Write $\Psi=(\phi+\psi)/2$, the [Weyl lensing potential](../../../../../weyl-lensing-potential.md). A conformal rescaling leaves the unparameterized [null geodesics](../../../../../null-geodesic.md) unchanged, although the affine parameter changes. To first order, the [conformal optical metric for scalar perturbations](../../../../../conformal-optical-metric-for-scalar-perturbations.md) has

$$
\widehat g_{00}=1+4\Psi,\qquad\widehat g_{0i}=0,\qquad
\widehat g_{ij}=-\delta_{ij}.
$$

The only nonzero connection coefficients at this order are

$$
\widehat\Gamma^0_{00}=2\partial_\eta\Psi,\qquad
\widehat\Gamma^0_{0i}=2\partial_i\Psi,\qquad
\widehat\Gamma^i_{00}=2\partial^i\Psi.
$$

Here spatial indices are raised with $\delta^{ij}$. An affine parameter $\lambda$ for this rescaled metric therefore obeys

$$
\begin{aligned}
\eta_{,\lambda\lambda}
+2\partial_\eta\Psi\,\eta_{,\lambda}^2
+4\partial_i\Psi\,x^i_{,\lambda}\eta_{,\lambda}&=0,\\
x^i_{,\lambda\lambda}+2\partial^i\Psi\,\eta_{,\lambda}^2&=0.
\end{aligned}
$$

The first line is also $\eta_{,\lambda\lambda}+2\eta_{,\lambda}d\Psi/d\lambda+2x^i_{,\lambda}\eta_{,\lambda}\partial_i\Psi=0$, since the derivative of the potential is along the ray.

Put $v^i=dx^i/d\eta$. The chain rule gives $x^i_{,\lambda\lambda}=\eta_{,\lambda}^2dv^i/d\eta+v^i\eta_{,\lambda\lambda}$. Eliminating the affine acceleration gives

$$
\boxed{\frac{dv^i}{d\eta}-2v^i\left(\frac{d\Psi}{d\eta}+v^j\partial_j\Psi\right)
+2\partial^i\Psi=0,\qquad
\frac{d\Psi}{d\eta}=\partial_\eta\Psi+v^j\partial_j\Psi.}
$$

The extra spatial-gradient term inside the parentheses does not replace the spatial term already contained in the total derivative.

At reception, the null condition is $|v|^2=1+4\Psi_0$. With the specified unit propagation vector $e$, this implies

$$
\boxed{v^i(\eta_0)=(1+2\Psi_0)e^i.}
$$

The zero-order trajectory is $x^i=e^i(\eta-\eta_0)$. In every term already containing a first-order potential, we may substitute $v=e$. Defining the transverse projector $P_\perp^{ij}=\delta^{ij}-e^ie^j$, the first-order [geodesic equation](../../../../../geodesic-equation.md) becomes

$$
\frac{d^2x^i}{d\eta^2}=2e^i\frac{d\Psi}{d\eta}
-2P_\perp^{ij}\partial_j\Psi.
$$

Integrating with the reception position and velocity gives the [first-order photon trajectory in scalar perturbations](../../../../../first-order-photon-trajectory-in-scalar-perturbations.md):

$$
\boxed{x^i(\eta)=e^i(\eta-\eta_0)+2e^i\int_{\eta_0}^{\eta}\Psi(\eta')\,d\eta'
-2\int_{\eta_0}^{\eta}(\eta-\eta')P_\perp^{ij}\partial_j\Psi(\eta')\,d\eta'.}
$$

Its first derivative at reception is $e^i+2e^i\Psi_0$, and differentiating twice gives the previous equation. For a first-order calculation, evaluating the integrals on the unperturbed ray is sufficient; shifting their evaluation points by the first-order displacement changes them only at second order. This is the [Born approximation in cosmological lensing](../../../../../born-approximation-in-cosmological-lensing.md).

To fix the angular-deflection sign, define $\chi_s=\eta_0-\eta_s>0$, $n_{\rm obs}=-e$, and $n_{\rm src}=x_s/|x_s|$. The latter is the unlensed coordinate direction to the source, while the former is its apparent direction measured by the observer. The longitudinal integral changes the radial distance, not the direction at this order. The transverse displacement is

$$
x_{s\perp}^i=-2\int_0^{\chi_s}(\chi_s-\chi)\partial_\perp^i
\Psi(\eta_0-\chi,-e\chi)\,d\chi.
$$

Dividing by $\chi_s$ yields

$$
\boxed{\alpha^i\equiv n_{\rm obs}^i-n_{\rm src}^i
=2\int_0^{\chi_s}\frac{\chi_s-\chi}{\chi_s}\,
\partial_\perp^i\Psi(\eta_0-\chi,-e\chi)\,d\chi.}
$$

This is the [angular deflection kernel for cosmological lensing](../../../../../angular-deflection-kernel-for-cosmological-lensing.md). It depends on the sum of the two metric potentials; setting them equal reduces it to the familiar twice-the-Newtonian-potential expression. With angular derivatives, the lensing potential is $2\int_0^{\chi_s}[(\chi_s-\chi)/(\chi_s\chi)]\Psi\,d\chi$, and its angular gradient is $\alpha$.

[Gravitational lensing](../../../../../gravitational-lensing.md) displaces apparent source positions and produces magnification and shear through angular derivatives of the deflection. [Weak gravitational lensing](../../../../../weak-gravitational-lensing.md) of galaxy shapes probes the foreground mass distribution, including [dark matter](../../../../../dark-matter.md). Lensing also remaps the [cosmic microwave background](../../../../../cosmic-microwave-background.md), smoothing its acoustic features and converting part of its E-mode polarization into B modes. Strong deflections can produce multiple images, though a single first-order ray calculation does not describe that regime completely.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
