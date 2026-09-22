<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [characteristic curves](../../../../../characteristic-curve.md) satisfy

$$
-x^2(dy)^2+(dx)^2=0,\qquad\frac{dy}{dx}=\pm\frac1x.
$$

Integrating suggests the [characteristic coordinates](../../../../../characteristic-coordinate.md)

$$
\boxed{\xi=y+\ln|x|,\qquad\eta=y-\ln|x|.}
$$

Their [Jacobian determinant](../../../../../jacobian-determinant.md) is $2/x$, so this is an invertible local [change of variables](../../../../../change-of-variables-formula.md) whenever $x\ne0$. Write $u(x,y)=U(\xi,\eta)$. The [chain rule](../../../../../chain-rule.md) gives

$$
\begin{aligned}
u_x&=\frac{U_\xi-U_\eta}{x},\\
x^2u_{xx}&=U_{\xi\xi}-2U_{\xi\eta}+U_{\eta\eta}-U_\xi+U_\eta,\\
u_{yy}&=U_{\xi\xi}+2U_{\xi\eta}+U_{\eta\eta}.
\end{aligned}
$$

Substitution cancels both unmixed second derivatives and both first derivatives:

$$
-x^2u_{xx}+u_{yy}-xu_x=4U_{\xi\eta}.
$$

The [canonical form of a second-order partial differential equation](../../../../../canonical-form-of-a-second-order-partial-differential-equation.md) is therefore

$$
\boxed{U_{\xi\eta}=1.}
$$

The cancellation of the first derivatives is the key feature of these [logarithmic characteristic coordinates](../../../../../logarithmic-characteristic-coordinates.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
