<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

Substituting $y=x^p$ in the homogeneous [ordinary differential equation](../../../../../ordinary-differential-equation.md) gives $p(p-1)-2=(p-2)(p+1)=0$. Thus

$$
\boxed{y_h=Cx^2+D/x}.
$$

For a [Green's function](../../../../../green-s-function.md) decaying at the two ends, use $u(x)=x^2$ on the side of zero and $v(x)=x^{-1}$ on the side of infinity. Their [Wronskian](../../../../../wronskian.md) is $uv'-u'v=-3$. The [function](../../../../../function-split.md) must be continuous at $x=\xi$, or its second [derivative](../../../../../derivative.md) would contain a [derivative](../../../../../derivative.md) of a [Dirac delta](../../../../../dirac-delta-function.md). Its [derivative](../../../../../derivative.md) jump must be one, to give the specified positive delta source. These two conditions yield the [boundary-decaying Green kernel for an inverse-square differential operator](../../../../../boundary-decaying-green-kernel-for-an-inverse-square-differential-operator.md):

$$
\boxed{G(x,\xi)=-\frac13\begin{cases}x^2/\xi,&x\leq\xi,\\\xi^2/x,&x\geq\xi.\end{cases}}
$$

Its [derivatives](../../../../../derivative.md) at the join are $-2/3$ on the left and $1/3$ on the right, confirming the jump one. Away from the join each branch solves the homogeneous equation, and both endpoint conditions hold.

Integrate this [Green's function](../../../../../green-s-function.md) against the forcing, whose support is between zero and one. For $0<x\leq1$,

$$
y(x)=-\frac13\left(\frac1x\int_0^x\xi^2\,d\xi+x^2\int_x^1\frac{d\xi}{\xi}\right)=\frac{x^2}{3}\log x-\frac{x^2}{9}.
$$

For $x\geq1$, only the right branch contributes. Therefore

$$
\boxed{y(x)=\begin{cases}\dfrac{x^2}{3}\log x-\dfrac{x^2}{9},&0<x\leq1,\\-\dfrac1{9x},&x\geq1.\end{cases}}
$$

On the first branch, $y'=(2x/3)\log x+x/9$ and $y''=(2/3)\log x+7/9$, so $y''-2y/x^2=1$. The second branch is a multiple of the homogeneous solution $x^{-1}$, so its forcing is zero. At $x=1$, both $y$ and $y'$ agree, with values $-1/9$ and $1/9$, so there is no additional delta source. Finally $x^2\log x\to0$ as $x\downarrow0$ and $x^{-1}\to0$ as $x\to\infty$. A homogeneous solution obeying both [boundary conditions](../../../../../boundary-condition.md) has $C=D=0$, establishing uniqueness.

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
