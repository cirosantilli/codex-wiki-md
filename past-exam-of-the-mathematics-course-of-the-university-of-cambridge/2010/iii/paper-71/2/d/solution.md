<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [internal-wave ray tracing](../../../../../../internal-wave-ray-tracing.md) equations preserve the horizontal [wavenumber](../../../../../../wavenumber.md) $k$ and laboratory frequency. For the increasing wind, the upward branch satisfies

$$
m(z)=\frac{N_0}{U(z)}\sqrt{1-q^2(z)},\qquad
q(z)=\frac{kU(z)}{N_0}=q_0(1+z/H),\qquad q_0=\frac{kU_0}{N_0}<1.
$$

The group-velocity ratio therefore gives

$$
\frac{dx}{dz}=\frac{k}{m}=\frac{q}{\sqrt{1-q^2}}.
$$

Integrating from $(0,0)$ yields

$$
\boxed{x(z)=\frac{H}{q_0}\left[\sqrt{1-q_0^2}-\sqrt{1-q_0^2(1+z/H)^2}\right].}
$$

This is the ascending branch of the [circular mountain-wave ray in linear shear](../../../../../../circular-mountain-wave-ray-in-linear-shear.md):

$$
(x-x_t)^2+(z+H)^2=\left(\frac{H}{q_0}\right)^2,\qquad
x_t=\frac{H}{q_0}\sqrt{1-q_0^2}.
$$

It reaches $z_t=H(q_0^{-1}-1)$ at $x=x_t$, where the energy direction is horizontal. After reflection, $m<0$ and the ray continues downwind and downward along the other branch

$$
x(z)=\frac{H}{q_0}\left[\sqrt{1-q_0^2}+\sqrt{1-q_0^2(1+z/H)^2}\right],
$$

returning to $z=0$ at $x=2x_t$. The last panel of the figure in part (b) shows this path. These are WKB energy rays, with the short neighborhood of the turning height supplied by its transition solution.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
