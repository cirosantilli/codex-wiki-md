<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

An [exact differential](../../../exact-differential.md) $M\,dx+N\,dy$ is $d\Phi$ for a scalar [potential function](../../../potential-function.md) $\Phi$, so $M=\partial\Phi/\partial x$ and $N=\partial\Phi/\partial y$. Equality $\partial M/\partial y=\partial N/\partial x$ is necessary, and is sufficient on a [simply connected space](../../../simply-connected-space.md) when these [partial derivatives](../../../partial-derivative.md) are continuous.

Here, after multiplying the [ordinary differential equation](../../../ordinary-differential-equation.md) by $dx$,

$$
M=x+\frac{2x}{y^2},\qquad N=6y-\frac{2x^2}{y^3},\qquad
\frac{\partial M}{\partial y}=-\frac{4x}{y^3}=\frac{\partial N}{\partial x}.
$$

On either half-plane $y>0$ or $y<0$, integrate $M$ with respect to $x$:

$$
\Phi=\frac{x^2}{2}+\frac{x^2}{y^2}+h(y).
$$

Comparison of $\partial\Phi/\partial y$ with $N$ gives $h'(y)=6y$, hence $h(y)=3y^2$ up to a constant. The solution is therefore the family of [level sets](../../../level-set.md)

$$
\boxed{\frac{x^2}{2}+\frac{x^2}{y^2}+3y^2=C,\qquad y\ne0.}
$$

Locally these define differentiable graphs $y(x)$ wherever $N\ne0$, by the [implicit function theorem](../../../implicit-function-theorem.md). When $N=0$, $M\ne0$ on this domain, so a finite derivative cannot satisfy $M+Ny'=0$ there; such points are [vertical tangents](../../../vertical-tangent.md) of the implicit curves, rather than additional classical graph solutions.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2021 resit](../../2021-resit-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
