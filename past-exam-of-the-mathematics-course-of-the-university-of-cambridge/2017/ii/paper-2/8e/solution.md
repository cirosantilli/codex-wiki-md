<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

For variations vanishing at both endpoints, differentiating the [action](../../../../../action.md) and using [integration by parts](../../../../../integration-by-parts.md) gives

$$
\delta S=\int_{t_0}^{t_1}\sum_i\left(\frac{\partial L}{\partial q_i}-\frac{d}{dt}\frac{\partial L}{\partial\dot q_i}\right)\delta q_i\,dt.
$$

The [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore yields the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md)

$$
\boxed{\frac{d}{dt}\frac{\partial L}{\partial\dot q_i}=\frac{\partial L}{\partial q_i}.}
$$

For the specified [Lagrangian](../../../../../lagrangian.md), the [gauge transformation](../../../../../gauge-transformation.md) changes it by

$$
\Delta L=\dot{\mathbf r}\cdot\nabla F-\alpha F_t
=\frac{dF}{dt}-(\alpha+1)F_t.
$$

For arbitrary $F$, it is a [total derivative](../../../../../total-derivative.md) precisely when $\boxed{\alpha=-1}$. The corresponding change in [action](../../../../../action.md) is then an endpoint term whose variation is zero. In general time-dependent notation, the equations are

$$
m\ddot{\mathbf r}=-\nabla\phi-\partial_t\mathbf A+\dot{\mathbf r}\times(\nabla\times\mathbf A).
$$

The [electric field](../../../../../electric-field.md) $-\nabla\phi-\partial_t\mathbf A$ and [magnetic field](../../../../../magnetic-field.md) $\nabla\times\mathbf A$ are unchanged by the [gauge transformation](../../../../../gauge-transformation.md) with $\alpha=-1$. Although the original potentials have no time dependence, their transformed versions generally do; allowing this is essential to the stated invariance.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
