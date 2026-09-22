<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

Measure both vertical displacements upward from static equilibrium, so gravity cancels. The spring force changes by $k(x_1-x)$, while the damper is attached to a fixed surface and supplies $-b\dot x$. [Newton's second law](../../../../../newton-s-second-law.md) gives

$$
\boxed{m\ddot x+b\dot x+kx=kx_1.}
$$

For sinusoidal steady motion, substitution of $x=\operatorname{Re}(RAe^{i\omega t})$ gives the [spring-base displacement response with a grounded damper](../../../../../spring-base-displacement-response-with-a-grounded-damper.md)

$$
\boxed{R(\omega)=\frac{k}{k-m\omega^2+i b\omega}.}
$$

A decaying homogeneous transient must be added unless initial conditions already select steady state. At low frequency, $R\to1$ and the mass follows the slowly moving support; the first correction is $-ib\omega/k$. At high frequency, $R\sim-k/(m\omega^2)$: inertia suppresses motion and reverses its phase relative to the support. There is no $ib\omega$ in the numerator because the damper's other end does not move.

Minimize the squared denominator $D=(k-m\omega^2)^2+b^2\omega^2$. Its derivative is $2\omega[2m^2\omega^2-2mk+b^2]$, giving

$$
\boxed{\omega_{\rm res}^2=k/m-b^2/(2m^2),\qquad b^2<2mk.}
$$

Write $\omega_0=\sqrt{k/m}$ and $\zeta=b/(2m\omega_0)$. Then $|R|=[(1-r^2)^2+4\zeta^2r^2]^{-1/2}$ with $r=\omega/\omega_0$, and the finite-frequency peak is $1/[2\zeta\sqrt{1-\zeta^2}]$. Increasing light damping lowers and broadens the peak and shifts it left; the low-frequency limit remains1 and the high-frequency decay remains proportional to $\omega^{-2}$.

The [resonance versus oscillatory damping thresholds](../../../../../resonance-versus-oscillatory-damping-thresholds.md) differ. For $b^2\ge2mk$, the maximum is at zero frequency and the curve decreases monotonically. This threshold is $\zeta=1/\sqrt2$, distinct from the free-oscillation critical damping threshold $\zeta=1$.

<a id="section-b/b6/image-base-displacement-response"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-1-pa2010-base-response.png)

**[Figure 3](#section-b/b6/image-base-displacement-response). Base displacement response**. [Source](paper-1-pa2010-base-response.py). Three light-damping levels and one monotone response; dots mark the finite-frequency peaks.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
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
