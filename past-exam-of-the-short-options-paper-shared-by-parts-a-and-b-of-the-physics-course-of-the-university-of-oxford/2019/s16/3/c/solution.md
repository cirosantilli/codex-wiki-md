<h1 id="s16/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Introduce the electron momentum-relaxation rate $\nu$ through $m_e(\dot{\mathbf v}+\nu\mathbf v)=-e\mathbf E$. For a harmonic field $\mathbf E=\operatorname{Re}(\mathbf E_0e^{-i\omega t})$, the real part of the [electrical conductivity](../../../../../electrical-conductivity.md) is $\operatorname{Re}\sigma=n_ee^2\nu/[m_e(\omega^2+\nu^2)]$. At weak damping, the mean heating is $Q=\tfrac12\operatorname{Re}\sigma|E_0|^2$ and the beam [intensity](../../../../../intensity-physics.md) is $I=\tfrac12\epsilon_0cn|E_0|^2$, where $n=\sqrt{1-\omega_p^2/\omega^2}$. Therefore

$$
\frac{dI}{dx}=-\kappa I,\qquad
\kappa\simeq\frac{\nu}{c}\frac{\omega_p^2/\omega^2}{\sqrt{1-\omega_p^2/\omega^2}}.
$$

With the relaxation convention $\nu=1/(2\tau_{ei})$, this becomes the printed result

$$
\boxed{I(x)=I(0)e^{-\kappa x},\qquad\kappa=\frac{1}{2c\tau_{ei}}\frac{\omega_p^2}{\omega^2}\left(1-\frac{\omega_p^2}{\omega^2}\right)^{-1/2}.}
$$

**Convention qualification:** a $90^\circ$ deflection time does not by itself specify a momentum-relaxation rate without a collision model. If instead $\tau_{ei}$ is defined by $\nu=1/\tau_{ei}$, the intensity [absorption coefficient](../../../../../absorption-coefficient.md) is twice the printed one. Amplitude and intensity damping also differ by two. The result above states the extra convention needed rather than silently identifying these quantities. It assumes $\omega>\omega_p$, $\nu\ll\omega$ and sufficiently weak damping away from the cutoff; the apparent divergence near cutoff is outside that approximation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [S16](../../../s16.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
