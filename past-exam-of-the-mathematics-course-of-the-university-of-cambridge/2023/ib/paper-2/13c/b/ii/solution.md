<h1 id="13c/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrating the [ordinary differential equation](../../../../../../../ordinary-differential-equation.md) four times gives a quartic [polynomial](../../../../../../../polynomial-split.md). It is useful to use the [linearity](../../../../../../../linearity.md) of the equation and split the solution into a gravity part and a force part:

$$
y=y_0+y_F,
$$

where

$$
y_0(x)
=-\frac{\rho g}{24A}x^2(6L^2-4Lx+x^2)
$$

satisfies the clamped and torque-free [boundary conditions](../../../../../../../boundary-condition.md) with $F=0$, while

$$
y_F(x)=\frac{F}{6A}x^2(3L-x)
$$

satisfies the homogeneous equation and contributes the endpoint [force](../../../../../../../force.md). Direct [differentiation](../../../../../../../differentiation.md) verifies

$$
y(0)=y'(0)=0,\qquad y''(L)=0,\qquad -Ay'''(L)=F.
$$

Thus

$$
\boxed{
y(x)=-\frac{\rho g}{24A}x^2(6L^2-4Lx+x^2)
+\frac{F}{6A}x^2(3L-x)
},
$$

the [clamped-free beam under uniform load and endpoint force](../../../../../../../clamped-free-beam-under-uniform-load-and-endpoint-force.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [13C](../../../13c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
