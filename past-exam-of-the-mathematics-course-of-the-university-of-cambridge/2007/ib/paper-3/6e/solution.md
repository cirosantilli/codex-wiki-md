<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

For a differentiable equality constraint, the [Lagrange multiplier](../../../../../lagrange-multiplier.md) method finds candidate [extrema](../../../../../maximum-and-minimum.md) by solving

$$
\nabla f=\lambda\nabla g,\qquad g=c.
$$

The condition requires $\nabla g\ne0$ at the point: every tangent direction to the constraint is perpendicular to $\nabla g$, and at a [extremum](../../../../../maximum-and-minimum.md) the directional [derivative](../../../../../derivative.md) of $f$ vanishes in every such direction. Thus $\nabla f$ is parallel to $\nabla g$. One must then classify candidates and check any singular or boundary cases.

For the [ellipsoid](../../../../../ellipsoid.md), its constraint [gradient](../../../../../gradient.md) never vanishes on the surface, and its [compactness](../../../../../compact-space.md) guarantees a maximum and a minimum. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations become

$$
y=\frac{2\lambda x}{a^2},\qquad x=\frac{2\lambda y}{b^2},\qquad0=\frac{2\lambda z}{c^2}.
$$

If $\lambda=0$, then $x=y=0$ and $z=\pm c$, giving value $0$. If $\lambda\ne0$, then $z=0$; neither $x$ nor $y$ can vanish on this part of the surface. Combining the first two equations gives $4\lambda^2=a^2b^2$, and then $y=\pm(b/a)x$. The constraint yields $x^2=a^2/2$ and $y^2=b^2/2$. Therefore

$$
\boxed{\max xy=\frac{ab}{2},\qquad\min xy=-\frac{ab}{2}.}
$$

The maximum occurs at $(a/\sqrt2,b/\sqrt2,0)$ and its negative; the minimum at $(a/\sqrt2,-b/\sqrt2,0)$ and its negative. To verify these are the global [extrema](../../../../../maximum-and-minimum.md), use

$$
\frac{2|xy|}{ab}\leq\frac{x^2}{a^2}+\frac{y^2}{b^2}\leq1.
$$

Equality is attained at exactly the points just found. The remaining two candidates have value $0$ between the extremal values.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
