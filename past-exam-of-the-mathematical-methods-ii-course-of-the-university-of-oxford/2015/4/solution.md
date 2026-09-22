<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $r=\sqrt{x^2+y^2+z^2}>0$, the [radial vector field](../../../radial-vector-field.md) has components $F_i=x_if(r)$. The [product rule](../../../product-rule.md) gives

$$
\nabla\cdot\mathbf F=\sum_i\left[f(r)+x_if'(r)\frac{x_i}{r}\right]=3f(r)+rf'(r).
$$

Thus for $f(r)=r^{n-1}$,

$$
\boxed{\nabla\cdot\mathbf F=(n+2)r^{n-1},\qquad r>0}.
$$

When $n=-2$, $\mathbf F=\hat{\mathbf r}/r^2$ and the ordinary [divergence](../../../divergence.md) is zero at every nonzero radius. However, the field is singular at the origin. Its outward [flux](../../../flux.md) through a radius-$R$ sphere is $(1/R^2)(4\pi R^2)=4\pi$, so one cannot apply the smooth-field [divergence theorem](../../../divergence-theorem.md) across the origin and conclude that this flux vanishes.

In the language of [distributions](../../../distribution-mathematical-analysis.md), the complete [distributional divergence](../../../distributional-divergence.md) identity is $\boxed{\nabla\cdot(\hat{\mathbf r}/r^2)=4\pi\delta^{(3)}(\mathbf r)}$. Here $\delta^{(3)}$ is the three-dimensional [Dirac delta function](../../../dirac-delta-function.md). Without that generalized interpretation, the correct statement is simply zero divergence away from the origin and undefined ordinary divergence at the singular point. Removing a small ball around the origin restores the ordinary theorem: the inner boundary has inward radial orientation and cancels the outer flux.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2015](../../2015-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
