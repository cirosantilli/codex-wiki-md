<h1 id="k/k4/solution">Solution</h1>

↑ **Parent:** [K4](../k4.md)

A material interface obeys $D(y-\eta(x,t))/Dt=0$. In each [fluid](../../../../fluid.md) this gives $\phi_{jy}=\eta_t+(U_j+\phi_{jx})\eta_x$ at $y=\eta$, where $U_1=U$ and $U_2=V$. Discarding products of [perturbations](../../../../perturbation.md) and evaluating at the undisturbed interface gives

$$
\boxed{\phi_{1y}=\eta_t+U\eta_x,\qquad\phi_{2y}=\eta_t+V\eta_x\quad(y=0).}
$$

For an inviscid [irrotational](../../../../irrotational-vector-field.md) [fluid](../../../../fluid.md), unsteady Bernoulli is $\Phi_t+\tfrac12|\nabla\Phi|^2+p/\rho+gy=C(t)$, with total potential $\Phi=U_jx+\phi_j$. Subtract the undisturbed relation and linearize at the moving interface. The [pressure](../../../../pressure-split.md) [perturbation](../../../../perturbation.md) there is $-\rho_j(\phi_{jt}+U_j\phi_{jx}+g\eta)$. With no [surface tension](../../../../surface-tension-split.md) the two pressures agree, giving

$$
\boxed{\rho_1(\phi_{1t}+U\phi_{1x}+g\eta)=\rho_2(\phi_{2t}+V\phi_{2x}+g\eta)\quad(y=0).}
$$

Use [complex amplitudes](../../../../complex-amplitude.md) and take real parts at the end. For $k>0$, solutions of [Laplace's equation](../../../../laplace-equation.md) decaying away from the interface have the form

$$
\eta=Ae^{i(kx-\omega t)},\quad
\phi_1=B_1e^{ky}e^{i(kx-\omega t)},\quad
\phi_2=B_2e^{-ky}e^{i(kx-\omega t)}.
$$

Put $\Omega_1=\omega-Uk$ and $\Omega_2=\omega-Vk$. The kinematic conditions imply $B_1=-i\Omega_1A/k$ and $B_2=i\Omega_2A/k$. Substituting into the [pressure](../../../../pressure-split.md) condition gives

$$
\rho_1\left(g-\frac{\Omega_1^2}k\right)A=\rho_2\left(g+\frac{\Omega_2^2}k\right)A.
$$

A nonzero [amplitude](../../../../wave-amplitude.md) therefore requires

$$
\boxed{\rho_1(\omega-Uk)^2+\rho_2(\omega-Vk)^2=(\rho_1-\rho_2)gk.}
$$

To determine [stability](../../../../stability-of-a-numerical-method.md), let $R=\rho_1+\rho_2$ and $\overline U=(\rho_1U+\rho_2V)/R$. Completing the square yields

$$
(\omega-\overline Uk)^2=\frac{(\rho_1-\rho_2)gk}{R}-\frac{\rho_1\rho_2(U-V)^2k^2}{R^2}.
$$

For $U\neq V$, the right-hand side is negative exactly when

$$
k>\frac{(\rho_1^2-\rho_2^2)g}{\rho_1\rho_2(U-V)^2}.
$$

Then the two frequencies have opposite nonzero imaginary parts. The [root](../../../../root-of-a-root-system.md) with positive imaginary part gives [exponential growth](../../../../exponential-growth.md) through $e^{-i\omega t}$. In terms of [wavelength](../../../../wavelength.md) $\lambda=2\pi/k$, the unstable range is

$$
\boxed{\lambda<\lambda_c=\frac{2\pi\rho_1\rho_2(U-V)^2}{(\rho_1^2-\rho_2^2)g}.}
$$

This is the short-wavelength [Kelvin-Helmholtz instability](../../../../kelvin-helmholtz-instability.md) for a density-stable interface without [surface tension](../../../../surface-tension-split.md). Equality is the neutral threshold; if $U=V$, the gravitational term is positive and this shear [instability](../../../../instability.md) is absent.

## ↑ Ancestors (12)

1. [K4](../k4.md)
2. [K](../../k.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
