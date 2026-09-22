<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [work of a spatially gated myosin head](../../../../work-of-a-spatially-gated-myosin-head.md), the mechanical [force](../../../../force-split.md) exerted by an attached head in the increasing-$x$ direction is $f(x)=-dU/dx=\kappa(x_0-x)$. It assists motion before $x_0$ and resists it afterwards. For one site encounter the expected work is

$$
W=\int_0^\infty P(x)\kappa(x_0-x)\,dx.
$$

In the narrow binding-window limit, retain the capture [probability](../../../../probability.md) $p_b=1-e^{-k_{on}\Delta x/v}$ but neglect the attachment [displacement](../../../../displacement.md) compared with $x_0$. The positive work is $p_b\kappa x_0^2/2$. After $x_0$, use $s=x-x_0$ to obtain the negative contribution $-p_b\kappa\int_0^\infty se^{-k_{off}s/v}ds=-p_b\kappa(v/k_{off})^2$. Hence

$$
\boxed{W\simeq\kappa(1-e^{-k_{on}\Delta x/v})
\left[\frac{x_0^2}{2}-\left(\frac v{k_{off}}\right)^2\right].}
$$

An independent [energy](../../../../energy-split.md) calculation gives the same factor: binding near zero loads [energy](../../../../energy-split.md) $\kappa x_0^2/2$, while an [exponentially distributed](../../../../exponential-distribution.md) post-threshold attachment time has $\langle t^2\rangle=2/k_{off}^2$, leaving mean [elastic energy](../../../../elastic-energy.md) $\kappa v^2/k_{off}^2$ to be lost upon detachment. The factor of two in that [second moment](../../../../second-moment.md) is essential.

One site passes every distance $D$, so average work per distance, or power divided by $v$, gives

$$
\boxed{\overline F(v)=\frac{W}{D}\simeq
\frac\kappa D(1-e^{-k_{on}\Delta x/v})
\left[\frac{x_0^2}{2}-\frac{v^2}{k_{off}^2}\right].}
$$

The [force](../../../../force-split.md) tends to $\kappa x_0^2/(2D)$ as $v\downarrow0$ and changes sign at $v=k_{off}x_0/\sqrt2$ in this idealized model. Above that speed forced [sliding](../../../../facilitated-target-search.md) is resisted on average. The formula uses the reset condition in [b](../b.md), as well as $\Delta x\ll x_0$; if reset fails, replace $p_b$ by the periodic capture [probability](../../../../probability.md) to leading order in $\Delta x/x_0$. For arbitrary window width, the isolated-site work is exactly $\int_0^{\Delta x}(k_{on}/v)e^{-k_{on}x/v}[\kappa(x_0-x)^2/2-\kappa v^2/k_{off}^2]dx$. The loaded [spring](../../../../spring.md) [energy](../../../../energy-split.md) must be supplied by the binding/power-stroke chemistry; this model does not specify an [ATP](../../../../adenosine-triphosphate.md) efficiency. Real force-dependent transition rates and [energy](../../../../energy-split.md) budgets limit extrapolation of the toy [force-velocity](../../../../work-of-a-spatially-gated-myosin-head.md) law.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
