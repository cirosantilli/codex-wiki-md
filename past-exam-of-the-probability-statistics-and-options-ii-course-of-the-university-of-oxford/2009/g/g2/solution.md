<h1 id="g/g2/solution">Solution</h1>

↑ **Parent:** [G2](../g2.md)

At a regular constrained stationary curve, choose a constant multiplier $\lambda$ and make the augmented functional $I-\lambda J$ stationary under endpoint-fixed variations. Its integrand is $H=F-\lambda G$ and the equation is $dH_{y'}/dx-H_y=0$. This normal multiplier formulation requires the [first variation](../../../../first-variation.md) of the constraint not to vanish identically; the usual abnormal case would require two multipliers. When $H_x=0$,

$$
\frac d{dx}(y'H_{y'}-H)=y'\left(\frac d{dx}H_{y'}-H_y\right)-H_x=0,
$$

so $\boxed{y'H_{y'}-H=c_0}$ is constant, proving the requested first integral.

For the chain, $ds=\sqrt{1+(y')^2}dx$, so the fixed physical length is exactly $J[y]$. Its gravitational potential, apart from the constant factor $\rho g$, is $I[y]=\int_{-a}^ay\sqrt{1+(y')^2}dx$. Thus $H=(y-\lambda)\sqrt{1+(y')^2}$, and the Euler–Lagrange equation is

$$
\boxed{\frac d{dx}\left(\frac{(y-\lambda)y'}{\sqrt{1+(y')^2}}\right)-\sqrt{1+(y')^2}=0.}
$$

The first integral becomes $(y-\lambda)/\sqrt{1+(y')^2}=c$, after renaming the constant with the opposite sign. The differential equation also gives $(y-\lambda)y''=1+(y')^2$, so the nondegenerate solution integrates to $y=\lambda+c\cosh((x-x_0)/c)$. Equal endpoint heights force $x_0=0$: the two cosh values agree only when their arguments are equal or opposite, and $a>0$ excludes the former. Hence

$$
\boxed{y(x)=\lambda+c\cosh(x/c).}
$$

For the hanging energy [minimum](../../../../local-minimum.md) take $c>0$. Since $\sqrt{1+(y')^2}=\cosh(x/c)$,

$$
\boxed{L=2c\sinh(a/c),\qquad\lambda=b-c\cosh(a/c).}
$$

For $L>2a$ the length equation has exactly one positive solution: its right side decreases from infinity to $2a$ as $c$ increases from zero to infinity. For $L=2a$ the only feasible shape is the straight segment, obtained as a limiting case; for $L<2a$ no chain can span the endpoints. A negative $c$ gives the inverted stationary [catenary](../../../../catenary.md), rather than the physically hanging [minimum](../../../../local-minimum.md).

## ↑ Ancestors (12)

1. [G2](../g2.md)
2. [G](../../g.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
