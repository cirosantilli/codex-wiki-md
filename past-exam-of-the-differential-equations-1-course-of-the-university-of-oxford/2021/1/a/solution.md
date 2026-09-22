<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [method of characteristics](../../../../method-of-characteristics.md) replaces the [first-order partial differential equation](../../../../first-order-partial-differential-equation.md) by the [ordinary differential equations](../../../../ordinary-differential-equation.md)

$$
\dot x=x,\qquad \dot y=2y+\beta x,\qquad \dot u=x+2.
$$

An [integrating factor](../../../../integrating-factor.md) for the second equation gives $d(e^{-2s}y)/ds=\beta C e^{-s}$, so their general [solution of a differential equation](../../../../solution-of-a-differential-equation.md) is

$$
\boxed{x=C e^s,\qquad y=D e^{2s}-\beta C e^s,\qquad u=C e^s+2s+E.}
$$

Here $C,D,E$ are real constants. For $C\ne0$, eliminating $s$ gives the [characteristic projections](../../../../characteristic-projection.md)

$$
\boxed{y=Kx^2-\beta x,\qquad K=D/C^2,}
$$

each restricted to either $x>0$ or $x<0$. These are arcs of [parabolas](../../../../parabola.md), with the straight-line exception $K=0$. Along an oriented [characteristic curve](../../../../characteristic-curve.md), $|x|$ increases with $s$.

For $C=0$, the [characteristic projections](../../../../characteristic-projection.md) lie on $x=0$: $y=D e^{2s}$ describes either vertical half-line when $D\ne0$. For $C=D=0$ the projection is the single point $(0,0)$, although $u=2s+E$ still changes. This last lifted [characteristic curve](../../../../characteristic-curve.md) cannot be contained in the [function graph](../../../../graph-of-a-function.md) of a [classical solution](../../../../classical-solution.md): at $(0,0)$ the original [partial differential equation](../../../../partial-differential-equation-split.md) would require $0=2$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the differential equations 1 course of the University of Oxford](../../../split.md)
5. [Differential equations 1 course of the University of Oxford](../../../../differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
