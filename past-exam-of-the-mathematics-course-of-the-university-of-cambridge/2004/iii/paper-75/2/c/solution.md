<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A linear, or “three-thirds”, boundary [heat transfer](../../../../../../heat-transfer.md) closure needs its own dimensional conductance $L>0$, so $q=L\Delta$. One cannot simply keep the dimensions of the previous nonlinear coefficient $K$. With equal conductances at both boundaries, the mean-temperature equation becomes

$$
\rho c_ph\dot\vartheta=L(\Delta T-2\vartheta).
$$

Integrating this linear [ordinary differential equation](../../../../../../ordinary-differential-equation.md) gives

$$
\boxed{\overline T(t)=T_0+\frac{\Delta T}{2}\left[1-e^{-2Lt/(\rho c_ph)}\right],\qquad \overline T(\infty)=T_0+\frac{\Delta T}{2}}.
$$

The relaxation time is $\rho c_ph/(2L)$. If the conductances differed, [conservation of energy](../../../../../../conservation-of-energy.md) would instead select their weighted boundary temperature; the arithmetic mean follows from the assumed upper/lower symmetry.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
