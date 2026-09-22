<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For $y=\alpha x+\beta x^2$, the derivatives are $y'=\alpha+2\beta x$ and $y''=2\beta$. Substituting gives $2\beta x^2-2x(\alpha+2\beta x)+2(\alpha x+\beta x^2)=0$. The independent solutions $x,x^2$ have [Wronskian](../../../wronskian.md) $x^2\neq0$ on $[1,2]$, so they form a [fundamental system of solutions](../../../fundamental-system-of-solutions.md).

Divide the [inhomogeneous linear differential equation](../../../inhomogeneous-linear-differential-equation.md) by $x^2$ and use [variation of parameters](../../../variation-of-parameters.md). Choosing integrals from one gives the particular solution

$$
z_p(x)=-x\int_1^x\frac{f(t)}{t^2}dt
+x^2\int_1^x\frac{f(t)}{t^3}dt.
$$

Thus $z=Ax+Bx^2+z_p$. The first [boundary condition](../../../boundary-condition.md) gives $A=-B$. The integral endpoint terms cancel when differentiating $z_p$, so the second gives

$$
0=3B-\int_1^2\frac{f(t)}{t^2}dt
+4\int_1^2\frac{f(t)}{t^3}dt.
$$

Consequently

$$
z(x)=\frac{x^2-x}{3}\int_1^2
\left(\frac1{t^2}-\frac4{t^3}\right)f(t)dt
-x\int_1^x\frac{f(t)}{t^2}dt
+x^2\int_1^x\frac{f(t)}{t^3}dt.
$$

Collect the coefficient of $f(t)$ on either side of $t=x$. A suitable [Green function](../../../green-s-function-split.md) is

$$
\boxed{G(x,t)=\frac1{3t^3}
\begin{cases}
(x^2-x)(t-4),&x\leq t,\\
(t-1)(x^2-4x),&t\leq x.
\end{cases}}
$$

The two pieces agree at $x=t$, $G(1,t)=0$, and $G_x(2,t)=0$ for $t<2$. For an interior source point its derivative jump is

$$
G_x(t+,t)-G_x(t-,t)=\frac1{t^2}.
$$

Thus multiplication by the leading coefficient $t^2$ gives [unit in a ring](../../../unit-in-a-ring.md) source strength. Away from $x=t$, both pieces solve the [homogeneous linear differential equation](../../../homogeneous-linear-differential-equation.md). With continuous $f$, the integral representation has the required second derivative and solves the equation pointwise in $(1,2)$.

For uniqueness, the difference of two solutions is $Ax+Bx^2$. Its [boundary conditions](../../../boundary-condition.md) give $A+B=0$ and $A+4B=0$, forcing $A=B=0$. Hence **the solution is unique**. This is the [mixed Green function for an Euler operator with exponents one and two](../../../mixed-green-function-for-an-euler-operator-with-exponents-one-and-two.md).

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
