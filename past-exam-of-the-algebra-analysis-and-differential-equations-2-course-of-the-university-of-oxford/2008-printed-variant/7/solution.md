<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Differentiate the [Wronskian](../../../wronskian.md):

$$
w'=uv''-u''v=u(-qv)-(-qu)v=0.
$$

It is therefore constant. [Linear dependence](../../../linear-dependence.md) plainly makes it zero. Conversely, if it is zero, the two initial-data vectors $(u(0),u'(0))$ and $(v(0),v'(0))$ are linearly dependent. Some constants $A,B$, not both zero, make $Au+Bv$ and its [derivative](../../../derivative.md) zero at zero. Uniqueness for a linear second-order equation with [continuous](../../../continuous-function.md) [coefficients](../../../coefficient.md) then makes $Au+Bv$ identically zero. Thus $\boxed{w=0\iff u,v\text{ are linearly dependent}}$.

For the prescribed integral put $K(x,s)=[u(x)v(s)-u(s)v(x)]/w$. Then $K(x,x)=0$, $K_x(x,x)=-1$, and $K_{xx}(x,s)=-q(x)K(x,s)$. [Differentiation](../../../differentiation.md) under the integral, using [continuity](../../../continuous-function.md) of the [coefficients](../../../coefficient.md) and forcing, gives

$$
y'(x)=\int_0^xK_x(x,s)f(s)\,ds,\qquad y''(x)=-f(x)-q(x)y(x).
$$

This proves the required inhomogeneous equation, with the sign of the forcing as printed.

For the explicit forcing take $u=\cosh x$, $v=\sinh x$, so $w=1$ and $K(x,s)=-\sinh(x-s)$. Since $2/(e^s+e^{-s})=\operatorname{sech}s$, the integral is

$$
-\int_0^x\sinh(x-s)\operatorname{sech}s\,ds=-x\sinh x+\cosh x\log\cosh x.
$$

Indeed expand $\sinh(x-s)=\sinh x\cosh s-\cosh x\sinh s$ and integrate $1$ and $\tanh s$. Adding the entire homogeneous solution gives

$$
\boxed{y(x)=A\cosh x+B\sinh x+\cosh x\log\cosh x-x\sinh x,\quad A,B\in\mathbb R.}
$$

Finally multiply the other equation by $\sin x$ and integrate from zero to $\pi$. [Integration by parts](../../../integration-by-parts.md) gives

$$
\int_0^\pi(y''+y)\sin x\,dx=[y'\sin x-y\cos x]_0^\pi=y(\pi)+y(0)=0.
$$

Thus $\boxed{\int_0^\pi f(s)\sin s\,ds=0}$ is necessary. It is also sufficient: the solution with $y(0)=0$ is $B\sin x-\int_0^x\sin(x-s)f(s)\,ds$, and the integral condition gives its value zero at $\pi$.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2008 printed variant](../../2008-printed-variant-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
