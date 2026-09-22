<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

For pendulum length $\ell$, small angular displacement gives $x\simeq\ell\theta$ and horizontal restoring force $-mgx/\ell$. Thus $\omega_0^2=g/\ell$ and

$$
\boxed{\ddot x+\omega_0^2x=\frac{F_0}{m}\sin\omega t}.
$$

For $\omega\ne\omega_0$, the [complementary solution](../../../../../homogeneous-solution.md) and a sinusoidal [particular solution](../../../../../particular-solution.md) give

$$
x=A\cos\omega_0t+B\sin\omega_0t+
\frac{F_0\sin\omega t}{m(\omega_0^2-\omega^2)}.
$$

Initial rest at the origin fixes $A=0$ and $B=-F_0\omega/[m\omega_0(\omega_0^2-\omega^2)]$, giving

$$
\boxed{x=\frac{F_0}{m(\omega_0^2-\omega^2)}
\left(\sin\omega t-\frac{\omega}{\omega_0}\sin\omega_0t\right)}.
$$

At exact [resonance](../../../../../resonance.md) the corresponding limit is $x=F_0[\sin\omega_0t-\omega_0t\cos\omega_0t]/(2m\omega_0^2)$; unrestricted initial conditions add the [complementary solution](../../../../../homogeneous-solution.md).

For $\omega=2\omega_0$, set $\tau=\omega_0t$. Then $m\omega_0^2x/F_0=(2\sin\tau-\sin2\tau)/3$: the period is $2\pi$ in $\tau$, zeros are at integer multiples of $\pi$, and the first extrema are $(2\pi/3,\sqrt3/2)$ and $(4\pi/3,-\sqrt3/2)$. Both initial displacement and slope vanish.

Substitution of the damped complex ansatz gives $[m(\omega_0^2-\omega^2)+ib\omega]x_0=F_0$. Hence

$$
\boxed{R(\omega)=\frac1{m(\omega_0^2-\omega^2)+ib\omega}}.
$$

For the [near-resonant mechanical susceptibility](../../../../../near-resonant-mechanical-susceptibility.md), put $\gamma=b/(2m)\ll\omega_0$ and $\delta=\omega-\omega_0$, and neglect $\delta^2$ and $b\delta$ near [resonance](../../../../../resonance.md):

$$
\boxed{R(\omega_0)=-\frac{i}{b\omega_0},\qquad
R(\omega)\simeq\frac1{2m\omega_0(-\delta+i\gamma)}}.
$$

Thus $|R|^2\simeq[4m^2\omega_0^2(\delta^2+\gamma^2)]^{-1}$, with angular-frequency full width $2\gamma=b/m$. The displacement lags the force by $\pi/2$ at $\omega_0$.

<a id="section-b/b6/image-original-initial-rest-response-at-twice-the-natural-frequency-and-weak-damping-resonance"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-2-driven-response.png)

**[Figure 1](#section-b/b6/image-original-initial-rest-response-at-twice-the-natural-frequency-and-weak-damping-resonance). Original initial-rest response at twice the natural frequency and weak-damping resonance**.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
