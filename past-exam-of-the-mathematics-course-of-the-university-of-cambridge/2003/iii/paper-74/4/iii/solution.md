<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $a(t)=a_0+a_1(t)$ and use $s=|y|$ for the source radius, reserving $r$ for observation distance. Incompressible spherical [potential flow](../../../../../../potential-flow.md) satisfies $s^2u_s=a^2\dot a$. Its [velocity potential](../../../../../../velocity-potential.md), tending to zero at infinity, and [velocity](../../../../../../velocity.md) are

$$
\Phi(y,t)=-\frac{a^2\dot a}{s},\qquad
u_s=\frac{a^2\dot a}{s^2}.
$$

The unsteady [Bernoulli equation](../../../../../../bernoulli-equation.md) gives

$$
p(s,t)-p_\infty=\rho_0\left[\frac{\frac{d}{dt}(a^2\dot a)}s-\frac{a^4\dot a^2}{2s^4}\right],\qquad
p(a,t)-p_\infty=\rho_0\left(a\ddot a+\tfrac32\dot a^2\right).
$$

The surface [pressure](../../../../../../pressure.md) is independent of angle. Hence the integrated surface [force](../../../../../../force.md) is zero, $f=p(a,t)\int_S n\,dS=0$, and **the leading compact surface dipole contribution vanishes**. This also makes $\mathcal F=0$ in the notation of the preceding part.

The volume flux is $\mathcal V=4\pi a^2\dot a$, so the [acoustic thickness noise](../../../../../../acoustic-thickness-noise.md) contribution is

$$
\boxed{\rho'_M=\frac{\rho_0}{c_0^2r}(a^2\ddot a+2a\dot a^2)_{\tau}}
=\frac{\rho_0a_0^2}{c_0^2r}\ddot a_1(\tau)+O(a_1^2).
$$

The leading part is linear in the radial oscillation. Keeping the quadratic terms explicitly gives $\rho_0[a_0^2\ddot a_1+a_0\frac{d^2}{dt^2}(a_1^2)]/(c_0^2r)$.

For the [acoustic quadrupole](../../../../../../acoustic-quadrupole.md), use $T_{ij}\simeq\rho_0u_i u_j$. To leading quadratic order,

$$
u_i=a_0^2\dot a_1\frac{y_i}{s^3},\qquad
\int_{s\ge a_0}\frac{y_i y_j}{s^6}\,dV
=\int_{a_0}^\infty\frac{ds}{s^2}\int n_i n_j\,d\Omega
=\frac{4\pi}{3a_0}\delta_{ij}.
$$

Thus

$$
S_{ij}=\frac{4\pi}{3}\rho_0a_0^3\dot a_1^2\delta_{ij},\qquad
\boxed{\rho'_Q=\frac{\rho_0a_0^3}{3c_0^4r}\frac{d^2}{dt^2}\big(\dot a_1^2\big)_{\tau}}.
$$

Keeping the instantaneous lower limit $s=a(t)$ instead gives $S_{ij}=4\pi\rho_0a^3\dot a^2\delta_{ij}/3$, whose leading small-oscillation term is the expression just obtained. Although the stress moment is isotropic, its contracted second derivative is not zero: $n_i n_j\delta_{ij}=1$.

For a sinusoidal radius perturbation $a_1=A\cos\omega t$, the leading [compact radiation moments of a pulsating spherical bubble](../../../../../../compact-radiation-moments-of-a-pulsating-spherical-bubble.md) are

$$
\rho'_M=-\frac{\rho_0a_0^2A\omega^2}{c_0^2r}\cos\omega\tau+O(A^2),\qquad
\rho'_Q=\frac{2\rho_0a_0^3A^2\omega^4}{3c_0^4r}\cos2\omega\tau.
$$

Writing $\delta=A/a_0$ and $\alpha=\omega a_0/c_0$, the quadrupole [amplitude](../../../../../../wave-amplitude.md) relative to the linear monopole is $2\delta\alpha^2/3$. The monopole also has a quadratic correction, $-2\rho_0a_0A^2\omega^2\cos2\omega\tau/(c_0^2r)$; the volume-stress quadrupole is smaller than this quadratic monopole correction by $\alpha^2/3$.

**In the small-amplitude compact regime, the linear monopole dominates, the leading dipole is zero, and the volume quadrupole is weaker and begins at twice the oscillation [frequency](../../../../../../frequency.md).** The compact formulas require $\alpha\ll1$ as well as a far observer. The stated small surface [Mach number](../../../../../../mach-number.md) $|\dot a_1|/c_0\sim\delta\alpha\ll1$ alone does not imply compactness. The incompressible near field has a decaying tail, but its stress moment is dominated by distances of order $a_0$; an acoustic matching region is still needed outside it. These are leading compact contributions, not a claim to retain every finite-wavelength correction at the smaller quadrupole order.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
