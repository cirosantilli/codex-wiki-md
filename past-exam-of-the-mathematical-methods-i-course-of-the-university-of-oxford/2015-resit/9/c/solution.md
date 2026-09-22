<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $b\ne-1$ and initially $y\ne0$, use the [Bernoulli power substitution](../../../../bernoulli-power-substitution.md) $v=y^{b+1}$. The equation becomes

$$
v'-a(b+1)v=(b+1)e^{-2x}.
$$

Write $\kappa=a(b+1)$. A [first-order linear differential equation](../../../../first-order-linear-differential-equation.md) then gives

$$
\boxed{y^{b+1}=\begin{cases}Ce^{\kappa x}-\dfrac{b+1}{\kappa+2}e^{-2x},&\kappa\ne-2,\\e^{-2x}[C+(b+1)x],&\kappa=-2.\end{cases}}
$$

The second line is the resonant case of a [Bernoulli equation with exponential forcing](../../../../bernoulli-equation-with-exponential-forcing.md). Recover $y$ using real branches for which the original power $y^{-b}$ is defined; for example, unrestricted noninteger powers are unambiguous on $y>0$.

The exceptional exponent $b=-1$ makes the original equation linear: $y'=(a+e^{-2x})y$. Its solutions are

$$
\boxed{y=C\exp\left(ax-\frac12e^{-2x}\right).}
$$

Domain restrictions matter when the solution reaches zero. If $b<0$ and the real power at zero is defined, $y\equiv0$ is also a solution. For $-1<b<0$, [waiting-time solutions of a sublinear Bernoulli equation](../../../../waiting-time-solutions-of-a-sublinear-bernoulli-equation.md) may stay zero until an arbitrary $x_0$ and then become positive, with

$$
y^{b+1}=(b+1)e^{\kappa x}\int_{x_0}^{x}e^{-(\kappa+2)s}\,ds\quad(x>x_0),\qquad y=0\quad(x\le x_0).
$$

The joining derivative is zero because $1/(b+1)>1$. For $b=0$, the linear formula can pass through zero normally; for $b>0$, the original negative power excludes zero. These qualifications prevent dividing out a valid zero solution or inventing one where the equation is undefined.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
