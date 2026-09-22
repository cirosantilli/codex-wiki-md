<h1 id="section-b/b6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [gyrocompass oscillation](../../../../../../gyrocompass-oscillation.md), use the same local basis and define $\theta$ about the stable orientation, with spin [angular momentum](../../../../../../angular-momentum.md) directed north at $\theta=0$. Because the vertical is perpendicular to the horizontal axle, the extra vertical [angular momentum](../../../../../../angular-momentum.md) from the slow azimuthal motion is $I_2\dot\theta$. To leading order in [Earth](../../../../../../earth.md)'s small [angular velocity](../../../../../../angular-velocity.md),

$$
\mathbf J\simeq J_s\mathbf u+I_2\dot\theta\,\mathbf z,\qquad J_s=I_1\omega.
$$

A constant vertical contribution $I_2\Omega_E\sin\lambda$ from [Earth's rotation](../../../../../../earth-s-rotation.md) has zero terrestrial time [derivative](../../../../../../derivative.md); the transverse terrestrial contributions affect the following equation only at order $\Omega_E^2$. Taking the vertical component of the [torque](../../../../../../torque.md) equation gives

$$
0=I_2\ddot\theta+J_s\Omega_E\cos\lambda\sin\theta.
$$

The terrestrial [derivative](../../../../../../derivative.md) of $J_s\mathbf u$ is horizontal, as is $\boldsymbol\Omega_E\times(I_2\dot\theta\mathbf z)$, so neither contributes to this component. Thus the small [angle](../../../../../../angle.md) satisfies, using the [small-angle approximation](../../../../../../small-angle-approximation.md) $\sin\theta\simeq\theta$,

$$
\ddot\theta+\frac{I_1}{I_2}\omega\Omega_E\cos\lambda\,\theta\simeq0,
\qquad
\boxed{\omega_{\rm shm}^2\simeq\frac{I_1}{I_2}\omega\Omega_E\cos\lambda.}
$$

This is [simple harmonic motion](../../../../../../simple-harmonic-motion.md), $\theta=A\cos(\omega_{\rm shm}t+\phi)$, with positive squared [angular frequency](../../../../../../angular-frequency.md) away from the poles. The approximation requires rapid spin, small angular displacement and negligible bearing [friction](../../../../../../friction.md). Near the opposite orientation, putting $\theta=\pi+\delta$ instead yields $\ddot\delta-\omega_{\rm shm}^2\delta\simeq0$, which is unstable. Consequently, the paper's oscillation claim applies to the stable [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md), not both north--south spin directions. Without [damping](../../../../../../damping.md) the ideal [gyrocompass](../../../../../../gyrocompass.md) continues to oscillate rather than settling.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
