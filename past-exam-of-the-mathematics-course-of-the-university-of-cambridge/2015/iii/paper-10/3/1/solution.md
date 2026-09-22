<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The sign convention makes this a [defocusing semilinear wave equation](../../../../../../defocusing-semilinear-wave-equation.md):

$$
\phi_{tt}-\Delta\phi+\phi^3=0.
$$

Its [wave energy](../../../../../../wave-energy.md) includes a nonnegative potential term:

$$
\boxed{E(t)=\int_{\mathbb R^3}\left(\frac12\phi_t^2+\frac12|\nabla\phi|^2+\frac14\phi^4\right)\,dx=E(0).}
$$

For a [smooth function](../../../../../../smooth-function.md) solution, [finite propagation speed](../../../../../../finite-propagation-speed.md) preserves [compact support](../../../../../../compact-support.md) on finite time intervals. Differentiate under the integral and use [integration by parts](../../../../../../integration-by-parts.md):

$$
\frac{dE}{dt}=\int_{\mathbb R^3}\phi_t\bigl(\phi_{tt}-\Delta\phi+\phi^3\bigr)\,dx=0.
$$

Equivalently the local [conservation law](../../../../../../conservation-law.md) has density $e=\phi_t^2/2+|\nabla\phi|^2/2+\phi^4/4$ and flux $-\phi_t\nabla\phi$. All three terms are nonnegative, and $E=0$ forces both [Cauchy data](../../../../../../cauchy-data.md) to vanish. Hence this is a positive conserved [energy](../../../../../../energy.md), rather than the indefinite energy associated with the opposite sign.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
