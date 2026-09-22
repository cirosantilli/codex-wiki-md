<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In the non-scattering [grey atmosphere](../../../../grey-atmosphere.md) approximation, $I$ is the frequency-integrated [specific intensity](../../../../spectral-radiance.md) along a ray, $s$ is distance along that ray, $\rho$ is the [mass density](../../../../density.md), and $\kappa$ is the [mass absorption coefficient](../../../../mass-absorption-coefficient.md). The [local thermodynamic equilibrium](../../../../local-thermodynamic-equilibrium.md) source is the frequency-integrated [Planck function](../../../../planck-function.md) $B=\sigma_{\rm SB}T^4/\pi$. Across a thin element $ds$, absorption removes $\kappa\rho I\,ds$ and thermal emission adds $\kappa\rho B\,ds$. Their balance gives $dI/ds=-\kappa\rho(I-B)$.

Take the upward vertical as the polar axis, put $\mu=\cos\theta$, and define downward [optical depth](../../../../optical-depth.md) by

$$
\boxed{\tau(z)=\int_z^\infty\kappa(z')\rho(z')\,dz'.}
$$

Along a ray, $dz/ds=\mu$ and $d\tau/ds=-\kappa\rho\mu$. The [chain rule](../../../../chain-rule.md) therefore gives $\boxed{\mu I_\tau=I-B}$. In a plane-parallel, azimuthally symmetric field, the [solid angle](../../../../solid-angle.md) element is $d\omega=d\varphi\,d\mu$, so

$$
\boxed{J(\tau)=\frac12\int_{-1}^{1}I(\tau,\mu)\,d\mu.}
$$

[Local radiative equilibrium](../../../../local-radiative-equilibrium.md) requires zero net radiative heating of the material: absorption $4\pi\kappa\rho J$ balances emission $4\pi\kappa\rho B$. Where the absorption coefficient is nonzero this gives $B=J$, and substitution gives the required angular [radiative transfer equation](../../../../radiative-transfer-equation.md). It does not require the [specific intensity](../../../../spectral-radiance.md) itself to be isotropic.

At the top of an atmosphere with no external incoming long-wave radiation, impose $\boxed{I(0,\mu)=0\quad(-1\leq\mu<0)}$. These are inward directions; prescribing the same zero value for outward directions would remove the emergent radiation as well. The upward [radiative flux](../../../../radiative-flux.md) and its derivative are

$$
\Phi=2\pi\int_{-1}^{1}\mu I\,d\mu,\qquad
\frac{d\Phi}{d\tau}=2\pi\int_{-1}^{1}(I-B)\,d\mu=4\pi(J-B)=0.
$$

Thus $\boxed{\Phi\text{ is constant with height}}$: [local radiative equilibrium](../../../../local-radiative-equilibrium.md) expresses energy conservation through successive atmospheric layers.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
