<h1 id="30e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $G(x,y,t)=\Psi(x+y/2,t)\overline\Psi(x-y/2,t)$. The [Schrödinger equation](../../../../../../schrodinger-equation.md) and its conjugate give

$$
\partial_tG=\frac i2(\Delta_+-\Delta_-)G=i\nabla_x\cdot\nabla_yG,
$$

since $\nabla_x=\nabla_++\nabla_-$ and $\nabla_y=(\nabla_+-\nabla_-)/2$. In the [Wigner transform](../../../../../../wigner-distribution.md), integration by parts turns $\nabla_y$ into $i\xi$, yielding the free transport equation

$$
\boxed{\partial_tw+\xi\cdot\nabla_xw=0.}
$$

Along its characteristics $x(t)=x_0+t\xi$, the value is constant. Thus

$$
\boxed{w(x,\xi,t)=g(x-t\xi,\xi).}
$$

For rapidly decreasing smooth data every integration by parts is justified; weaker data follow distributionally.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30E](../../30e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
