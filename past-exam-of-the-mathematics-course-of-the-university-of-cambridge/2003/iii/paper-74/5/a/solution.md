<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The positive drift places the [boundary layer](../../../../../../boundary-layer.md) at the left endpoint. Set $y_{\rm out}=y_0+\epsilon y_1+\cdots$ and impose the right [boundary condition](../../../../../../boundary-condition.md) order by order. The leading [ordinary differential equation](../../../../../../ordinary-differential-equation.md) is $[(1+x)y_0]'=0$, so $y_0=2/(1+x)$. At the next order,

$$
[(1+x)y_1]'=-y_0''=-\frac4{(1+x)^3},\qquad y_1(1)=0,
$$

which integrates to

$$
\boxed{y_{\rm out}=\frac2{1+x}+\epsilon\left[\frac2{(1+x)^3}-\frac1{2(1+x)}\right]+O(\epsilon^2)}.
$$

The outer limit at the left endpoint is two, so it cannot satisfy the left boundary value without a rapidly varying correction.

For the inner expansion use $X=x/\epsilon$ and $y=Y_0(X)+\epsilon Y_1(X)+\cdots$. Its equations and boundary values are

$$
Y_0''+Y_0'=0,\qquad Y_0(0)=1,
$$



$$
Y_1''+Y_1'=-(XY_0'+Y_0),\qquad Y_1(0)=0.
$$

Matching the leading constant gives $Y_0=2-e^{-X}$. The first-order forcing is then $-2+(1-X)e^{-X}$. A particular solution is $-2X+\tfrac12X^2e^{-X}$, and matching determines the constant to be $3/2$. Enforcing $Y_1(0)=0$ gives

$$
\boxed{y_{\rm in}=2-e^{-X}+\epsilon\left[\frac32-2X+\left(\frac{X^2}{2}-\frac32\right)e^{-X}\right]+O(\epsilon^2)}.
$$

In the overlap region the common expansion is $2+\epsilon(3/2-2X)$. Adding the inner and outer approximations and subtracting that common part gives the [uniform asymptotic approximation](../../../../../../uniform-asymptotic-approximation.md)

$$
\boxed{y_{\rm comp}(x)=\frac2{1+x}+\epsilon\left[\frac2{(1+x)^3}-\frac1{2(1+x)}\right]
-e^{-x/\epsilon}+\epsilon\left(\frac{x^2}{2\epsilon^2}-\frac32\right)e^{-x/\epsilon}}.
$$

It has error $O(\epsilon^2)$ uniformly for $0\le x\le1$, apart from an exponentially small endpoint adjustment of the same asymptotic irrelevance. At $x=0$ it equals one exactly, and at $x=1$ it differs from one only exponentially. The polynomial multiplying the exponential remains bounded on the inner scale.

There is an independent check from a first integral. The equation is $[\epsilon y'+(1+x)y]'=0$, so its exact solution has the form

$$
y(x)=e^{-(x+x^2/2)/\epsilon}\left[1+\frac C\epsilon\int_0^x e^{(s+s^2/2)/\epsilon}\,ds\right],
$$

where $C$ is selected by the right boundary value. Endpoint expansion of this integral gives $C=2-\epsilon/2+O(\epsilon^2)$, the same outer coefficients and the same inner expansion. This check also establishes the uniform order of the composite approximation without treating an inner residual as an outer estimate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
