<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

Differentiating the [Wronskian](../../../../../wronskian.md) gives

$$
\begin{aligned}
W'
&=(y_1y_2'-y_2y_1')'\\
&=y_1y_2''-y_2y_1''\\
&=y_1(-py_2'-qy_2)-y_2(-py_1'-qy_1)\\
&=-pW.
\end{aligned}
$$

Thus $W'+pW=0$, the [Abel identity](../../../../../abel-s-identity.md).

Also,

$$
\left(\frac{y_2}{y_1}\right)'
=\frac{y_1y_2'-y_2y_1'}{y_1^2}
=\frac W{y_1^2}.
$$

If $y_2(x_0)=0$, integration gives the [reduction of order](../../../../../reduction-of-order.md) formula

$$
\boxed{
y_2(x)=y_1(x)\int_{x_0}^x\frac{W(t)}{y_1(t)^2}\,dt}.
$$

For the specified equation, division by $x^2$ gives $p(x)=-1/x$, so $W=Cx$. With $y_1=x^3$, an independent solution is

$$
x^3\int x^{-5}\,dx,
$$

which is a nonzero multiple of $x^{-1}$. Hence

$$
y=Ax^3+\frac Bx.
$$

The conditions at $x=1$ give $A+B=0$ and $3A-B=1$, so

$$
\boxed{y(x)=\frac14\left(x^3-\frac1x\right)}.
$$

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
