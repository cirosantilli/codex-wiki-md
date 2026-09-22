<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $G=\Delta p/L>0$, with flow in the positive $z$ direction, so $dp/dz=-G$. Balancing pressure forces and wall shear on a cylindrical fluid volume of radius $R$ and length $L$ gives

$$
\Delta p\,\pi R^2=2\pi RL\,\tau_R,
\qquad
\boxed{\tau_R=\frac{\Delta p\,R}{2L}=\frac{GR}{2}}.
$$

Thus the wall stress is fixed before any [constitutive equation](../../../../../../constitutive-equation.md) is specified.

For fully developed [pipe flow](../../../../../../pipe-flow.md), the axial Cauchy equation reduces to

$$
-G=\frac1r\frac d{dr}(r\tau_{rz}).
$$

Regularity at the axis removes the $1/r$ integration constant, so

$$
\boxed{\tau_{rz}(r)=-\frac{Gr}{2}
=-\tau_R\frac rR}.
$$

Its magnitude rises linearly from zero at the axis to $\tau_R$ at the wall.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
