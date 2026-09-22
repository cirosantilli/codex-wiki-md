<h1 id="k/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Milne-Thomson's circle theorem](../../../../milne-thomson-circle-theorem.md) inserts an impermeable circular boundary into a two-dimensional [irrotational](../../../../irrotational-vector-field.md) [incompressible flow](../../../../incompressible-flow.md). If $f(z)$ is analytic in a neighborhood of the [closed disc](../../../../closed-disc.md) and its flow singularities lie outside, the new complex potential outside $|z|=a$ is

$$
\boxed{w(z)=f(z)+\overline{f(a^2/\bar z)}.}
$$

Reflection and coefficient conjugation make the second term analytic outside the [circle](../../../../circle.md), with its image singularities inside. On $|z|=a$, $a^2/\bar z=z$, so the two terms sum to $2\operatorname{Re}f(z)$: the [streamfunction](../../../../stream-function.md) is constant there. Thus no [velocity](../../../../velocity.md) crosses the [circle](../../../../circle.md). At infinity the image term tends to the constant $\overline{f(0)}$, which has no effect on [velocity](../../../../velocity.md), and the far-field flow is retained. This proves the construction, with an additive potential constant immaterial.

Put $A=\mu e^{i\alpha}$, $B=\mu e^{-i\alpha}$. For the dipole the reflected potential is $B/(a^2/z-b)=Bz/(a^2-bz)$, giving

$$
\boxed{w(z)=\frac{A}{z-b}+\frac{Bz}{a^2-bz}.}
$$

Its image pole is $c=a^2/b$, inside the [cylinder](../../../../cylinder-geometry.md). The [complex velocity](../../../../complex-velocity.md) is

$$
w'(z)=-\frac A{(z-b)^2}+\frac{Ba^2}{(a^2-bz)^2}.
$$

Near $c$, the second term is $C(z-c)^{-2}$ with $C=Ba^2/b^2$, while $v_0(z)=-A/(z-b)^2$ is analytic there. The square of the pole term has no [residue](../../../../residue.md), nor does $v_0^2$. The cross term has [residue](../../../../residue.md) $2Cv_0'(c)$, so

$$
\operatorname{Res}_{z=c}(w')^2
=\frac{4ABa^2b}{(a^2-b^2)^3}
=-\frac{4\mu^2a^2b}{(b^2-a^2)^3}.
$$

Take the contour counterclockwise around the [cylinder](../../../../cylinder-geometry.md), as in the supplied [Blasius force theorem](../../../../blasius-force-theorem.md). The [residue theorem](../../../../residue-theorem.md) gives $\tfrac12i\rho\oint(w')^2dz=-\pi\rho\operatorname{Res}(w')^2$. Therefore

$$
\boxed{F_x=\frac{4\pi\rho\mu^2a^2b}{(b^2-a^2)^3},\qquad F_y=0.}
$$

The force points toward the dipole. Its independence of dipole orientation follows from the product $AB=\mu^2$ in the sole [residue](../../../../residue.md) contribution.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [K](../../k.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
