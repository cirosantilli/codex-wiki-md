<h1 id="question-2/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

Use [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md) $(\rho,\theta,z)$. The [right circular cone](../../../../../../right-circular-cone.md) is described by $0\leq z\leq1$ and $0\leq\rho\leq a(1-z)$, and the [divergence](../../../../../../divergence.md) of $\mathbf F=(0,0,z^2)$ is $2z$. Direct [integration](../../../../../../integral-split.md) gives

$$
\begin{aligned}
\iiint_R\nabla\cdot\mathbf F\,dV
&=\int_0^1\int_0^{2\pi}\int_0^{a(1-z)}2z\rho\,d\rho\,d\theta\,dz\\
&=2\pi a^2\int_0^1z(1-z)^2\,dz\\
&=2\pi a^2\left(\frac12-\frac23+\frac14\right)
=\boxed{\frac{\pi a^2}6}.
\end{aligned}
$$

To check the boundary [flux integral](../../../../../../flux-integral.md) independently, first consider the base $z=0$. Its outward [unit normal vector](../../../../../../unit-normal.md) is $-\mathbf k$, but $\mathbf F=\mathbf0$ there, so its [flux](../../../../../../flux.md) is zero. Parametrize the lateral [surface](../../../../../../topological-surface-split.md) by

$$
\mathbf s(\theta,z)=\bigl(a(1-z)\cos\theta,a(1-z)\sin\theta,z\bigr),
\qquad0\leq\theta\leq2\pi,\quad0\leq z\leq1.
$$

The [cross product](../../../../../../cross-product.md)

$$
\mathbf s_\theta\times\mathbf s_z
=\bigl(a(1-z)\cos\theta,a(1-z)\sin\theta,a^2(1-z)\bigr)
$$

points outward: its horizontal component points away from the axis of the [cone](../../../../../../cone-geometry.md). This gives the [vector surface element](../../../../../../vector-area-element.md) without separately normalizing it. Consequently the lateral [flux integral](../../../../../../flux-integral.md) is

$$
\int_0^1\int_0^{2\pi}
\mathbf F(\mathbf s)\cdot(\mathbf s_\theta\times\mathbf s_z)\,d\theta\,dz
=2\pi a^2\int_0^1z^2(1-z)\,dz
=2\pi a^2\left(\frac13-\frac14\right)
=\boxed{\frac{\pi a^2}6}.
$$

Adding the zero base contribution agrees with the [volume integral](../../../../../../volume-integral.md), verifying the [divergence theorem](../../../../../../divergence-theorem.md). The apex has zero [surface area](../../../../../../surface-area.md); the [vector field](../../../../../../vector-field.md) is smooth there, so no additional [flux](../../../../../../flux.md) is hidden at that point.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [Question 2](../../question-2.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
