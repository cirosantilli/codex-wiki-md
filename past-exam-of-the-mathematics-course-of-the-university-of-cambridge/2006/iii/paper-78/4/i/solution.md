<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $V=\Delta\dot\alpha$, positive downwards. Then $h_t=-V\cos\theta$. The leading axisymmetric [lubrication](../../../../../../lubrication-theory.md) flux is $q_\theta=-h^3p_\theta/(12\mu a)$. Wall Couette flux from the translating sphere is smaller by $\Delta/a$ than the squeeze flux and does not affect this leading [pressure](../../../../../../pressure.md). The spherical [Reynolds lubrication equation](../../../../../../reynolds-equation.md) is

$$
h_t+\frac1{a\sin\theta}\partial_\theta(\sin\theta\,q_\theta)=0.
$$

Regularity at the pole gives $q_\theta=(aV/2)\sin\theta$, so

$$
p_\theta=-\frac{6\mu a^2V\sin\theta}{\Delta^3(1-\alpha\cos\theta)^3},\qquad
\boxed{p=\frac{3\mu a^2V}{\alpha\Delta^3(1-\alpha\cos\theta)^2}+p_*}.
$$

The apparent singularity at $\alpha=0$ is a constant-pressure gauge term: subtract $3\mu a^2V/(\alpha\Delta^3)$ before taking the limit. The remaining [pressure](../../../../../../pressure.md) tends to $6\mu a^2V\cos\theta/\Delta^3$.

To leading lubrication order the [force](../../../../../../force.md) is the [pressure](../../../../../../pressure.md) integral. Its downward component on the inner sphere is

$$
F_z=-2\pi a^2\int_0^\pi p\cos\theta\sin\theta\,d\theta
=-\frac{6\pi\mu a^4V}{\alpha^3\Delta^3}\int_{-\alpha}^{\alpha}\frac{t}{(1-t)^2}\,dt.
$$

The original PDF's first integration hint is incorrect: the rational term needs $1-b^2$, not $(1-b)^2$. From the antiderivative $1/(1-t)+\log(1-t)$,

$$
\int_{-b}^b\frac{t}{(1-t)^2}\,dt=\frac{2b}{1-b^2}+\log\frac{1-b}{1+b}.
$$

Thus the [squeeze resistance of eccentric nested spheres](../../../../../../squeeze-resistance-of-eccentric-nested-spheres.md) gives

$$
\boxed{F_z=-\frac{6\pi\mu a^4V}{\alpha^3\Delta^3}\left[\frac{2\alpha}{1-\alpha^2}+\log\frac{1-\alpha}{1+\alpha}\right].}
$$

It opposes the [velocity](../../../../../../velocity.md) for either sign of $\alpha$. The continuous concentric limit is $F_z=-8\pi\mu a^4V/\Delta^3$, since the bracket is $4\alpha^3/3+O(\alpha^5)$. As $\alpha\to1$, its leading magnitude is $6\pi\mu a^4|V|/[\Delta^3(1-\alpha)]$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
