<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

With $y=xv$, direct differentiation gives

$$
x^2y''-2xy'+(x^2+2)y=x^3(v''+v).
$$

The homogeneous [ordinary differential equation](../../../ordinary-differential-equation.md) therefore has general solution $y=x(A\cos x+B\sin x)$. Choose

$$
y_1(x)=x\cos x,\qquad y_2(x)=x\sin x,
$$

so $y_1(\pi/2)=0$ and $y_2(\pi)=0$. Their [Wronskian](../../../wronskian.md) in the convention $W=y_1y_2'-y_1'y_2$ is $W(x)=x^2$. There is no nonzero homogeneous solution satisfying both [boundary conditions](../../../boundary-condition.md), since the first forces $B=0$ and the second forces $A=0$.

For the operator as printed, whose leading coefficient is $x^2$, the [Green's function](../../../green-s-function-split.md) is

$$
\boxed{G(x,s)=\begin{cases}
\displaystyle\frac{x\cos x\sin s}{s^3},&\pi/2\leq x\leq s\leq\pi,\\
\displaystyle\frac{x\sin x\cos s}{s^3},&\pi/2\leq s\leq x\leq\pi.
\end{cases}}
$$

It satisfies the endpoint [boundary conditions](../../../boundary-condition.md), is continuous across $x=s$, and its first derivative has jump $1/s^2$. Multiplying that jump by the leading coefficient $s^2$ produces the unit source required by a [Green's function](../../../green-s-function-split.md). This factor matters because the operator was not normalized to leading coefficient one; it is an instance of a [Green function under dependent-variable rescaling](../../../green-function-under-dependent-variable-rescaling.md).

Thus $y(x)=\int_{\pi/2}^\pi G(x,s)f(s)\,ds$. For $f(s)=s^3$, split the integral at $s=x$ to obtain

$$
\begin{aligned}
y(x)&=x\sin x\int_{\pi/2}^x\cos s\,ds+x\cos x\int_x^\pi\sin s\,ds\\
&=x\sin x(\sin x-1)+x\cos x(1+\cos x).
\end{aligned}
$$

Therefore

$$
\boxed{y(x)=x(1+\cos x-\sin x).}
$$

The substitution above gives $v''+v=1$, so the forcing is indeed $x^3$, and both endpoint values vanish.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2011](../../2011-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
