<h1 id="33a/solution">Solution</h1>

↑ **Parent:** [33A](../33a.md)

Let $\varepsilon=\omega/B\ll1$. The exact frequency has expansion $\lambda=B-\omega\cos\alpha+O(\omega^2/B)$. The ratio $(B-\omega\cos\alpha)/\lambda=1+O(\varepsilon^2)$, while the coefficient of the orthogonal state is uniformly $O(\varepsilon)$. Hence the supplied solution reduces to

$$
\chi(t)=e^{-iBt/2}\,e^{-i\omega(1-\cos\alpha)t/2}\chi_+(t)+O(\varepsilon),
$$

with phase error $O(\omega^2t/B)$, which is $O(\varepsilon)$ over one cycle. This is the adiabatic approximation: the system remains in the instantaneous positive-energy eigenstate, with energy $E_+=\hbar B/2$.

Thus **the dynamic phase is $-Bt/2$ and the geometric phase is $-\omega t(1-\cos\alpha)/2$**, in the gauge for $\chi_+$ printed in the PDF. For one cycle $T=2\pi/\omega$, the [Berry phase](../../../../../berry-phase.md) is

$$
\boxed{\Gamma=-\pi(1-\cos\alpha)\pmod{2\pi},}
$$

minus half the [solid angle](../../../../../solid-angle.md) swept by the field direction.

To calculate the requested integral, use $|\psi(\alpha,\varphi)\rangle=(\cos(\alpha/2),e^{i\varphi}\sin(\alpha/2))^T$. It has $i\langle\psi|\partial_\varphi\psi\rangle=-\sin^2(\alpha/2)$; its radial and polar-angle connection components vanish in this gauge. Along the circle in parameter space, $\varphi$ runs from zero to $2\pi$, so $\Gamma=-\int_0^{2\pi}\sin^2(\alpha/2)d\varphi=-\pi(1-\cos\alpha)$, agreeing with the exact-solution limit.

## ↑ Ancestors (10)

1. [33A](../33a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
