<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

The [Biot-Savart law](../../../biot-savart-law.md) is

$$
B(r)=\frac{\mu_0I}{4\pi}\int\frac{d\ell'\times(r-r')}{|r-r'|^3}.
$$

Here $r'$ is the current-element position, $d\ell'$ follows the [electric current](../../../electric-current.md), and $r$ is the observation point. For a circular [current loop](../../../current-loop.md), transverse components cancel on the axis. Each element contributes axial factor $a/\sqrt{a^2+x^2}$ in addition to the inverse-square distance. Integrating around length $2\pi a$ gives the [on-axis magnetic field of a circular current loop](../../../on-axis-magnetic-field-of-a-circular-current-loop.md)

$$
\boxed{B_{\mathrm{axis}}(x)=\frac{\mu_0Ia^2}{2(a^2+x^2)^{3/2}},}
$$

with axial direction set by the [right-hand rule](../../../right-hand-rule.md).

For a finite straight wire parametrized by $z\in[-b,b]$, at perpendicular distance $a$, the [Biot-Savart law](../../../biot-savart-law.md) gives

$$
B=\frac{\mu_0I}{4\pi}\int_{-b}^{b}\frac{a\,dz}{(a^2+z^2)^{3/2}}
=\boxed{\frac{\mu_0Ib}{2\pi a\sqrt{a^2+b^2}}.}
$$

The direction is azimuthal about the current axis by the [right-hand rule](../../../right-hand-rule.md). In the hairpin, the semicircle contributes $\mu_0I/(4a)$ and each semi-infinite straight segment contributes $\mu_0I/(4\pi a)$. For the indicated current, all three contributions point **out of the page**. Thus the [magnetic field at the center of a hairpin wire](../../../magnetic-field-at-the-center-of-a-hairpin-wire.md) is

$$
\boxed{B(P)=\frac{\mu_0I}{4\pi a}(\pi+2),\quad\text{out of the page}.}
$$

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2018](../../2018-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
