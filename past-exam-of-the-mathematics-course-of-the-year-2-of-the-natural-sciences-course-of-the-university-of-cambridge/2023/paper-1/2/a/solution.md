<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [separation of variables](../../../../../separation-of-variables.md), $u=X(x)Y(y)$, and divide by $XY$ where nonzero. A real separation constant $\kappa$ gives

$$
\frac{X''}{X}=\frac{Y'}Y+1+\sin y=\kappa,
$$

so $X''=\kappa X$ and $Y'=(\kappa-1-\sin y)Y$. Normalizing the second factor to one at zero gives

$$
\boxed{Y_\kappa(y)=\exp[(\kappa-1)y+\cos y-1].}
$$

The spatial [ordinary differential equation](../../../../../ordinary-differential-equation.md) has three types of real solution:

$$
\boxed{X(x)=\begin{cases}A\cos(kx)+B\sin(kx),&\kappa=-k^2<0,\\A+Bx,&\kappa=0,\\A\cosh(kx)+B\sinh(kx),&\kappa=k^2>0.\end{cases}}
$$

Products $X Y_\kappa$ are the separated [eigenfunctions](../../../../../eigenfunction.md). The negative, zero and positive separation constants give trigonometric, linear and [hyperbolic function](../../../../../hyperbolic-function.md) forms respectively. There is no discrete quantization until [boundary conditions](../../../../../boundary-condition.md) on $x$ are supplied. Since $\cos y-1$ is bounded, the envelope of $Y_\kappa$ decays for $\kappa<1$, grows for $\kappa>1$, and is bounded and periodic for $\kappa=1$. The scalar prefactor can also be derived by [removing a variable scalar reaction rate by an integrating factor](../../../../../removing-a-variable-scalar-reaction-rate-by-an-integrating-factor.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
