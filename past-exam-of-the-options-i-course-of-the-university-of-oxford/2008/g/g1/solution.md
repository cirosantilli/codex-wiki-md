<h1 id="g/g1/solution">Solution</h1>

↑ **Parent:** [G1](../g1.md)

With fixed endpoint values, a smooth extremal satisfies the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) $F_y-(d/dx)F_{y'}=0$. If $F$ has no explicit $x$ dependence, differentiation gives

$$
\frac d{dx}(F-y'F_{y'})=y'\left(F_y-\frac d{dx}F_{y'}\right)=0.
$$

Thus $F-y'F_{y'}$ is constant, the [Beltrami identity](../../../../beltrami-identity.md).

For this integrand, $F_y=2y$ and $F_{y'}=1+2y'$, so the equation is $y''=y$. Consequently

$$
\boxed{y(x)=Ae^x+Be^{-x}}.
$$

The two constants are fixed uniquely by the prescribed values at distinct endpoints. Equivalently, writing these values as $y_1,y_2$,

$$
y(x)=\frac{y_1\sinh(x_2-x)+y_2\sinh(x-x_1)}{\sinh(x_2-x_1)}.
$$

Its first integral is $y^2-y'^2$, which is constant. Using only that first integral without the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) could admit spurious constant functions, so the differential equation was used directly.

For any nonzero endpoint-vanishing perturbation $\eta$, the linear terms in $J[y+\eta]-J[y]$ vanish by the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) and [integration by parts](../../../../integration-by-parts.md); also $\int\eta'=0$. The remainder is

$$
J[y+\eta]-J[y]=\int_{x_1}^{x_2}(\eta^2+\eta'^2)\,dx>0.
$$

Hence the extremal is the **unique strict global minimum**, and cannot be a maximum.

## ↑ Ancestors (12)

1. [G1](../g1.md)
2. [G](../../g.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
