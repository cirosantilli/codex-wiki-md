<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $H=\hat p^2/(2m)+V(\hat x)$, divide elapsed time $t$ into $J$ slices $\Delta t=t/J$ and apply the [Trotter product formula](../../../../../lie-product-formula.md). Inserting complete position and momentum bases gives the regulated [phase-space path integral](../../../../../phase-space-path-integral.md)

$$
K(x_f,x_i;t)=\lim_{J\to\infty}\int\prod_{j=1}^{J-1}dx_j\prod_{j=0}^{J-1}\frac{dp_j}{2\pi\hbar}\exp\left\{\frac i\hbar\sum_{j=0}^{J-1}\left[p_j(x_{j+1}-x_j)-\Delta t\left(\frac{p_j^2}{2m}+V(x_j)\right)\right]\right\}.
$$

The endpoint values are $x_0=x_i$, $x_J=x_f$. Each [Gaussian momentum integration in a phase-space path integral](../../../../../gaussian-momentum-integration-in-a-phase-space-path-integral.md) can be performed explicitly, leaving the [configuration-space path integral](../../../../../configuration-space-path-integral.md)

$$
\boxed{K=\int_{x_i}^{x_f}\mathcal Dx\,e^{iS[x]/\hbar},\qquad S[x]=\int_0^t ds\,[m\dot x^2/2-V(x)].}
$$

Its measure is the time-sliced limit of $(m/(2\pi i\hbar\Delta t))^{J/2}\prod_{j=1}^{J-1}dx_j$, with the usual infinitesimal convergence prescription. The integral sums amplitudes, not positive classical probabilities. Operator ordering remains part of the time-slice definition. Expanding a short-time kernel recovers the [Schrödinger equation](../../../../../schrodinger-equation.md); composing kernels reproduces the [time-evolution operator](../../../../../time-evolution-operator.md).

In the [classical limit](../../../../../classical-limit.md), rapid phase cancellation suppresses paths away from stationary [action](../../../../../action.md). Varying $S$ with fixed endpoints gives $m\ddot x=-V'(x)$. The semiclassical result sums the classical-path phases multiplied by fluctuation [functional determinants](../../../../../functional-determinant.md); for a quadratic [Hamiltonian](../../../../../hamiltonian.md) the fluctuation integral is Gaussian and this expansion is exact.

For [quantum statistical mechanics](../../../../../quantum-statistical-mechanics.md), continue $t=-i\tau$ by a [Wick rotation](../../../../../wick-rotation.md). The [Euclidean action](../../../../../euclidean-action.md) and thermal [trace](../../../../../matrix-trace.md) give

$$
S_E=\int_0^{\beta\hbar}d\tau\,[m(\partial_\tau x)^2/2+V(x)],\qquad
\boxed{Z=\operatorname{Tr}e^{-\beta H}=\int_{x(\beta\hbar)=x(0)}\mathcal Dx\,e^{-S_E/\hbar}.}
$$

The trace closes position-space paths. In a many-particle trace one also sums over endpoint permutations with the appropriate exchange signs. In a [coherent state](../../../../../coherent-state.md) field formulation, bosonic fields are periodic and [fermionic coherent states](../../../../../fermionic-coherent-state.md) instead give antiperiodic [Grassmann fields](../../../../../grassmann-field.md), hence bosonic and fermionic [Matsubara frequencies](../../../../../matsubara-frequency.md) $2\pi n/(\beta\hbar)$ and $(2n+1)\pi/(\beta\hbar)$. [§§3.1–3.2, coherent-state time slicing and trace boundary conditions](../../../../../physics-215c-quantum-field-theory-part-3-by-john-mcgreevy.md)

The [quantum-to-classical imaginary-time mapping](../../../../../quantum-to-classical-imaginary-time-mapping.md) views a local $d$-dimensional quantum problem as a classical-looking field theory in $d+1$ dimensions, with imaginary-time extent $\beta\hbar$. A genuine classical probability interpretation additionally requires a nonnegative weight; fermion signs and Berry terms can obstruct it.

For a smooth potential in the high-temperature or small-$\hbar$ limit, imaginary-time paths fluctuate only over the [thermal de Broglie wavelength](../../../../../thermal-de-broglie-wavelength.md) $\lambda_T=\sqrt{2\pi\beta\hbar^2/m}$. If this is short compared with the potential's variation scale, the diagonal free kernel gives

$$
\boxed{Z\simeq\frac1{2\pi\hbar}\int dx\,dp\,e^{-\beta[p^2/(2m)+V(x)]}=\frac1{\lambda_T}\int dx\,e^{-\beta V(x)}.}
$$

This [classical phase-space limit of the thermal kernel](../../../../../classical-phase-space-limit-of-the-thermal-kernel.md) is the classical [phase space](../../../../../phase-space.md) partition function for one degree of freedom. A dilute identical-particle gas also needs its $1/N!$ factor; when exchange is appreciable, classical statistics fails. As a check, a single [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator-split.md) gives $Z=[2\sinh(\beta\hbar\omega/2)]^{-1}\to1/(\beta\hbar\omega)$, precisely the classical phase-space integral.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
