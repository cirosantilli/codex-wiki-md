<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [exponential ridge-draft model](../../../../../../exponential-ridge-draft-model.md) along the direction of motion relative to the seabed. During time $dt$, the stationary point samples track length $|V|dt$. Peaks deeper than the seabed have line density

$$
\mu_D=\int_{\max(D,h_0)}^\infty n(H)\,dH
=\mu\exp\left[-\frac{\max(D,h_0)-h_0}{h_m-h_0}\right].
$$

The candidate [seabed gouging by ice](../../../../../../seabed-gouging-by-ice.md) encounter rate is therefore

$$
\boxed{\nu_D=|V|\mu
\exp\left[-\frac{\max(D,h_0)-h_0}{h_m-h_0}\right].}
$$

For the usual case $D\ge h_0$, replace $\max(D,h_0)$ by $D$. For $D<h_0$, every counted ridge is deep enough and $\nu_D=|V|\mu$.

The units are inverse time. This is the number of potentially scouring keel passages per unit time, not sediment volume removed per unit time. The latter also requires keel width, sediment properties and an erosion law. The expression assumes the ridge statistics remain applicable during drift and grounding does not arrest or reshape the deep keels before they reach the point. If speed fluctuates, use mean relative speed under independence from ridge occurrence, not the magnitude of a vector-mean drift that might cancel reversing motion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
