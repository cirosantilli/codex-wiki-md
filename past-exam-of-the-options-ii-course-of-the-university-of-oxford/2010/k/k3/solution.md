<h1 id="k/k3/solution">Solution</h1>

↑ **Parent:** [K3](../k3.md)

The [Milne-Thomson circle theorem](../../../../milne-thomson-circle-theorem.md) says that if a complex potential $f(z)$ has no singularities on or inside $|z|=a$, then a circular impermeable boundary can be introduced by taking

$$
W(z)=f(z)+f^*(a^2/z),\qquad f^*(w)=\overline{f(\overline w)}.
$$

The new singularities are the reflected ones inside the circle. On $|z|=a$, $a^2/z=\overline z$, so $W(z)=f(z)+\overline{f(z)}$ is real; the [stream function](../../../../stream-function.md) is constant and there is no normal velocity. At infinity the added term tends to $f^*(0)$, a harmless potential constant, so it preserves the far-[field](../../../../field.md) flow. This proves the theorem with zero added net [circulation](../../../../circulation-physics.md) about the cylinder. A logarithmic term may then specify a different cylinder [circulation](../../../../circulation-physics.md).

For $f(z)=-i\Gamma\log(z-b)/(2\pi)$, put $c=a^2/b$. The reflected term is

$$
f^*(a^2/z)=\frac{i\Gamma}{2\pi}\log(a^2/z-b)
=\frac{i\Gamma}{2\pi}\log(z-c)-\frac{i\Gamma}{2\pi}\log z+\text{constant},
$$

with locally consistent logarithm branches. The circle-theorem solution has zero cylinder [circulation](../../../../circulation-physics.md): its image [vortex](../../../../phase-vortex.md) at $c$ and its central [vortex](../../../../phase-vortex.md) cancel. To impose [circulation](../../../../circulation-physics.md) $-\Gamma$, add $i\Gamma\log z/(2\pi)$. The result is

$$
\boxed{w(z)=-\frac{i\Gamma}{2\pi}\log(z-b)
+\frac{i\Gamma}{2\pi}\log(z-c)+\text{constant}.}
$$

It consists of the physical [vortex](../../../../phase-vortex.md) and an opposite image [vortex](../../../../phase-vortex.md) inside the obstacle. On the circle, $|z-b|=(b/a)|z-c|$, so its [stream function](../../../../stream-function.md) is indeed constant.

The [complex velocity](../../../../complex-velocity.md) is

$$
q(z)=w'(z)=-\frac{i\Gamma}{2\pi}
\left(\frac1{z-b}-\frac1{z-c}\right).
$$

Inside the positively oriented obstacle contour, $q^2$ has only the double pole at $c$. Its [residue](../../../../residue.md) is

$$
\operatorname{Res}_{z=c}q(z)^2
=\left.\frac d{dz}\left[-\frac{\Gamma^2(b-c)^2}{4\pi^2(z-b)^2}\right]\right|_{z=c}
=-\frac{\Gamma^2}{2\pi^2(b-c)}.
$$

The [residue theorem](../../../../residue-theorem.md) and the supplied [Blasius force theorem](../../../../blasius-force-theorem.md) therefore give

$$
F_x-iF_y=\frac{i\rho}{2}(2\pi i)\left[-\frac{\Gamma^2}{2\pi^2(b-c)}\right]
=\frac{\rho\Gamma^2}{2\pi(b-c)}.
$$

Consequently

$$
\boxed{F_x=\frac{\rho\Gamma^2b}{2\pi(b^2-a^2)},\qquad F_y=0.}
$$

The force points toward the held [vortex](../../../../phase-vortex.md), independent of the sign of its [circulation](../../../../circulation-physics.md).

The residue calculation is the [force on a circular cylinder from a held exterior vortex](../../../../force-on-a-circular-cylinder-from-a-held-exterior-vortex.md).

## ↑ Ancestors (12)

1. [K3](../k3.md)
2. [K](../../k.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
