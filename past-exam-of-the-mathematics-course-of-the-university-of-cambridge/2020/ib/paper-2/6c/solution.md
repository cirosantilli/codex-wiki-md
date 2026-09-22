<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Let the upper plate in flow A move at speed $U$, with the lower plate fixed. The [Couette flow](../../../../../couette-flow.md) profile is

$$
u_A(y)=\frac Uh\,y,
$$

so its mid-plane speed is $U/2$ and its total [viscous dissipation](../../../../../viscous-dissipation.md) per unit plate area is

$$
\dot Q_A=\int_0^h\mu\left(\frac Uh\right)^2dy
=\frac{\mu U^2}{h}.
$$

Write $G=-dp/dx>0$ for the constant pressure-gradient magnitude in flow B. The [plane Poiseuille flow](../../../../../plane-poiseuille-flow.md) profile is

$$
u_B(y)=\frac{G}{2\mu}y(h-y).
$$

Equality of the mid-plane speeds gives

$$
\frac{Gh^2}{8\mu}=\frac U2,
\qquad
G=\frac{4\mu U}{h^2}.
$$

Since $u_B'(y)=G(h-2y)/(2\mu)$,

$$
\dot Q_B
=\frac{G^2}{4\mu}\int_0^h(h-2y)^2dy
=\frac{G^2h^3}{12\mu}
=\frac{4\mu U^2}{3h}.
$$

Hence

$$
\boxed{\frac{\dot Q_A}{\dot Q_B}=\frac34}.
$$

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
