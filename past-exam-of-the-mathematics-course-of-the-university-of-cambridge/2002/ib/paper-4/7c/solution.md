<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

Direct differentiation of the [velocity field](../../../../../velocity-field.md) gives $(\mathbf u\cdot\nabla)\mathbf u=(-\Omega^2x,-\Omega^2y,0)$. Since $u^2=\Omega^2(x^2+y^2)$, this equals $\nabla(-u^2/2)$ as required.

In cylindrical coordinates, steady rigid rotation has $u_r=u_z=0$, $u_\theta=\Omega r$. The radial and vertical [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) for constant-density fluid are $p_r=\rho\Omega^2r$ and $p_z=-\rho g$, hence $p=\rho(\Omega^2r^2/2-gz)+C$. Constant atmospheric pressure on the [free surface](../../../../../free-surface.md) gives $z_s(r)=H+\Omega^2r^2/(2g)$. Conservation of fluid volume determines $H$:

$$
\pi a^2h=2\pi\int_0^a z_s(r)r\,dr=\pi a^2H+\frac{\pi\Omega^2a^4}{4g}.
$$

Therefore

$$
\boxed{z_s(r)=h+\frac{\Omega^2}{2g}\left(r^2-\frac{a^2}{2}\right).}
$$

The lowest point is the axis, where $z_s(0)=h-\Omega^2a^2/(4g)$. The [free surface](../../../../../free-surface.md) first meets the bottom when

$$
\boxed{|\Omega|=\frac{2\sqrt{gh}}a.}
$$

This assumes no overflow and uses the full disk of wetted bottom until first contact. Once a dry central region forms, the volume constraint and geometry must be modified.

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
