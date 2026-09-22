<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [characteristic equation](../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) of the [damped harmonic oscillator](../../../damped-harmonic-oscillator.md) is $r^2+\gamma r+\omega_0^2=0$. In the underdamped case its [roots](../../../root-of-a-root-system.md) are $-\gamma/2\pm i\omega_d$, where $\omega_d=\sqrt{\omega_0^2-\gamma^2/4}$. Thus the exact real solution is $y=Ae^{-\gamma t/2}\cos(\omega_dt+\alpha)$. For $\gamma\ll\omega_0$, $\omega_d=\omega_0+O(\gamma^2/\omega_0)$, giving the requested leading approximation

$$
\boxed{y(t)\simeq y_0e^{-\gamma t/2}\cos(\omega_0t+\alpha).}
$$

For [mass](../../../mass.md) $m$ and [spring constant](../../../spring-constant.md) $m\omega_0^2$, the [mechanical energy](../../../mechanical-energy.md) is $E=\tfrac12m(\dot y^2+\omega_0^2y^2)$. Differentiating and using the [differential equation](../../../differential-equation-split.md) gives $\dot E=-m\gamma\dot y^2$. In particular, [energy decay of a viscously damped harmonic oscillator](../../../energy-decay-of-a-viscously-damped-harmonic-oscillator.md) is not an exact pointwise [exponential decay](../../../exponential-decay.md): $\dot E=0$ at a turning point. To leading order in $\gamma/\omega_0$, the [period average](../../../period-average.md) is

$$
\boxed{\overline E(t)\simeq\frac12m\omega_0^2y_0^2e^{-\gamma t},\qquad \overline P_{\mathrm{loss}}\simeq\gamma\overline E.}
$$

The [quality factor](../../../q-factor.md) is $Q=2\pi\overline E/(\text{energy lost in one cycle})$. Using the [period](../../../period-of-a-function.md) $T\simeq2\pi/\omega_0$ and the small fractional loss $\gamma T$ gives $\boxed{Q\simeq\omega_0/\gamma}$. Equivalently, the energy-decay definition $Q=\omega_0\overline E/\overline P_{\mathrm{loss}}$ yields the same leading result. Replacing $\omega_d$ by $\omega_0$ in the oscillatory phase is not uniform over arbitrarily long times; its phase error is $O(\gamma^2t/\omega_0)$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2018](../../2018-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
