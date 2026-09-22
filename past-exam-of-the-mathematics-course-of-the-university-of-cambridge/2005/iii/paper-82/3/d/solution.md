<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If two harmonic solutions have the same [body force](../../../../../../body-force.md) and prescribed boundary [traction](../../../../../../traction.md), their difference has no [body force](../../../../../../body-force.md) and is traction-free. A nonzero difference would therefore be a free [eigenfunction](../../../../../../eigenfunction.md) at that [frequency](../../../../../../frequency.md). For any [frequency](../../../../../../frequency.md) outside the countable exceptional set found above, **the difference must vanish**, so the forced boundary-value solution, when it exists, is unique. At an [eigenfrequency](../../../../../../eigenfrequency.md), a free [eigenfunction](../../../../../../eigenfunction.md) can be added to any existing solution, and a resonant forcing may fail to admit a steady harmonic response. This distinguishes uniqueness from existence.

For the full time-dependent problem, let $\mathbf w$ be the difference between two fields with identical forces, [tractions](../../../../../../traction.md) and initial [displacement field](../../../../../../displacement-field-mechanics.md) and [velocity](../../../../../../velocity.md). It obeys $\rho\mathbf w_{tt}=\nabla\cdot\boldsymbol\sigma(\mathbf w)$, zero boundary [traction](../../../../../../traction.md), and zero initial data. Its [energy uniqueness for traction-driven elasticity](../../../../../../energy-uniqueness-for-traction-driven-elasticity.md) follows by direct [integration](../../../../../../integral.md):

$$
E(t)=\frac12\int_{\mathcal D}\left[\rho|\mathbf w_t|^2+c_{ijpq}e_{ij}(\mathbf w)e_{pq}(\mathbf w)\right]dV,\qquad e_{ij}=\frac12(\partial_iw_j+\partial_jw_i).
$$

Multiply the equation by $\mathbf w_t$ and integrate by parts. Major symmetry turns the [strain](../../../../../../strain.md) term into the [derivative](../../../../../../derivative.md) of [elastic energy](../../../../../../elastic-energy.md), giving $E'(t)=\int_{\partial\mathcal D}\mathbf w_t\cdot\mathbf t(\mathbf w)dS=0$. Stable [elasticity](../../../../../../elasticity-physics.md) makes $E\geq0$, and $E(0)=0$ gives $\mathbf w_t=0$. Thus $\mathbf w$ equals its initial value zero. Even rigid zero-strain motions cannot survive these [initial conditions](../../../../../../initial-condition.md).

The PDF correctly specifies zero initial [displacement field](../../../../../../displacement-field-mechanics.md) and zero initial [velocity](../../../../../../velocity.md); the TeX duplicates [displacement field](../../../../../../displacement-field-mechanics.md) in the second condition. **The complete causal [displacement field](../../../../../../displacement-field-mechanics.md) is unique**, including when its Fourier representation contains resonant modal contributions fixed by the initial data.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
