<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [change of variables](../../../../../../change-of-variables-formula.md) $u=x+y$. Then $u'=1+y'=1+\cos u=2\cos^2(u/2)$, a [separable differential equation](../../../../../../separable-differential-equation.md). Where $u$ is not an odd multiple of $\pi$, [separation of variables](../../../../../../separation-of-variables.md) gives

$$
\int\frac{du}{1+\cos u}=\int dx,
\qquad
\boxed{\tan\frac{x+y}{2}=x+C.}
$$

Indeed the [derivative](../../../../../../derivative.md) of $\tan(u/2)$ with respect to $u$ is $1/(1+\cos u)$. The nonconstant branches can also be written $y=2\arctan(x+C)+2k\pi-x$, $k\in\mathbb Z$. Dividing by $1+\cos u$ excluded its zeros: the missing [equilibrium solutions](../../../../../../equilibrium-solution-of-an-ordinary-differential-equation.md) for $u$ give the additional [solutions of a differential equation](../../../../../../solution-of-a-differential-equation.md)

$$
\boxed{y=(2k+1)\pi-x,\qquad k\in\mathbb Z.}
$$

They satisfy $y'=-1=\cos(x+y)$ directly. The transformed right side is continuously differentiable, so the [uniqueness theorem for ordinary differential equations](../../../../../../uniqueness-theorem-for-ordinary-differential-equations.md) prevents a nonconstant branch from crossing an [equilibrium solution](../../../../../../equilibrium-solution-of-an-ordinary-differential-equation.md) at finite $x$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Mathematics III resit](../../../mathematics-iii-resit-split.md)
4. [Prelims](../../../split.md)
5. [Undated](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
