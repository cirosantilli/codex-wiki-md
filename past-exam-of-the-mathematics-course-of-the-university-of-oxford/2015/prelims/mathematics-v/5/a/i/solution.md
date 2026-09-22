<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $w$ be the difference of two sufficiently regular solutions of the [wave equation](../../../../../../../wave-equation-split.md) with the prescribed data. By [linearity](../../../../../../../linearity.md), $w$ has zero [initial displacement](../../../../../../../initial-displacement.md), zero [initial velocity](../../../../../../../initial-velocity.md), and homogeneous [Dirichlet boundary conditions](../../../../../../../dirichlet-boundary-condition.md). Define its [wave energy](../../../../../../../wave-energy.md) by

$$
E(t)=\frac12\int_0^\pi(w_t^2+w_x^2)\,dx\geq0.
$$

For $\alpha=0$, [differentiation under the integral sign](../../../../../../../differentiation-under-the-integral-sign.md) and [integration by parts](../../../../../../../integration-by-parts.md) yield

$$
E'(t)=\int_0^\pi w_t(w_{tt}-w_{xx})\,dx+[w_tw_x]_0^\pi=0.
$$

The [boundary term](../../../../../../../boundary-term.md) vanishes because $w=0$ at both fixed endpoints implies $w_t=0$ there. The zero [initial data](../../../../../../../initial-data-in-general-relativity.md) give $E(0)=0$, so $w_t=w_x=0$ for all times. Thus $w$ is spatially constant, and its zero [boundary values](../../../../../../../boundary-value.md) give $\boxed{w=0}$. This proves [uniqueness](../../../../../../../uniqueness.md) for the undamped [wave equation](../../../../../../../wave-equation-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
