<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Where $y\ne\beta$, taking the quotient of the two [ordinary differential equations](../../../../../ordinary-differential-equation.md) gives

$$
\frac{dy}{dx}=\frac{x^3-x}{y-\beta},\qquad
\frac{(y-\beta)^2}{2}=\frac{x^4}{4}-\frac{x^2}{2}+\text{constant}.
$$

Choose the [first integral](../../../../../first-integral.md)

$$
\boxed{h(x,y)=\frac{(y-\beta)^2}{2}+\frac{x^2}{2}-\frac{x^4}{4}.}
$$

The [chain rule](../../../../../chain-rule.md) checks conservation even at points excluded in taking that quotient:

$$
\dot h=(x-x^3)(y-\beta)+(y-\beta)(x^3-x)=0.
$$

Thus each trajectory is contained in a [connected component](../../../../../connected-component.md) of a [level set](../../../../../level-set.md) of $h$. At $(0,\beta)$ the [gradient](../../../../../gradient.md) vanishes and the [Hessian matrix](../../../../../hessian-matrix.md) is the identity, so $h$ has a strict [local minimum](../../../../../local-minimum.md) there. To make the closed-trajectory argument explicit, put $z=y-\beta$ and $0<E<1/4$. The bounded component of $h=E$ is

$$
z=\pm\sqrt{2E-x^2+x^4/2},\qquad
|x|\leq r_E:=\sqrt{1-\sqrt{1-4E}}<1.
$$

The two arcs join at $(\pm r_E,0)$ to form a [simple closed curve](../../../../../simple-closed-curve.md) that is a [regular level set](../../../../../regular-level-set.md). The [gradient](../../../../../gradient.md) cannot vanish on it: the only [critical point of a dynamical system](../../../../../equilibrium-point-of-a-dynamical-system.md) in $|x|<1$ is the centre, whose level is $0$.

The [vector field](../../../../../vector-field.md) is tangent and nowhere zero on this [compact set](../../../../../compact-space.md), so its speed has a positive minimum. It therefore traverses the curve in finite time and returns to its initial point, giving a [periodic orbit](../../../../../periodic-orbit.md). These ovals shrink to the centre as $E\downarrow0$. This is the [planar first integral criterion for a centre](../../../../../planar-first-integral-criterion-for-a-centre.md) and proves the required nonlinear assertion; it also gives [Lyapunov stability](../../../../../lyapunov-stability.md) without [asymptotic stability](../../../../../asymptotic-stability.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
