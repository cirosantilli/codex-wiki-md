<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Axisymmetric [mass conservation](../../../../../../mass-conservation.md) in the spherical gap gives

$$
\frac{\partial h}{\partial t}
+\frac1{a\sin\theta}
\frac{\partial}{\partial\theta}(q\sin\theta)=0.
$$

Since $h_t=-V\cos\theta$ and regularity requires $q\sin\theta=0$ at $\theta=0$, integration gives

$$
q\sin\theta
=aV\int_0^\theta\sin\vartheta\cos\vartheta\,d\vartheta
=\frac12aV\sin^2\theta,
\qquad
\boxed{q=\frac12Va\sin\theta}.
$$

The leading [pressure-driven lubrication flux](../../../../../../hagen-poiseuille-equation.md) is

$$
q=-\frac{h^3}{12\mu a}\frac{dp}{d\theta}.
$$

Substitution of $h$ and $q$ gives

$$
\frac{dp}{d\theta}
=-\frac{6\mu a^2V\sin\theta}
{\Delta^3(1-\lambda\cos\theta)^3},
$$

and therefore

$$
\boxed{
p(\theta)=
\frac{3\mu a^2V}
{\lambda\Delta^3(1-\lambda\cos\theta)^2}+p_0}.
$$

Take downward as the positive vertical direction. The constant pressure contributes no resultant, while the pressure force on the inner sphere is opposite its outward normal. Thus

$$
F_z=-2\pi a^2\int_0^\pi
(p-p_0)\cos\theta\sin\theta\,d\theta.
$$

With $t=\lambda\cos\theta$ and the supplied integral,

$$
\boxed{
F_z=-\frac{6\pi\mu a^4V}{\lambda^3\Delta^3}
\left[
\frac{2\lambda}{1-\lambda^2}
+\log\left(\frac{1-\lambda}{1+\lambda}\right)
\right]}.
$$

The sign is upward for $V>0$, so this is a [drag force](../../../../../../drag-physics.md). As $\lambda\to0$, the bracket is $4\lambda^3/3+O(\lambda^5)$ and $F_z\to-8\pi\mu a^4V/\Delta^3$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
