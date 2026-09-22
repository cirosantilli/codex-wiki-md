<h1 id="14e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\operatorname{Im}z>0$, close the $t$-contour in the upper half-plane. [Jordan lemma](../../../../../../jordan-s-lemma.md) removes the large semicircle, and the only enclosed [pole](../../../../../../pole.md) is the order-$n$ pole at $t=z$. By the [residue at a pole of order n](../../../../../../residue-at-a-pole-of-order-n.md),

$$
\operatorname{Res}_{t=z}\frac{e^{it}}{(t-z)^n}
=\frac1{(n-1)!}
\left.\frac{d^{\,n-1}}{dt^{\,n-1}}e^{it}\right|_{t=z}
=\frac{i^{n-1}e^{iz}}{(n-1)!}.
$$

The [residue theorem](../../../../../../residue-theorem.md) therefore gives

$$
F(z)=\frac{2\pi i^ne^{iz}}{(n-1)!}.
$$

To continue the integral itself, move the $t$-contour downward locally as $z$ approaches and crosses the real axis, always keeping the pole above the contour. This [analytic continuation by contour deformation](../../../../../../analytic-continuation-by-contour-deformation.md) defines

$$
\widetilde F(z)
=\int_{\mathcal C_z}\frac{e^{it}}{(t-z)^n}\,dt,
$$

where $\mathcal C_z$ passes below $z$. Closing $\mathcal C_z$ upward continues to enclose the pole, even when $\operatorname{Im}z\leq0$, so

$$
\boxed{
\widetilde F(z)=\frac{2\pi i^ne^{iz}}{(n-1)!}
}
$$

there as well. The right-hand side is an [entire function](../../../../../../entire-function.md), so it is the unique analytic continuation of $F$ to the whole [complex plane](../../../../../../complex-plane.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
