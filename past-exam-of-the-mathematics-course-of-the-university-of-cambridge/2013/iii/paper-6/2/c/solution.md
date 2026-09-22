<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Separate the transported initial datum from the gain term. Define

$$
F(f_0)(t,x,v)=e^{-t}f_0(x-tv,v),
$$

and the [Boltzmann Volterra operator](../../../../../../boltzmann-volterra-operator.md)

$$
(\tau f)(t,x,v)=\int_0^t e^{-(t-s)}\int_{\mathbb R^d}
k\bigl(s,x-(t-s)v,v,v_*\bigr)f\bigl(s,x-(t-s)v,v_*\bigr)\,dv_*\,ds.
$$

The [Duhamel principle](../../../../../../duhamel-s-principle.md) makes the [linear Boltzmann equation](../../../../../../linear-boltzmann-equation.md) equivalent, whenever the [integrals](../../../../../../integral.md) and solution are legitimate, to

$$
\boxed{f=F(f_0)+\tau f}.
$$

The gain samples velocities $v_*$ at the backward spatial position of the outgoing velocity $v$; replacing that spatial shift by one depending on $v_*$ would give a different equation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
