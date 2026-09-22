<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the clamp at $s=0$ with $x(0)=y(0)=\theta(0)=0$. An end [force](../../../../force-split.md) without an applied end moment gives the free-end condition $\theta'(1)=0$. With $F=0$, the [Euler elastica](../../../../euler-elastica.md) equation is $EI\theta''+G\cos\theta=0$. For $|G|/(EI)\ll1$, $\theta$ is small, so the leading equation is

$$
EI\theta''=-G.
$$

Integrating with the two [boundary conditions](../../../../boundary-condition.md) gives

$$
\boxed{\theta(s)=\frac G{EI}\left(s-\frac{s^2}{2}\right).}
$$

To first order, $x'=\cos\theta=1+O(G^2)$ and $y'=\sin\theta=\theta+O(G^3)$. Hence

$$
\boxed{x(s)=s+O(G^2),\qquad
y(s)=\frac{G}{6EI}s^2(3-s)+O(G^3),\quad0\leq s\leq1.}
$$

Equivalently $y(x)=Gx^2(3-x)/(6EI)$ at leading order, the familiar [cantilever](../../../../cantilever.md) response. Because $G<0$, the deflection is downward. The free-end [displacement field](../../../../displacement-field-mechanics.md) and slope are $y(1)=G/(3EI)$ and $\theta(1)=G/(2EI)$. The remainder notation holds with fixed positive $EI$ and nondimensional unit rod length.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
