<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For azimuthally symmetric [Rutherford scattering](../../../../../rutherford-scattering.md), integrate over the [solid angle](../../../../../solid-angle.md), $d\Omega=2\pi\sin\theta\,d\theta$. Substituting $u=\sin(\theta/2)$ gives $\sin\theta\,d\theta=4u\,du$, so

$$
\begin{aligned}
\sigma&=\frac{2\pi K}{p^2}\int_{\theta_{\min}}^{\theta_{\max}}
\frac{\sin\theta}{\sin^4(\theta/2)}\,d\theta\\
&=\frac{4\pi K}{p^2}\left[\csc^2\frac{\theta_{\min}}2-\csc^2\frac{\theta_{\max}}2\right].
\end{aligned}
$$

The small lower cutoff dominates when $\theta_{\max}\gg\theta_{\min}$ and $\theta_{\min}\ll1$. Using $\sin(\theta_{\min}/2)\simeq\theta_{\min}/2$, the leading total [cross section](../../../../../cross-section-physics.md) is

$$
\boxed{\sigma\simeq\frac{16\pi K}{p^2\theta_{\min}^2}.}
$$

A nonzero cutoff is essential: the unscreened forward [cross section](../../../../../cross-section-physics.md) otherwise diverges.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the particle physics course of the University of Oxford](../../../../split.md)
6. [Particle physics course of the University of Oxford](../../../../../particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the physics course of the University of Oxford](../../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
