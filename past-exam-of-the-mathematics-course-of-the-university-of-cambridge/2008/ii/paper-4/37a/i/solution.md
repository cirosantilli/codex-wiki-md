<h1 id="37a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Axisymmetric incompressibility is $\partial_r(ru_r)+r\partial_zu_z=0$. Multiply the radial momentum equation by $r$ and use this to put advection in conservative form:

$$
\partial_r(ru_r^2)+r\partial_z(u_ru_z)=\nu r\partial_z^2u_r.
$$

Integrating through the layer gives

$$
\frac{dF}{dr}=r[\nu\partial_zu_r-u_ru_z]_{-\infty}^{\infty}=0.
$$

The boundary terms vanish because radial velocity and its shear decay into the surrounding fluid; an entrainment velocity need not itself vanish as long as its product with $u_r$ does. Hence

$$
\boxed{F=\int_{-\infty}^{\infty}ru_r^2\,dz\text{ is independent of }r.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [37A](../../37a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
