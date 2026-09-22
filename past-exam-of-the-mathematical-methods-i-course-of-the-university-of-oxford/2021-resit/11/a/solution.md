<h1 id="11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On an interval with $x\ne0$, this is a [homogeneous first-order differential equation](../../../../homogeneous-first-order-differential-equation.md). Put $y=xv(x)$, so $y'=v+xv'$. Substitution and division by $x^2$ give

$$
xv'=v^2-2v=v(v-2).
$$

The constant choices $v=0$ and $v=2$ give $y=0$ and $y=2x$. Otherwise the [separable differential equation](../../../../separable-differential-equation.md) gives

$$
\int\frac{dv}{v(v-2)}=\int\frac{dx}{x},\qquad
\frac12\ln\left|\frac{v-2}{v}\right|=\ln|x|+C_0.
$$

Absorbing the sign and the exponential integration constant yields $(v-2)/v=Cx^2$. Relabelling the arbitrary constant then gives

$$
\boxed{y(x)=\frac{2x}{1+Kx^2},\qquad\text{or}\qquad y(x)=0.}
$$

The first family already includes $y=2x$ at $K=0$. Choose any interval where its denominator is nonzero. These give all solutions on intervals avoiding $x=0$. Both families extend through $x=0$ with $y(0)=0$, as required by the original [ordinary differential equation](../../../../ordinary-differential-equation.md). Because it is singular there, differentiable continuations of the nonzero family may use different $K$ on the two sides: both one-sided derivatives at zero equal $2$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [11](../../11.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
