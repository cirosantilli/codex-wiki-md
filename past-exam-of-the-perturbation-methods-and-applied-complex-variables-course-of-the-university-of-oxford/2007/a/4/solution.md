<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

On the two independent variables, the total [derivative](../../../../derivative.md) is $D_x=\partial_x+\epsilon^{-1}\partial_X$. Multiplication of $D_x(aD_xy)=f$ by $\epsilon^2$ gives exactly the stated multiple-scale equation.

At order one, $\partial_X(a\,\partial_Xy_0)=0$. Integrating twice gives

$$
y_0=B(x)+A(x)\int^X\frac{dS}{a(x,S)}.
$$

The periodic reciprocal coefficient has strictly positive mean. Unless $A=0$, the [integral](../../../../integral-split.md) has a nonzero linear drift in $X$, violating the periodic cell ansatz and creating secular growth when $X=x/\epsilon$. Thus $A=0$ and $y_0=y_0(x)$.

At order $\epsilon$,

$$
\partial_X\{a(y_{1X}+y_0')\}=0,\qquad
y_{1X}=\frac{C(x)}{a(x,X)}-y_0'.
$$

Periodicity requires the [derivative](../../../../derivative.md) to have zero cell average. Consequently

$$
0=C(x)\int_0^1a^{-1}(x,X)dX-y_0',
\qquad C(x)=\hat a(x)y_0'(x).
$$

At order $\epsilon^2$, the equation is

$$
\partial_X\{a(y_{2X}+y_{1x})\}
+\partial_x\{a(y_{1X}+y_0')\}=f(x,X).
$$

The second flux inside braces is $C(x)$, independent of $X$. Integrating over one [period](../../../../period-of-a-function.md) annihilates the first [derivative](../../../../derivative.md), by periodicity, and yields $C'(x)=\int_0^1f(x,X)dX$. Hence

$$
\boxed{\frac d{dx}\bigl(\hat a(x)y_0'(x)\bigr)=\hat f(x),\quad
\hat a(x)=\left(\int_0^1a(x,X)^{-1}dX\right)^{-1},\quad
\hat f(x)=\int_0^1f(x,X)dX.}
$$

The effective transport coefficient is the [harmonic mean](../../../../harmonic-mean.md) of $a$ over the fast [period](../../../../period-of-a-function.md); the source is averaged arithmetically. Smoothness sufficient for these formal differentiations and uniform positivity on the cells are understood.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../split.md)
5. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
