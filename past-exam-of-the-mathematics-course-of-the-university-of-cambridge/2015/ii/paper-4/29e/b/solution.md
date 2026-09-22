<h1 id="29e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $v=e^{t/2}u$. The cancellation of the damping and mass terms gives $v_{tt}=v_{xx}$, with $v(x,0)=u_0(x)$ and $v_t(x,0)=u_1(x)+u_0(x)/2$. For the [wave equation](../../../../../../wave-equation-split.md), $w_+=v_t+v_x$ satisfies $(\partial_t-\partial_x)w_+=0$, and $w_-=v_t-v_x$ satisfies $(\partial_t+\partial_x)w_-=0$. Thus these combinations are transported on straight [characteristics](../../../../../../characteristic-of-a-field.md). Integrating them and matching the initial displacement yields the [D'Alembert formula](../../../../../../d-alembert-s-formula.md), and hence

$$
\boxed{u(x,t)=e^{-t/2}\left[\frac{u_0(x+t)+u_0(x-t)}2+\frac12\int_{x-t}^{x+t}\left(u_1(y)+\frac12u_0(y)\right)dy\right].}
$$

Here the initial functions are extended periodically to the real line. Direct differentiation verifies both initial conditions and the equation, and arbitrary repeated differentiation shows the solution is smooth and periodic.

This characteristic derivation also proves [finite propagation speed](../../../../../../finite-propagation-speed.md) from first principles: the value at $(x,t)$ depends only on the two endpoint displacements and initial velocity data in $[x-t,x+t]$. If two data sets agree on that interval, their solutions agree at that point. Equivalently initially supported data have no influence outside the unit-speed characteristic cone, interpreted on the periodic covering line. Multiplication by $e^{-t/2}$ does not enlarge this domain of dependence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29E](../../29e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
