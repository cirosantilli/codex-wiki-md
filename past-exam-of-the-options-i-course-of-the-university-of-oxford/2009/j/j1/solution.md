<h1 id="j/j1/solution">Solution</h1>

↑ **Parent:** [J1](../j1.md)

For a [field](../../../../field.md) point in the plane of the loop, both the directed line element $d\mathbf s$ and the displacement $\mathbf r-\mathbf s$ lie in that plane. Their [cross product](../../../../cross-product.md) is normal to it, so every term of the [Biot-Savart law](../../../../biot-savart-law.md) is normal, and their integral is normal as well. This argument also allows the [field](../../../../field.md) to vanish at particular points.

Choose the loop in the $xy$-plane with centre at the origin and let positive current be counterclockwise as seen from $+z$. On its lower side, write $\mathbf s=(t,-a,0)$, $-a\leq t\leq a$, so

$$
d\mathbf s\times(-\mathbf s)=a\,dt\,\mathbf e_z.
$$

That side contributes

$$
\frac{\mu_0I}{4\pi}\int_{-a}^a\frac{a\,dt}{(t^2+a^2)^{3/2}}\,\mathbf e_z
=\frac{\mu_0I}{4\pi}\left[\frac{t}{a\sqrt{t^2+a^2}}\right]_{-a}^a\mathbf e_z
=\frac{\sqrt2\mu_0I}{4\pi a}\mathbf e_z.
$$

All four contributions have the same direction and size by [rotation](../../../../rotation-mathematics.md). Thus

$$
\boxed{\mathbf B(0)=\frac{\sqrt2\mu_0I}{\pi a}\,\mathbf n},
$$

where $\mathbf n$ follows the [right-hand rule](../../../../right-hand-rule.md) for the current.

## ↑ Ancestors (12)

1. [J1](../j1.md)
2. [J](../../j.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
