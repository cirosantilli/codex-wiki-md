<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

On an interval where $p,q$ are continuous, define the [Wronskian](../../../../../wronskian.md)

$$
W[u_1,u_2]=\det\begin{pmatrix}u_1&u_2\\u_1'&u_2'\end{pmatrix}
=u_1u_2'-u_1'u_2.
$$

Using the two [second-order linear differential equations](../../../../../second-order-linear-differential-equation.md) to eliminate the second derivatives gives

$$
W'=u_1u_2''-u_1''u_2=-pW.
$$

The [integrating factor](../../../../../integrating-factor.md) yields the [Abel identity](../../../../../abel-s-identity.md)

$$
\boxed{W(x)=W(x_0)\exp\left(-\int_{x_0}^x p(s)\,ds\right).}
$$

Thus the [Wronskian](../../../../../wronskian.md) either vanishes identically or is nonzero everywhere on the interval. If $u_1,u_2$ are [linearly dependent](../../../../../linear-dependence.md), it is identically zero. Conversely, if $W(x_0)=0$, the two initial-data vectors are dependent, so some nontrivial linear combination has both value and first derivative zero at $x_0$. The [uniqueness theorem for ordinary differential equations](../../../../../uniqueness-theorem-for-ordinary-differential-equations.md) makes that combination identically zero. Hence **the solutions are linearly independent exactly when their Wronskian is nonzero at one, and therefore every, point**. Continuity and the common differential equation are essential to this converse.

For the particular equation, divide by $x^2$ on either interval $x>0$ or $x<0$. The coefficient of $y'$ is zero, so its [Wronskian](../../../../../wronskian.md) is constant there. The proposed $y_1=x^2$ satisfies $x^2y_1''-2y_1=2x^2-2x^2=0$. To construct a second solution by [reduction of order](../../../../../reduction-of-order.md), impose

$$
x^2y_2'-2xy_2=C\ne0.
$$

Dividing by $x^4$ shows that $(y_2/x^2)'=C/x^4$, giving

$$
y_2=Dx^2-\frac{C}{3x}.
$$

Taking $C=-3,D=0$ produces

$$
\boxed{y_2(x)=x^{-1},\qquad W[x^2,x^{-1}]=-3.}
$$

The nonzero [Wronskian](../../../../../wronskian.md) proves [linear independence](../../../../../linear-independence.md); hence the [general solution](../../../../../general-solution.md) on either nonsingular interval is $y=Ax^2+B/x$. Zero is a [singular point of a differential equation](../../../../../singular-point-of-a-differential-equation.md) and is excluded from this construction.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
