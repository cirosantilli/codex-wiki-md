<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work first on $x>0$. For $b=0$, the [power-law ansatz](../../../../power-law-ansatz.md) $y=x^r$ gives the [indicial equation](../../../../indicial-equation.md) $r(r-1)+r-a^2=r^2-a^2=0$. Therefore the [Cauchy-Euler equation](../../../../cauchy-euler-equation.md) has [general solution](../../../../general-solution.md)

$$
\boxed{y(x)=
\begin{cases}
C_1x^a+C_2x^{-a},&a>0,\\
C_1+C_2\log x,&a=0.
\end{cases}}
$$

For $a=0$ the repeated [indicial root](../../../../indicial-root.md) supplies the [logarithm](../../../../logarithm.md) rather than two copies of the constant solution. Alternatively, the [change of variables](../../../../change-of-variables-formula.md) $t=\log x$ turns the [differential equation](../../../../differential-equation-split.md) into $Y''-a^2Y=0$. On $x<0$ the corresponding real formulas use $|x|$ and $\log|x|$, with independent constants on the two sides of zero.

For general $b$, normalize the [second-order linear differential equation](../../../../second-order-linear-differential-equation.md) as

$$
y''+P(x)y'+Q(x)y=0,\qquad P(x)=\frac1x,\qquad Q(x)=-\frac{a^2}{x^2}+bx^{\beta-2}.
$$

The coefficient $P$ is singular at zero, but $xP(x)=1$ and $x^2Q(x)=-a^2+bx^\beta$ are [analytic functions](../../../../holomorphic-function-split.md) there because $\beta$ is a positive integer. The [regular singular point criterion for a second-order equation](../../../../regular-singular-point-criterion-for-a-second-order-equation.md) therefore proves that zero is a [regular singular point](../../../../regular-singular-point.md) for every allowed $a,b,\beta$. The [indicial equation](../../../../indicial-equation.md) remains $r^2-a^2=0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
