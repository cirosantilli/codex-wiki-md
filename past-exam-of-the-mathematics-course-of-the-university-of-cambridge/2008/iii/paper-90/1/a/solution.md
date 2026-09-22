<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the [shallow-water approximation](../../../../../../shallow-water-approximation.md): the horizontal scale is long compared with the depth, the [hydrostatic approximation](../../../../../../hydrostatic-approximation.md) applies, and the cross-section-averaged [velocity](../../../../../../velocity.md) is approximately uniform. Neglect viscosity and drag for this part. [Volume conservation](../../../../../../volume-conservation.md) gives the constant discharge $Q=bhu$. The steady horizontal momentum equation is

$$
u u_x=-g(H+h)_x,
$$

so its integral is the [Bernoulli equation](../../../../../../bernoulli-equation.md) head $\mathcal H=H+h+u^2/(2g)$. The [shallow-water specific energy](../../../../../../shallow-water-specific-energy.md) measured above the bed is therefore

$$
\boxed{E(h;Q,b)=h+\frac{Q^2}{2gb^2h^2},\qquad E+H=\mathcal H.}
$$

The [Froude number](../../../../../../froude-number.md) compares the flow [velocity](../../../../../../velocity.md) with the long-wave speed $\sqrt{gh}$:

$$
\boxed{F=\frac{u}{\sqrt{gh}},\qquad E=h\left(1+\frac{F^2}{2}\right),\qquad
\left.\frac{\partial E}{\partial h}\right|_{Q,b}=1-F^2.}
$$

At fixed $Q,b$, the [shallow-water specific energy](../../../../../../shallow-water-specific-energy.md) tends to infinity as $h$ tends to zero or infinity. Its unique minimum occurs at the critical depth

$$
h_c=\left(\frac{Q^2}{gb^2}\right)^{1/3},\qquad F=1,\qquad E_c=\frac32h_c.
$$

The two depth branches above that minimum are [subcritical flow](../../../../../../subcritical-flow.md), $F<1$ with $h>h_c$, and [supercritical flow](../../../../../../supercritical-flow.md), $F>1$ with $h<h_c$. The long-wave [characteristic speeds](../../../../../../characteristic-speed.md) relative to the bed are $u\pm\sqrt{gh}$. Thus a [subcritical flow](../../../../../../subcritical-flow.md) can receive information from downstream, whereas both [characteristic curves](../../../../../../characteristic-curve.md) travel downstream in a positive [supercritical flow](../../../../../../supercritical-flow.md).

A [hydraulic control](../../../../../../hydraulic-control.md) is a critical section where one [characteristic speed](../../../../../../characteristic-speed.md) vanishes and a smooth flow can pass between the two branches. Regularity there supplies a condition relating $Q$, the depth and the geometry; together with reservoir or inlet data, it can determine the discharge. Merely finding $F=1$ is not enough: a finite depth gradient also requires the geometric forcing to vanish in the critical momentum equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
