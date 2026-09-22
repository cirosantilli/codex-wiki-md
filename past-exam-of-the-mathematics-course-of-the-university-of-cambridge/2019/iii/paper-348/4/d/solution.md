<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define $T^\dagger(0)=0$; the printed quotient is undefined at the origin, but this continuous extension changes no transport cost because $\mu(\{0\})=0$. In [polar coordinates](../../../../../../polar-coordinates.md), the two [probability density functions](../../../../../../probability-density-function.md) give

$$
\mu\{|x|\leq r\}=r^2,\qquad
\nu\{|y|\leq s\}=s^4\quad(0\leq r,s\leq1).
$$

Both angular distributions are uniform, with [independence](../../../../../../independent-random-variables.md) of angle and radius. The proposed [transport map](../../../../../../transport-map.md) preserves the angle and sends $r$ to $s=\sqrt r$. Therefore

$$
\mu\{|T^\dagger(x)|\leq s\}=\mu\{|x|\leq s^2\}=s^4,
$$

and preservation of the angle proves $(T^\dagger)_\#\mu=\nu$. As a local check using the [Jacobian determinant](../../../../../../jacobian-determinant.md), its radial and tangential derivatives for $r>0$ are $1/(2\sqrt r)$ and $1/\sqrt r$, respectively, so $\det DT^\dagger=1/(2r)$ and $g(T^\dagger(x))\det DT^\dagger(x)=(2r/\pi)/(2r)=f(x)$.

Now use the [convex function](../../../../../../convex-function.md)

$$
\Phi(x)=\frac23|x|^{3/2}\quad(x\in\mathbb R^2).
$$

It is [convex](../../../../../../convex-function.md) because the [Euclidean norm](../../../../../../euclidean-norm.md) is [convex](../../../../../../convex-function.md) and $s\mapsto(2/3)s^{3/2}$ is increasing and [convex](../../../../../../convex-function.md) on $[0,\infty)$. It is [differentiable](../../../../../../differentiable-function.md), including at zero, and

$$
\boxed{\nabla\Phi(x)=T^\dagger(x)=\frac{x}{\sqrt{|x|}}\ (x\ne0),\qquad\nabla\Phi(0)=0.}
$$

Its graph [transport plan](../../../../../../transport-plan.md) lies in the graph of $\partial\Phi$, so the [Knott–Smith optimality criterion](../../../../../../knott-smith-optimality-criterion.md) proves quadratic optimality. Since that plan is induced by a map, part 1(b) proves optimality for the [Monge optimal transport problem](../../../../../../monge-optimal-transport-problem.md) as well. The minimum provides a useful independent check:

$$
\boxed{\min\mathbb M=\int_0^1(r-\sqrt r)^2\,2r\,dr
=\frac12-\frac87+\frac23=\frac1{42}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
