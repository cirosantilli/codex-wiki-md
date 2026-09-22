<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

With $\eta=x-t$ and $\xi=x+t$, the [chain rule](../../../../../chain-rule.md) gives

$$
\partial_x=\partial_\eta+\partial_\xi,
\qquad
\partial_t=-\partial_\eta+\partial_\xi.
$$

Hence

$$
u_{xx}-u_{tt}=4U_{\eta\xi},
$$

so the [wave equation](../../../../../wave-equation-split.md) is equivalent to $U_{\eta\xi}=0$. Integrating in each variable gives

$$
u(x,t)=F(x-t)+G(x+t).
$$

The initial conditions imply

$$
F(x)+G(x)=f(x),
\qquad
-F'(x)+G'(x)=g(x).
$$

Solving and integrating yields the [D'Alembert formula with initial velocity](../../../../../d-alembert-formula-with-initial-velocity.md)

$$
\boxed{
u(x,t)=\frac12[f(x-t)+f(x+t)]
+\frac12\int_{x-t}^{x+t}g(y)\,dy}.
$$

If $|x-x_0|>r+t$, then both $x-t$ and $x+t$ lie outside the support interval $[x_0-r,x_0+r]$, and every point between them does as well. All three terms therefore vanish. Thus

$$
\boxed{u(x,t)=0\quad\text{when }|x-x_0|>r+t},
$$

which is finite propagation speed.

For the finite string, differentiate its energy and use $y_{tt}=y_{xx}$:

$$
\begin{aligned}
\frac{dE}{dt}
&=\int_0^L(y_xy_{xt}+y_ty_{tt})\,dx\\
&=\int_0^L(y_xy_{xt}+y_ty_{xx})\,dx\\
&=[y_ty_x]_0^L.
\end{aligned}
$$

The fixed-end conditions hold for every $t$, so differentiation gives $y_t(0,t)=y_t(L,t)=0$. The boundary term vanishes and

$$
\boxed{E(t)=E(0)}.
$$

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
