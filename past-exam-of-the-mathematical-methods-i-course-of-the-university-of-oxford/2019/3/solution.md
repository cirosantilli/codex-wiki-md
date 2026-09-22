<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The right-hand side depends on $x+y$, suggesting the substitution $u=x+y$. Then $y'=u'-1$, so the [ordinary differential equation](../../../ordinary-differential-equation.md) becomes

$$
u'=2-\frac4u=\frac{2(u-2)}u.
$$

The original equation is undefined at $u=0$. If $u\ne2$, this is a [separable differential equation](../../../separable-differential-equation.md):

$$
\frac{u}{u-2}\,du=2\,dx,\qquad
u+2\ln|u-2|=2x+C.
$$

Substituting back gives the implicit family

$$
\boxed{y-x+2\ln|x+y-2|=C,\qquad x+y\ne0,2.}
$$

Differentiating the implicit equation gives $y'-1+2(1+y')/(x+y-2)=0$, or $(x+y)y'=x+y-4$, verifying it on its permitted intervals.

Division by $u-2$ excluded the constant solution $u=2$, which must be restored separately:

$$
\boxed{y=2-x.}
$$

It satisfies $y'=-1=(2-4)/2$. Together these give all local real solutions on intervals where $x+y\ne0$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2019](../../2019-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
