<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Near the closest point, the cylinder–plane gap is

$$
h(x)=\frac a2\varepsilon+\frac{x^2}{2a}
=\frac a2(\varepsilon+\xi^2),
\qquad
\xi=\frac xa.
$$

For translation parallel to the cylinder axis, the leading flow is [Couette flow](../../../../../../couette-flow.md). Its shear traction is $\mu U/h$, so

$$
\frac{F_y}{U}
=\mu L\int_{-\infty}^{\infty}\frac{dx}{h(x)}
=2\mu L\int_{-\infty}^{\infty}
\frac{d\xi}{\varepsilon+\xi^2}
=\boxed{2\pi\varepsilon^{-1/2}\mu L}.
$$

Hence $A_{yy}=2\pi\varepsilon^{-1/2}\mu L$.

For transverse translation, the local [Couette-Poiseuille flow in a thin gap](../../../../../../couette-poiseuille-flow-in-a-thin-gap.md) and mass conservation give the [Reynolds lubrication equation](../../../../../../reynolds-equation.md). Writing $x=a\sqrt\varepsilon\,X$ and using pressure recovery at both ends determines its integration constant. The pressure and viscous contributions to the horizontal traction reduce to

$$
\frac{F_x}{U}
=\frac{\mu L}{\sqrt\varepsilon}
\left(16I_2-16I_3\right)
=\frac{\mu L}{\sqrt\varepsilon}
\left(8\pi-6\pi\right)
+\frac{2\pi\mu L}{\sqrt\varepsilon},
$$

where the final term is the direct Couette shear contribution. Therefore

$$
\boxed{A_{xx}=4\pi\varepsilon^{-1/2}\mu L}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
