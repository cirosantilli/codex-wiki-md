<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

At the sheet, the second-order conditions are $\psi_{2x}(0)=0$ and $\psi_{2y}(0)=-f_d''(0)\sin^2\theta$. At the wall, $\psi_{2x}(d)=0$ and $\psi_{2y}(d)=\overline U_2$. The general solution has a polynomial mean mode and a second harmonic with exponentials $e^{\pm2y}$, as in the unbounded calculation.

Let $\overline u_2(y)=\langle\psi_{2y}\rangle$. The averaged [Stokes equation](../../../../../../stokes-equation.md), with periodic pressure and no imposed mean pressure gradient, gives $\overline u_2''=0$. The total horizontal hydrodynamic force on the sheet is opposite to the mean shear force on the flat wall. Since the swimmer is [force-free](../../../../../../force-free.md), $\overline u_2'(d)=0$, making the mean velocity constant. Matching its values at the sheet and wall therefore gives

$$
\overline U_2=-\frac12 f_d''(0).
$$

The previous part gives $f_d''(0)=1-2\sinh^2d/\Delta=-(\sinh^2d+d^2)/\Delta$, hence

$$
\boxed{\overline U_2=\frac{\sinh^2d+d^2}{2(\sinh^2d-d^2)}.}
$$

This determines the speed without solving the second-harmonic flow. The force constraint matters: prescribing a translating sheet without imposing zero net force would allow a mean shear and would not determine a unique swimming speed.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 334](../../../paper-334-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
