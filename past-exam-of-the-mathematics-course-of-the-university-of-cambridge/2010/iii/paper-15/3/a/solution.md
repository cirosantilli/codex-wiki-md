<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [oriented atlas](../../../../../../oriented-atlas.md) is a [smooth atlas](../../../../../../smooth-atlas.md) whose [smooth transition maps](../../../../../../smooth-transition-map.md) have positive [Jacobian determinants](../../../../../../jacobian-determinant.md) at every point of their domains. Such an atlas supplies an [orientation of a vector space](../../../../../../orientation-of-a-vector-space.md) on every [tangent space](../../../../../../tangent-space.md), and these choices agree on overlaps.

Let $\omega$ be a nowhere-vanishing smooth top-degree [differential form](../../../../../../differential-form-split.md). In a [coordinate chart](../../../../../../manifold-chart.md) write

$$
\omega=f(x)\,dx^1\wedge\cdots\wedge dx^n.
$$

The coefficient $f$ is smooth and nowhere zero. Restrict the [coordinate chart](../../../../../../manifold-chart.md) to connected neighborhoods; the [intermediate value theorem](../../../../../../intermediate-value-theorem.md) makes the sign of $f$ constant on each. If $f$ is negative, replacing $x^1$ by $-x^1$ changes the sign of the coordinate [volume form](../../../../../../volume-form.md). Thus for $n\geq1$ we can choose a covering of [coordinate charts](../../../../../../manifold-chart.md) in each of which the coefficient is positive.

On an overlap of two such [coordinate charts](../../../../../../manifold-chart.md), the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md) transforms by

$$
dx^1\wedge\cdots\wedge dx^n
=\det\left(\frac{\partial x}{\partial y}\right)
dy^1\wedge\cdots\wedge dy^n.
$$

Consequently $f_y=f_x\det(\partial x/\partial y)$. Both coefficients are positive, so the [Jacobian determinant](../../../../../../jacobian-determinant.md) is positive, as is that of the inverse transition. **A nowhere-vanishing top form therefore determines an oriented atlas.** The zero-dimensional case has only zero-dimensional transitions, whose determinant is one, and is automatically orientable. Connectedness of $M$ is not needed for the positive-dimensional construction; only the local sign choice matters.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
