<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interchange the input and feedback components: put the [capacitor](../../../../capacitor.md) $C$ between the input and the inverting terminal, and the [resistor](../../../../resistor.md) $R$ between the output and the inverting terminal. Keep the non-inverting terminal grounded, as in the lower circuit above. For an [ideal operational amplifier](../../../../ideal-operational-amplifier.md) under unsaturated [negative feedback](../../../../negative-feedback.md), the inverting node remains at [virtual ground](../../../../virtual-ground.md).

The input [capacitor current](../../../../capacitor-current.md) is $I_C=C\,dV_{\rm in}/dt$. It flows through the feedback [resistor](../../../../resistor.md), giving

$$
C\frac{dV_{\rm in}}{dt}=\frac{0-V_{\rm out}}R,\qquad\boxed{V_{\rm out}=-RC\frac{dV_{\rm in}}{dt}}.
$$

This is an inverting [op amp differentiator](../../../../op-amp-differentiator.md). Its ideal gain magnitude increases with [frequency](../../../../frequency.md), so it strongly amplifies high-frequency noise. Practical differentiators include components that restrict the useful band and stabilize feedback; that qualification does not change the displayed ideal low-amplitude relation within the operating band.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
