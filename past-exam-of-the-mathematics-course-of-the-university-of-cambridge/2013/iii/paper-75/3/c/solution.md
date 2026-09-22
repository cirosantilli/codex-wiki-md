<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the new periodic potential, let $\kappa$ be the single-neighbour hopping rate and $\Delta\epsilon=\hbar\kappa$. It is determined by the barrier between adjacent minima; an unspecified periodic potential does not determine it from the preceding quartic potential's numerical action. The minimum spacing is now $a$.

A path with $r$ right hops and $s$ left hops has $r-s=n-m$. Summing the ordered-center weights and their direction choices gives

$$
\langle na|e^{-H\tau/\hbar}|ma\rangle\simeq\mathcal A_0e^{-\omega\tau/2}
\sum_{r,s\ge0}\frac{(\kappa\tau)^{r+s}}{r!s!}\delta_{r-s,n-m}.
$$

Insert the [Fourier representation of a Kronecker delta](../../../../../../fourier-representation-of-a-kronecker-delta.md). The two exponential series sum independently, yielding the [dilute-hopping lattice propagator](../../../../../../dilute-hopping-lattice-propagator.md)

$$
\boxed{\langle na|e^{-H\tau/\hbar}|ma\rangle\simeq\mathcal A_0e^{-\omega\tau/2}
\int_0^{2\pi}\frac{d\theta}{2\pi}e^{-i(n-m)\theta}
\exp\left(\frac{2\Delta\epsilon\tau}{\hbar}\cos\theta\right).}
$$

The two Fourier-sign choices are equivalent by $\theta\mapsto-\theta$. Equivalently the integral is the [modified Bessel function](../../../../../../modified-bessel-function.md) $I_{n-m}(2\kappa\tau)$.

The original PDF prints $e^{+\omega\tau/2}$ here. Its sign is inconsistent with both the previous double-well result and the requested positive on-site oscillator energy. The correct factor is **$e^{-\omega\tau/2}$**: a positive oscillator [ground-state energy](../../../../../../ground-state-energy.md) must decay under $e^{-H\tau/\hbar}$. The other factors and their derivation remain as displayed. The energy $\Delta\epsilon$ is the positive nearest-neighbour [quantum tunnelling](../../../../../../quantum-tunnelling.md) matrix-element magnitude, exponentially small relative to the local well scale in the semiclassical regime.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
