<h1 id="39c/solution">Solution</h1>

↑ **Parent:** [39C](../39c.md)

Take downward [velocity](../../../../../velocity.md) as positive. Lubrication theory reduces the axial [momentum](../../../../../momentum.md) equation to a constant [pressure](../../../../../pressure.md) [gradient](../../../../../gradient.md), and the no-slip conditions are $u(0)=0$, $u(h)=U$. Twice integrating gives

$$
\boxed{u(y)=-\frac{\Delta p}{2\mu L}y(h-y)+U\frac yh.}
$$

The flux per unit circumference and the total gap flux are

$$
q=\int_0^hu(y)dy
=-\frac{\Delta p\,h^3}{12\mu L}+\frac{Uh}{2},
\qquad
Q\simeq2\pi a q.
$$

The shear at the cylinder is

$$
\boxed{
\tau_h=\mu u_y(h)=\frac{\Delta p\,h}{2L}+\frac{\mu U}{h},}
$$

with the fluid traction on the falling cylinder opposing its motion.

The descending solid displaces volume at rate $\pi a^2U$, so closed-container mass conservation gives

$$
2\pi a\left(-\frac{\Delta p\,h^3}{12\mu L}+\frac{Uh}{2}\right)
=-\pi a^2U.
$$

Since $h\ll a$, the Couette-flux term is smaller, and

$$
\boxed{\Delta p\simeq\frac{6\mu aLU}{h^3}.}
$$

The [pressure](../../../../../pressure.md) or form drag is

$$
F_p\simeq\pi a^2\Delta p
=\frac{6\pi\mu a^3LU}{h^3}.
$$

Using the pressure-dominated part of $\tau_h$, the side shear force is of order

$$
F_\mu\simeq2\pi aL\frac{\Delta p h}{2L}
=\frac{6\pi\mu a^2LU}{h^2},
$$

so $F_p/F_\mu\simeq a/h\gg1$. Balancing form drag against the excess weight $\Delta\rho g\pi a^2L$ gives

$$
\boxed{U\simeq\frac{\Delta\rho\,g h^3}{6\mu a}.}
$$

This is [annular lubrication drag on a settling cylinder](../../../../../annular-lubrication-drag-on-a-settling-cylinder.md).

## ↑ Ancestors (10)

1. [39C](../39c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
