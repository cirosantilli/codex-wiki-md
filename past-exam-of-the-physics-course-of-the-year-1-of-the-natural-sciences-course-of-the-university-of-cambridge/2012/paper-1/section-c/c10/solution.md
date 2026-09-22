<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

The bob experiences weight $Mg$ vertically downward and a rod [force](../../../../../force-split.md) towards the pivot. The tangential component of weight is $-Mg\sin\theta$, so

$$
ML\ddot\theta=-Mg\sin\theta\simeq-Mg\theta,\qquad
\boxed{\omega_0^2=g/L,\qquad T_0=2\pi\sqrt{L/g}.}
$$

The rod [force](../../../../../force-split.md) supplies the radial [acceleration](../../../../../acceleration.md) and contributes no tangential [torque](../../../../../torque.md) about the pivot.

<a id="section-c/c10/image-original-force-diagram-for-a-displaced-pendulum-with-radial-and-tangential-directions"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1-ia2012-pendulum-forces.png)

**[Figure 1](#section-c/c10/image-original-force-diagram-for-a-displaced-pendulum-with-radial-and-tangential-directions). Original force diagram for a displaced pendulum, with radial and tangential directions**.

To the same small-angle order, writing $\chi=\omega_0t+\phi$,

$$
U=MgL(1-\cos\theta)\simeq\frac12MgL\theta_0^2\cos^2\chi,\qquad
K=\frac12ML^2\dot\theta^2=\frac12MgL\theta_0^2\sin^2\chi.
$$

Thus **$K+U=MgL\theta_0^2/2$** is constant. Put $b=\dot\theta(0)$, a signed [angular velocity](../../../../../angular-velocity.md). Then

$$
\boxed{\theta_0=\sqrt{\alpha^2+b^2/\omega_0^2},\qquad
\phi=\operatorname{atan2}(-b/\omega_0,\alpha)\pmod{2\pi}.}
$$

If the printed [angular speed](../../../../../angular-speed.md) $\beta$ is intended as the signed rate, set $b=\beta$. If it means magnitude only, $b=\pm\beta$ gives two possible [phases](../../../../../phase-waves.md); the [amplitude](../../../../../wave-amplitude.md) is unique. At zero [amplitude](../../../../../wave-amplitude.md) the [phase](../../../../../phase-waves.md) is arbitrary.

For a [finite-radius spherical pendulum bob](../../../../../finite-radius-spherical-pendulum-bob.md), the PDF dimension $L$ runs from pivot to [centre of mass](../../../../../center-of-mass.md). The [parallel axis theorem](../../../../../parallel-axis-theorem.md) gives $I_P=ML^2+2Ma^2/5$. The restoring [torque](../../../../../torque.md) remains $-MgL\theta$, hence

$$
T=2\pi\sqrt{\frac{ML^2+2Ma^2/5}{MgL}}
=T_0\sqrt{1+\frac{2a^2}{5L^2}}
\simeq T_0\left(1+\frac{a^2}{5L^2}\right).
$$

With $a=[3M/(4\pi\rho)]^{1/3}=0.02605\,\mathrm m$,

$$
\boxed{100\frac{T-T_0}{T_0}=0.01357\%\simeq0.0136\%.}
$$

The finite bob increases the inertia without changing the gravitational lever arm.

## ↑ Ancestors (13)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
