<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $f(x,y)=y$ and $\beta=1/2$, the [explicit midpoint method](../../../../explicit-midpoint-method.md) multiplies the current value by $R=1+h+h^2/2$. Starting from one, induction gives

$$
\boxed{y_n=\left(1+h+\frac{h^2}{2}\right)^n.}
$$

Let $A=e^h$ and $B=R$. The [Taylor theorem with Lagrange remainder](../../../../taylor-theorem-with-lagrange-remainder.md) for the [exponential function](../../../../exponential-function.md) gives

$$
\frac{h^3}{6}\leq A-B\leq\frac{h^3e^h}{6},\qquad 1\leq B\leq A.
$$

The [difference of powers](../../../../difference-of-powers.md) identity gives $A^n-B^n=(A-B)\sum_{k=0}^{n-1}A^{n-1-k}B^k$. Every summand lies between one and $A^{n-1}$. Since $nh=x_n$, the [global error](../../../../global-discretization-error.md) therefore satisfies

$$
\boxed{\frac{h^2x_n}{6}\leq y(x_n)-y_n\leq\frac{h^2x_ne^{x_n}}6.}
$$

The same inequalities hold at $n=0$, where the error vanishes. At the fixed endpoint $x_N=1$, the lower bound $h^2/6$ prevents any higher [order of a numerical method](../../../../order-of-a-numerical-method.md), while the upper bound is $eh^2/6$. Thus **the convergence order is exactly two**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../../numerical-linear-algebra-and-numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
6. [MSc in mathematical modelling and scientific computing course of the University of Oxford](../../../../msc-in-mathematical-modelling-and-scientific-computing-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
