<h1 id="g/g2/solution">Solution</h1>

↑ **Parent:** [G2](../g2.md)

For a [variation](../../../../variation.md) $y+\varepsilon\eta$ with $\eta(0)=\eta(1)=0$, stationarity gives

$$
0=\int_0^1(F_y\eta+F_{y'}\eta')\,dx
=\int_0^1\left(F_y-\frac d{dx}F_{y'}\right)\eta\,dx.
$$

The boundary term vanishes. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore gives the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) $dF_{y'}/dx-F_y=0$.

Differentiating the proposed first integral gives

$$
\frac d{dx}(F-y'F_{y'})=F_x+y'\left(F_y-\frac d{dx}F_{y'}\right).
$$

Thus it is constant along an extremal when $F_x=0$, proving the [Beltrami identity](../../../../beltrami-identity.md).

For the positive branch relevant to the endpoint data, $F=\sqrt{1+y'^2}/y$. The identity becomes

$$
\frac1{y\sqrt{1+y'^2}}=\frac1R,\qquad y^2(1+y'^2)=R^2.
$$

The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) itself gives $yy''=-(1+y'^2)$, so $(y^2)''=-2$. Integrating, or solving the first integral, yields a circle $y^2+(x-c)^2=R^2$. The equal endpoint values force $c=1/2$ and $R^2=5/4$. Hence the unique positive smooth extremal is

$$
\boxed{y(x)=\sqrt{\frac54-\left(x-\frac12\right)^2}.}
$$

It stays positive on the entire interval and satisfies the second-order equation, including its turning point. Merely differentiating the first integral after dividing by $y'$ would need extra care there. Geometrically this is an arc of a [hyperbolic geodesic](../../../../geodesic-in-the-poincare-half-plane-model.md) in the [upper half-plane model](../../../../poincare-half-plane-model.md).

## ↑ Ancestors (12)

1. [G2](../g2.md)
2. [G](../../g.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
