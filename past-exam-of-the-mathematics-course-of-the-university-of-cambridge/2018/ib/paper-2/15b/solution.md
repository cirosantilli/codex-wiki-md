<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

For a variation $y+\varepsilon\eta$ with $\eta=\eta'=0$ at both endpoints, the [first variation](../../../../../first-variation.md) is

$$
\delta I=\int_{x_0}^{x_1}
(f_y\eta+f_{y'}\eta'+f_{y''}\eta'')\,dx.
$$

Two applications of [integration by parts](../../../../../integration-by-parts.md) remove derivatives from $\eta$. The boundary terms vanish, and the [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives the [higher-order Euler-Lagrange equation](../../../../../higher-order-euler-lagrange-equation.md)

$$
\boxed{f_y-\frac d{dx}f_{y'}+\frac{d^2}{dx^2}f_{y''}=0.}
$$

For the stated integrand,

$$
f_y=2y,\qquad f_{y'}=4y'+2y'',\qquad f_{y''}=2(y'+y''),
$$

so the equation reduces to

$$
y^{(4)}-2y''+y=0,
\qquad (D^2-1)^2y=0.
$$

The general solution of this [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) is

$$
y=(A+Bx)e^x+(C+Dx)e^{-x}.
$$

Decay and finiteness of the integral force $A=B=0$; $y(0)=1$ gives $C=1$, and $y'(0)=2$ gives $D=3$. Hence the unique stationary function is

$$
\boxed{y(x)=(3x+1)e^{-x}.}
$$

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
