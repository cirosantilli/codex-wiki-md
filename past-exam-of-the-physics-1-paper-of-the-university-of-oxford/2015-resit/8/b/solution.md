<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The air fall lasts

$$
t_a=\sqrt{\frac{2H_a}{g}}\simeq1.0096\,\mathrm s.
$$

Retain the underwater deceleration rather than replacing the whole water trajectory with motion at [terminal velocity](../../../../terminal-velocity.md). Define

$$
\chi=\operatorname{arctanh}\frac{v_t}{u}>0,\qquad \nu=bv_t.
$$

Separation of the descent equation gives the [hyperbolic cotangent](../../../../hyperbolic-cotangent.md) solution and its integrated depth:

$$
v(t)=v_t\coth(\chi+\nu t),\qquad
z(t)=\frac1b\ln\frac{\sinh(\chi+\nu t)}{\sinh\chi},
$$

where $t=0$ now means water entry. The derivative of the logarithm verifies $\dot z=v$, while $v(0)=v_t\coth\chi=u$. At water depth $H_w=5\,\mathrm m$, inversion using the [inverse hyperbolic sine](../../../../inverse-hyperbolic-sine.md) yields

$$
\boxed{t_w=\frac{\operatorname{arsinh}(e^{bH_w}\sinh\chi)-\chi}{bv_t}\simeq4.4264\,\mathrm s.}
$$

The total elapsed [time](../../../../time-in-physics.md) is therefore

$$
\boxed{t_{\mathrm{total}}=t_a+t_w\simeq5.44\,\mathrm s.}
$$

For an estimate without evaluating the exact expression, $bH_w\gg1$ permits $\operatorname{arsinh}x\simeq\ln(2x)$ here, giving

$$
t_w\simeq\frac{H_w}{v_t}+\frac{\ln(2\sinh\chi)-\chi}{bv_t}.
$$

This gives the same $4.43\,\mathrm s$ to the quoted precision. The simpler $H_w/v_t\simeq4.72\,\mathrm s$ overestimates the underwater [time](../../../../time-in-physics.md) because the pebble initially moves faster than $v_t$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
