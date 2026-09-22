<h1 id="g/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take independent smooth [variations](../../../../variation.md) $y+\varepsilon\eta$ and $z+\varepsilon\zeta$. Differentiating the [functional](../../../../functional.md) and using [integration by parts](../../../../integration-by-parts.md) gives its [first variation](../../../../first-variation.md)

$$
\delta J=[F_{y'}\eta+F_{z'}\zeta]_a^b+\int_a^b\left[(F_y-\tfrac d{dx}F_{y'})\eta+(F_z-\tfrac d{dx}F_{z'})\zeta\right]dx.
$$

First choose [variations](../../../../variation.md) vanishing at the endpoints. To use the stated form of the [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md), take $\eta=(x-a)(b-x)\chi$ with arbitrary smooth $\chi$, and similarly for $\zeta$. The lemma makes $(x-a)(b-x)(F_y-dF_{y'}/dx)$ vanish, and hence makes the unweighted coefficient vanish in the interior; continuity extends this to the endpoints. Applying the same argument to $z$ gives the [Euler-Lagrange equations](../../../../euler-lagrange-equation.md)

$$
\boxed{\frac d{dx}F_{y'}=F_y,\qquad\frac d{dx}F_{z'}=F_z.}
$$

If either endpoint value of $y$ or $z$ is free, the corresponding variation there is arbitrary. The remaining boundary term gives the [natural boundary conditions for a free endpoint](../../../../natural-boundary-conditions-for-a-free-endpoint.md): $F_{y'}=0$ for a free $y$ value and $F_{z'}=0$ for a free $z$ value at that endpoint. With both coordinates free at both endpoints, all four conditions apply.

For the specified integrand these equations reduce to

$$
y''+5y-2z=0,\qquad z''+2y=0,
$$

and the natural conditions are $y'=z'=0$ at each free endpoint. Eliminating $z$ gives

$$
y^{(4)}+5y''+4y=0,\qquad (D^2+1)(D^2+4)y=0.
$$

Its four independent modes give the full general solution

$$
\begin{aligned}
y&=A\cos x+C\sin x+B\cos2x+D\sin2x,\\
z&=2A\cos x+2C\sin x+\tfrac12B\cos2x+\tfrac12D\sin2x.
\end{aligned}
$$

At zero, $y'(0)=C+2D$ and $z'(0)=2C+D$. Vanishing forces $C=D=0$, giving

$$
\boxed{y=A\cos x+B\cos2x,\qquad z=2A\cos x+\frac B2\cos2x.}
$$

At $x=\pi/6$ the two derivative conditions become $A/2+\sqrt3B=0$ and $A+\sqrt3B/2=0$. Their coefficient determinant is nonzero, so $A=B=0$. Thus **the unique stationary extremal with all four natural boundary conditions is $y=z=0$**. The word extremal here means a stationary point of the functional; the indefinite integrand does not require this point to be a minimum.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [G](../../g.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
