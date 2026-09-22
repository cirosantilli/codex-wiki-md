<h1 id="30a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Parameterize the initial line by $(s,2)$ and use characteristic time $\tau$. The [characteristic equations for a transport equation](../../../../../../characteristic-equations-for-a-transport-equation.md) integrate to

$$
x_1=se^{2\tau},\qquad x_2=2e^{4\tau},\qquad U=\frac{h}{1-h\tau},\qquad \tau<1/h.
$$

Here $dU/d\tau=U^2$ and $U(0)=h$. Since $\tau=\tfrac14\log(x_2/2)$, the solution is

$$
\boxed{u(x_1,x_2)=\frac{h}{1-\frac h4\log(x_2/2)},\qquad (x_1,x_2)\in\mathbb R\times(0,2e^{4/h}).}
$$

Direct differentiation gives $u_{x_1}=0$, $u_{x_2}=u^2/(4x_2)$, verifying the equation and the initial values. The map $(s,\tau)\mapsto(x_1,x_2)$ has determinant $8e^{6\tau}\ne0$, so every point of this strip is reached exactly once.

At the upper boundary $u\to+\infty$, a [finite-time blow-up of an ordinary differential equation](../../../../../../finite-time-blow-up-of-an-ordinary-differential-equation.md). At the lower boundary $u\to0$, but $u_{x_2}=u^2/(4x_2)$ diverges as $x_2\downarrow0$, so no $C^1$ continuation through that boundary is possible. Thus the displayed strip is the maximal connected domain containing the initial line on which this classical Cauchy solution exists.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30A](../../30a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
