<h1 id="8c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For real initial data, [separation of variables](../../../../../../separation-of-variables.md) gives

$$
\boxed{z(t)=\frac{z_0}{1-z_0t}.}
$$

This includes $z_0=0$, whose solution is identically zero. Every other real $z_0$ has a pole at $t=1/z_0$, so only $z_0=0$ gives a finite solution on the whole real line. If complex-valued initial data are allowed, a nonreal $z_0$ has no real-time pole; the whole-real-line conclusion here uses the usual real-valued differential-equation convention.

Along a [characteristic curve](../../../../../../characteristic-curve.md) $y=u+ax$, the [chain rule](../../../../../../chain-rule.md) gives $d f(x,u+ax)/dx=f_x+af_y$. For the homogeneous [transport equation](../../../../../../transport-equation.md) this is zero, so $f(x,y)=F(y-ax)$. For the nonlinear equation, the same [method of characteristics](../../../../../../method-of-characteristics.md) reduces the problem to $d f/dx=f^2$, with initial value $g(u)$. Therefore

$$
\boxed{f(x,y)=\frac{g(y-ax)}{1-xg(y-ax)}.}
$$

For [differentiable](../../../../../../differentiable-function.md) real $g$, this is the classical solution wherever its denominator is nonzero, on the characteristic intervals containing the initial line. If $g(u)\ne0$ for some $u$, that characteristic blows up at $x=1/g(u)$, $y=u+a/g(u)$. Thus **the only real-valued solution bounded on all of $\mathbb R^2$ has $g\equiv0$, giving $f\equiv0$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8C](../../8c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
