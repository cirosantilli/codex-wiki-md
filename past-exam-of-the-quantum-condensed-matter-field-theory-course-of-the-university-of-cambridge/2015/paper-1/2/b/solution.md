<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For one coordinate with [Hamiltonian](../../../../../hamiltonian.md) $H=\hat p^2/(2m)+V(\hat x)$, the propagator is $K(x_f,t_f;x_i,t_i)=\langle x_f|e^{-iHT/\hbar}|x_i\rangle$, where $T=t_f-t_i>0$. Divide $T$ into $M$ intervals $\delta t$, use the [Trotter product formula](../../../../../lie-product-formula.md) to separate kinetic and potential evolution, and insert complete [position](../../../../../position.md) and [momentum](../../../../../momentum-split.md) bases at each slice. The [momentum](../../../../../momentum-split.md) integral is Gaussian:

$$
\langle x_{j+1}|e^{-i\delta t\hat p^2/(2m\hbar)}|x_j\rangle
=\int\frac{dp_j}{2\pi\hbar}\exp\left[\frac i\hbar p_j(x_{j+1}-x_j)-\frac{i\delta t}{2m\hbar}p_j^2\right]
=\left(\frac m{2\pi i\hbar\delta t}\right)^{1/2}
 e^{im(x_{j+1}-x_j)^2/(2\hbar\delta t)}.
$$

Multiplying the short-time kernels gives the [time-sliced configuration-space path integral](../../../../../time-sliced-configuration-space-path-integral.md),

$$
K=\lim_{M\to\infty}\left(\frac m{2\pi i\hbar\delta t}\right)^{M/2}
\int\prod_{j=1}^{M-1}dx_j\,
\exp\left\{\frac i\hbar\sum_{j=0}^{M-1}
\left[\frac{m(x_{j+1}-x_j)^2}{2\delta t}-\delta t V(x_j)\right]\right\},
$$

with $x_0=x_i$, $x_M=x_f$. Continuum notation abbreviates this limit as $\int_{x_i}^{x_f}\mathcal D x\,e^{iS[x]/\hbar}$, where $S=\int dt\,[m\dot x^2/2-V(x)]$. The measure includes the displayed normalization; it is not an unweighted count of paths. A small damping or analytic-continuation prescription defines the oscillatory integrals. The paths contribute complex amplitudes, so alternative histories interfere before [probabilities](../../../../../probability.md) are calculated. This is the central difference from a classical statistical mixture of trajectories.[pp.367–374, action phases and construction of the propagator](../../../../../space-time-approach-to-non-relativistic-quantum-mechanics-by-richard-feynman.md)

When [actions](../../../../../action.md) vary rapidly relative to $\hbar$, [stationary phase](../../../../../stationary-phase-method.md) selects [classical paths](../../../../../classical-path.md). Put $x=x_{\rm cl}+\eta$, with $\eta$ zero at the endpoints. Vanishing first variation gives $m\ddot x_{\rm cl}+V'(x_{\rm cl})=0$. The quadratic term is

$$
S[x]=S[x_{\rm cl}]+\frac12\int dt\,
\eta\left(-m\frac{d^2}{dt^2}-V''(x_{\rm cl})\right)\eta+O(\eta^3).
$$

The resulting Gaussian fluctuation [determinant](../../../../../determinant.md) is the [semiclassical propagator](../../../../../semiclassical-propagator.md) prefactor. In one dimension, away from caustics,

$$
\boxed{K_{\rm sc}=\sum_{\rm cl}
\left(\frac{D_{\rm cl}}{2\pi i\hbar}\right)^{1/2}
\exp\left[\frac{iS_{\rm cl}}\hbar-\frac{i\pi\nu_{\rm cl}}2\right],\qquad
D_{\rm cl}=\left|-\frac{\partial^2S_{\rm cl}}{\partial x_f\partial x_i}\right|.}
$$

The branch convention makes $\nu=0$ for a direct free-particle path before any caustic. The [Maslov index](../../../../../maslov-index.md) tracks the phase changes as fluctuations pass through a focal singularity. In several dimensions replace the endpoint [derivative](../../../../../derivative.md) by the [Van Vleck determinant](../../../../../van-vleck-determinant.md). The approximation sums all relevant [classical paths](../../../../../classical-path.md); real-time [action](../../../../../action.md) need only be stationary, not a minimum. It fails in this simple form at a caustic or coalescing saddles, where a uniform approximation is needed. Quadratic [actions](../../../../../action.md) have no higher fluctuation terms, making their Gaussian evaluation exact. For example $S_{\rm cl}=m(x_f-x_i)^2/(2T)$ gives the exact free-particle kernel $\sqrt{m/(2\pi i\hbar T)}e^{iS_{\rm cl}/\hbar}$. Tunnelling involves classically forbidden regions and can be described by imaginary-time saddles rather than real classical trajectories.

Quantum [statistical mechanics](../../../../../statistical-mechanics.md) follows by [Wick rotation](../../../../../wick-rotation.md) $t=-i\tau$. The imaginary-time evolution operator is $e^{-\tau H/\hbar}$, with [Euclidean action](../../../../../euclidean-action.md)

$$
S_E[x]=\int_0^{\beta\hbar}d\tau\left[\frac m2(\partial_\tau x)^2+V(x)\right].
$$

Taking a [thermal trace](../../../../../thermal-trace.md) identifies and integrates the endpoint [positions](../../../../../position.md):

$$
\boxed{Z=\operatorname{Tr}e^{-\beta H}
=\int dx\int_{x(0)=x}^{x(\beta\hbar)=x}\mathcal D x\,e^{-S_E[x]/\hbar}.}
$$

This [thermal trace as a closed Euclidean path integral](../../../../../thermal-trace-as-a-closed-euclidean-path-integral.md) explains the periodic imaginary-time direction. A density-matrix element instead retains open endpoints. For many identical particles the [trace](../../../../../matrix-trace.md) also sums over endpoint permutations, with a plus sign for [bosons](../../../../../boson.md) and permutation parity for [fermions](../../../../../fermion.md). In coherent-state language this becomes periodic bosonic fields and antiperiodic [Grassmann fields](../../../../../grassmann-field.md), with corresponding [Matsubara frequencies](../../../../../matsubara-frequency.md).

The Euclidean weight resembles a classical [Boltzmann weight](../../../../../boltzmann-factor.md). A time-sliced local [quantum field](../../../../../quantum-field.md) in $d$ spatial dimensions becomes a classical-looking field model in $d+1$ dimensions, with anisotropic couplings and extra extent $\beta\hbar$. Thus zero-temperature quantum criticality can be treated using an infinitely extended imaginary-time direction, while nonzero [temperature](../../../../../temperature-split.md) imposes a finite thickness. The dynamical scaling of [time](../../../../../time-in-physics.md) need not equal the spatial scaling: the [dynamical critical exponent](../../../../../dynamical-critical-exponent.md) specifies their relationship. This [quantum-to-classical imaginary-time mapping](../../../../../quantum-to-classical-imaginary-time-mapping.md) requires qualification when weights have signs or imaginary terms; such a [functional integral](../../../../../functional-measure.md) is not automatically an ordinary positive classical [probability](../../../../../probability.md) [distribution](../../../../../distribution-mathematical-analysis.md). Even with a positive weight, the mapping concerns equilibrium statistics, not literal dissipative real-time trajectories. For a free particle the Euclidean kernel is a [diffusion](../../../../../diffusion.md) kernel with [diffusion](../../../../../diffusion.md) coefficient $\hbar/(2m)$, illustrating the mathematical correspondence.

The classical high-temperature limit is a further approximation, rather than simply another name for imaginary [time](../../../../../time-in-physics.md). If quantum level spacings and exchange effects are negligible, a one-particle [partition function](../../../../../canonical-partition-function.md) in $d$ dimensions becomes

$$
Z_{\rm cl}\simeq\int\frac{d^dx\,d^dp}{(2\pi\hbar)^d}
 e^{-\beta[p^2/(2m)+V(x)]}.
$$

For [indistinguishable particles](../../../../../indistinguishable-particles.md) there is a factor $1/N!$ in the dilute classical gas, and exchange is negligible when the [number density](../../../../../number-density.md) [times](../../../../../time-in-physics.md) the [thermal de Broglie wavelength](../../../../../thermal-de-broglie-wavelength.md) to power $d$ is small. For a [harmonic oscillator](../../../../../simple-harmonic-motion.md), the exact quantum result $Z=[2\sinh(\beta\hbar\omega/2)]^{-1}$ tends to $1/(\beta\hbar\omega)$ as $\beta\hbar\omega\to0$, recovering the classical phase-space integral. **[stationary phase](../../../../../stationary-phase-method.md) explains [classical mechanics](../../../../../classical-mechanics-split.md); the short imaginary-time, weak-exchange limit explains classical [statistical mechanics](../../../../../statistical-mechanics.md).** These are related but distinct limits of the same quantum formulation.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
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
