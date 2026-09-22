<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write the [Generalized Korteweg–De Vries equation](../../../../../../generalized-korteweg-de-vries-equation.md) as

$$
u_t=-\partial_x(u_{xx}+u^p).
$$

For a sufficiently regular solution, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\frac d{dt}\int_{\mathbb R}u^2\,dx
=-2\int_{\mathbb R}u\,\partial_x(u_{xx}+u^p)\,dx
=2\int_{\mathbb R}u_xu_{xx}\,dx
+2\int_{\mathbb R}u^pu_x\,dx=0.
$$

Thus [KdV mass conservation](../../../../../../kdv-mass-and-energy-conservation.md) gives

$$
\boxed{\|u(t)\|_2=\|u_0\|_2}
$$

is conserved.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
