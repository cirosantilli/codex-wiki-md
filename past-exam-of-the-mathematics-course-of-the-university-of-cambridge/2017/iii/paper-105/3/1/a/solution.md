<h1 id="3/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The growth bound is $|F(t,x)|\le K(1+|x|)$. A [characteristic curve](../../../../../../../characteristic-curve.md) through $(s,a)$ solves

$$
\boxed{\dot X(t;s,a)=F(t,X(t;s,a)),\qquad X(s;s,a)=a.}
$$

The $C^1$ field is locally Lipschitz in space, giving local existence and uniqueness. On either direction of a bounded time interval the [Gronwall inequality](../../../../../../../gronwall-inequality.md) gives $1+|X(t;s,a)|\le(1+|a|)e^{K|t-s|}$. Thus no trajectory can escape to infinity at finite time. On the resulting compact space-time region, local [ordinary differential equation](../../../../../../../ordinary-differential-equation.md) existence continues it, proving global definition for all $t\in\mathbb R$.

Uniqueness gives the flow composition law and inverse $X(s;t,\cdot)$. Differentiation with respect to $a$ solves the variational equation, making each map a $C^1$ [diffeomorphism](../../../../../../../diffeomorphism.md). Its positive [Jacobian determinant](../../../../../../../jacobian-determinant.md) is

$$
J(t;s,a)=\exp\left(\int_s^t\operatorname{div}F(\tau,X(\tau;s,a))\,d\tau\right).
$$

These facts constitute the [global characteristic flow under linear growth](../../../../../../../global-characteristic-flow-under-linear-growth.md). A uniform global bound on $D_xF$ is not required; its bounds on each compact characteristic tube suffice.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
