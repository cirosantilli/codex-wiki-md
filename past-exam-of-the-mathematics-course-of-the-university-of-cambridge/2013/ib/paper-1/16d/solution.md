<h1 id="16d/solution">Solution</h1>

↑ **Parent:** [16D](../16d.md)

The [Drude model](../../../../../drude-model.md) treats carriers as classical independent particles, accelerated between collisions by the electric force. Collisions occur at constant rate $\tau^{-1}$ and randomize the directed velocity to zero mean; the ions are an effectively stationary background. Over a short time $dt$, directed velocity gains $(e/m)\mathbf E\,dt$ while the fraction $dt/\tau$ that collides loses its mean directed motion. Therefore

$$
\frac{d\langle\mathbf v\rangle}{dt}=-\frac{\langle\mathbf v\rangle}{\tau}+\frac em\mathbf E.
$$

Here $e$ is the signed carrier charge. For the stated complex harmonic convention,

$$
\mathbf v_0=\frac{e\tau/m}{1-i\omega\tau}\mathbf E_0,
\qquad
\boxed{\mathbf J=ne\langle\mathbf v\rangle=\sigma\mathbf E,\quad
\sigma=\frac{ne^2\tau/m}{1-i\omega\tau}.}
$$

The conductivity is positive in its dissipative real part regardless of the sign of $e$.

For zero charge density, Gauss's law makes the electric amplitude transverse. Faraday's and Ampère-Maxwell's laws, with displacement current retained, give

$$
\nabla\times\nabla\times\mathbf E
=-\mu_0\sigma\partial_t\mathbf E-\mu_0\epsilon_0\partial_t^2\mathbf E.
$$

Substitution of $e^{i\mathbf k\cdot\mathbf x-i\omega t}$ yields

$$
\boxed{k^2=\frac{\omega^2}{c^2}\epsilon_r,\qquad
\epsilon_r=1+\frac{i\sigma}{\omega\epsilon_0}
=1-\frac{\omega_p^2}{\omega(\omega+i/\tau)}.}
$$

For propagation in a fixed direction, $k$ is the possibly complex scalar wave number; equivalently the spatial equation uses $\mathbf k\cdot\mathbf k$, without complex conjugation. The printed real-vector notation $|\mathbf k|$ must be analytically continued in an absorbing or evanescent medium.

In the [high-frequency Drude plasma cutoff](../../../../../high-frequency-drude-plasma-cutoff.md) regime, $\omega\tau\gg1$ gives $\epsilon_r\simeq1-\omega_p^2/\omega^2$. Below the plasma frequency, the physical decaying branch is

$$
\boxed{k\simeq i\sqrt{\omega_p^2-\omega^2}/c,\qquad
\mathbf E\propto e^{-x\sqrt{\omega_p^2-\omega^2}/c}.}
$$

Finite collisions add a small phase component while maintaining positive attenuation. Very near the threshold one should retain the full complex permittivity rather than the purely imaginary approximation.

## ↑ Ancestors (10)

1. [16D](../16d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
