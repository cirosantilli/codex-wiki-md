<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In [Feynman gauge](../../../../../feynman-gauge.md), the Lagrangian differs by a total divergence from

$$
\mathcal L=-\frac12\partial_\mu A_\nu\partial^\mu A^\nu.
$$

Its [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is $\Box A^\mu=0$. Directly from the original gauge-fixed Lagrangian, the canonical momenta are

$$
\pi^\mu=-F^{0\mu}-\eta^{0\mu}\partial_\nu A^\nu,
$$

equivalently $\pi^\mu=-\partial^0A^\mu$ after using the total-divergence form.

Using the mode expansions and oscillator commutator, the two nonzero cross terms combine to

$$
\begin{aligned}
[\widehat A_\mu(\mathbf x),\widehat\pi_\nu(\mathbf y)]
&=\frac{i}{2}\int\frac{d^3p}{(2\pi)^3}
\sum_\lambda\eta_{\lambda\lambda}
\epsilon_\mu^\lambda(\mathbf p)\epsilon_\nu^\lambda(\mathbf p)
\left[e^{i\mathbf p\cdot(\mathbf x-\mathbf y)}
+e^{-i\mathbf p\cdot(\mathbf x-\mathbf y)}\right]\\
&=i\eta_{\mu\nu}\delta^{(3)}(\mathbf x-\mathbf y),
\end{aligned}
$$

where polarization completeness was used. The other equal-time field commutators vanish.

Substitution into the Hamiltonian and [normal ordering](../../../../../normal-ordering.md) give

$$
:\widehat H:
=-\sum_{\lambda=0}^3\eta_{\lambda\lambda}
\int\frac{d^3p}{(2\pi)^3}|\mathbf p|\,
\widehat a_{\mathbf p}^{\lambda\dagger}\widehat a_{\mathbf p}^{\lambda}.
$$

Every oscillator excitation carries positive energy $|\mathbf p|$, but the covariant state space has an indefinite inner product: time-like excitations have negative norm, and time-like and longitudinal polarizations are unphysical. [Gupta-Bleuler quantization](../../../../../gupta-bleuler-formalism.md) imposes

$$
(\partial_\mu\widehat A^\mu)^{(+)}|\mathrm{phys}\rangle=0
$$

and quotients by null states. The physical state space contains only the two transverse photon polarizations with positive norm, as required by [gauge invariance](../../../../../gauge-invariance.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
