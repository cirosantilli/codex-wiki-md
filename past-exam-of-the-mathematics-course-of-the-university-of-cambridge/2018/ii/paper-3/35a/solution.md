<h1 id="35a/solution">Solution</h1>

↑ **Parent:** [35A](../35a.md)

The asymptotic [scattering wavefunction](../../../../../scattering-wavefunction.md) is

$$
\boxed{\psi(\mathbf r)\sim e^{ikz}+f(\theta)\frac{e^{ikr}}r.}
$$

In each [partial wave](../../../../../partial-wave.md), the [Partial-wave S-matrix](../../../../../partial-wave-s-matrix.md) is the ratio of its outgoing coefficient to its incoming coefficient. With the conventions in the question,

$$
S_l=1+2if_l.
$$

For [elastic scattering](../../../../../elastic-scattering.md) by a real central potential, [unitarity](../../../../../unitary-operator.md) gives $|S_l|=1$, so $S_l=e^{2i\delta_l}$ for a real [scattering phase shift](../../../../../scattering-phase-shift.md) $\delta_l$. Hence

$$
\boxed{f_l=\frac{S_l-1}{2i}=e^{i\delta_l}\sin\delta_l.}
$$

Using the [Orthogonality of Legendre polynomials](../../../../../orthogonality-of-legendre-polynomials.md) in $\sigma_T=\int|f(\theta)|^2d\Omega$ yields the [partial-wave total scattering cross-section](../../../../../partial-wave-total-scattering-cross-section.md)

$$
\boxed{\sigma_T=\frac{4\pi}{k^2}\sum_{l=0}^\infty(2l+1)\sin^2\delta_l.}
$$

For the [S wave](../../../../../s-wave.md), write the reduced radial wavefunction as

$$
u_{<}(r)=A\sinh(\kappa r),
\qquad
u_{>}(r)=B\sin(kr+\delta_0),
\qquad
\kappa=\sqrt{\gamma^2-k^2},
$$

where regularity at $r=0$ selected the hyperbolic sine. Continuity of $u$ and $u'$ at $r=a$, equivalently [logarithmic-derivative matching](../../../../../logarithmic-derivative-matching.md), gives

$$
k\cot(ka+\delta_0)=\kappa\coth(\kappa a),
$$

or

$$
\boxed{\frac{\tan(ka+\delta_0)}{ka}
=\frac{\tanh(\sqrt{\gamma^2-k^2}\,a)}{\sqrt{\gamma^2-k^2}\,a}.}
$$

For $ka\ll1$, let the [scattering length](../../../../../scattering-length-from-a-partial-wave-s-matrix.md) be $a_s=-\lim_{k\to0}\tan\delta_0/k$. Expanding the matching relation gives

$$
a-a_s=\frac{\tanh(\gamma a)}\gamma,
\qquad
a_s=a-\frac{\tanh(\gamma a)}\gamma.
$$

Only the S wave contributes at leading order, so

$$
\boxed{\sigma_T^{(0)}\sim4\pi
\left(a-\frac{\tanh(\gamma a)}\gamma\right)^2.}
$$

In the [hard-sphere limit](../../../../../hard-sphere-limit.md) $\gamma a\to\infty$, penetration is suppressed, $a_s\to a$, and

$$
\boxed{\sigma_T^{(0)}\to4\pi a^2.}
$$

This is four times the geometric area $\pi a^2$, a wave effect associated with diffraction from an impenetrable sphere.

## ↑ Ancestors (10)

1. [35A](../35a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
