<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

For a second-order [linear partial differential equation](../../../linear-partial-differential-equation.md) with principal part $Au_{xx}+2Bu_{xy}+Cu_{yy}$, the discriminant is $B^2-AC$. Here $A=1$, $B=0$, $C=-x^2$, so

$$
\boxed{B^2-AC=x^2>0\quad(x>0).}
$$

The equation is therefore a [hyperbolic partial differential equation](../../../hyperbolic-partial-differential-equation.md) throughout its domain. The lower-order term $-u_x/x$ does not affect this classification.

The [characteristic curves](../../../characteristic-curve.md) satisfy

$$
A(dy)^2-2B\,dx\,dy+C(dx)^2=0,
\qquad \frac{dy}{dx}=\pm x.
$$

Integrating gives the two families $y\mp x^2/2=\text{constant}$. Choose coordinates constant along these families:

$$
\xi=x^2-2y,\qquad\eta=x^2+2y.
$$

Their [Jacobian determinant](../../../jacobian-determinant.md) is $8x\ne0$, so they define an invertible [change of variables](../../../change-of-variables-formula.md) on $x>0$, with image $\xi+\eta>0$. Write $u(x,y)=U(\xi,\eta)$. The [chain rule](../../../chain-rule.md) gives

$$
\begin{aligned}
u_x&=2x(U_\xi+U_\eta),\\
u_{xx}&=2(U_\xi+U_\eta)+4x^2(U_{\xi\xi}+2U_{\xi\eta}+U_{\eta\eta}),\\
u_{yy}&=4(U_{\xi\xi}-2U_{\xi\eta}+U_{\eta\eta}).
\end{aligned}
$$

Both the pure second [partial derivatives](../../../partial-derivative.md) and the first [partial derivatives](../../../partial-derivative.md) cancel in the original equation, leaving

$$
16x^2U_{\xi\eta}=0,\qquad\boxed{U_{\xi\eta}=0.}
$$

This is the full [canonical form of a second-order partial differential equation](../../../canonical-form-of-a-second-order-partial-differential-equation.md), including the effect of the lower-order term. Integrating shows $U_\xi$ is a function of $\xi$ alone, hence

$$
\boxed{u(x,y)=f(x^2-2y)+g(x^2+2y),}
$$

with arbitrary twice [differentiable functions](../../../differentiable-function.md) $f,g$. The representation is global on $x>0$: for each fixed $\xi$, the allowed $\eta>-\xi$ form an interval, so $U_\xi$ is independent of $\eta$ throughout that interval; after subtracting its antiderivative, the same reasoning in the other coordinate leaves only $g(\eta)$. These are [quadratic characteristic coordinates for a variable-speed wave equation](../../../quadratic-characteristic-coordinates-for-a-variable-speed-wave-equation.md).

For the data on $x=1$, set $s=1-2y$, so the other argument is $2-s$. The two [initial conditions](../../../initial-condition.md) become

$$
f(s)+g(2-s)=1,\qquad 2\bigl(f'(s)+g'(2-s)\bigr)=2.
$$

Differentiating the first equation with respect to $s$ also gives $f'(s)-g'(2-s)=0$. Solving these two linear equations yields $f'(s)=g'(2-s)=1/2$. Since $s$ ranges over all real numbers,

$$
f(s)=\frac{s}{2}+C,\qquad g(t)=\frac{t}{2}-C.
$$

Consequently

$$
\boxed{u(x,y)=x^2.}
$$

Indeed $u_{xx}=2$, $u_{yy}=0$, $u_x=2x$, so the equation and both [initial conditions](../../../initial-condition.md) hold directly.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2012](../../2012-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
