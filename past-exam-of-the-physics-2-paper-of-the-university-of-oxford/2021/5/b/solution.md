<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $V_{\rm in}=v(t)+V_{\rm off}$, with constant unwanted offset $V_{\rm off}$. Add an adjustable reference [voltage](../../../../voltage.md) $V_b$ through another [resistor](../../../../resistor.md) $R_b$ to the **first** inverting summing junction, as the dashed branch in the circuit figure shows. [Kirchhoff's current law](../../../../kirchhoff-node-law.md) now gives

$$
V_1=-R_f\left(\frac{V_{\rm in}}{R_a}+\frac{V_b}{R_b}\right).
$$

Choose the reference polarity and magnitude so that

$$
\boxed{\frac{V_b}{R_b}=-\frac{V_{\rm off}}{R_a}.}
$$

A potentiometer between positive and negative reference supplies permits either sign. The first stage then has zero output [voltage](../../../../voltage.md) when $v=0$, and the [op amp integrator](../../../../op-amp-integrator.md) integrates only $v(t)$:

$$
\boxed{V_{\rm out}(t)=V_{\rm out}(t_0)+\frac{R_f}{R_aR_iC_i}\int_{t_0}^t v(t')\,dt'.}
$$

Merely placing a large [resistor](../../../../resistor.md) across the integrating [capacitor](../../../../capacitor.md) limits drift but also changes the [transfer function](../../../../transfer-function.md); cancellation at the summing junction preserves ideal integration of the desired signal.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
