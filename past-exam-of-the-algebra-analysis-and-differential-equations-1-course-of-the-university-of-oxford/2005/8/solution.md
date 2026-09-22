<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

The [characteristic equations for a first-order quasilinear equation](../../../characteristic-equations-for-a-first-order-quasilinear-equation.md) are $\dot x=x$, $\dot y=y$, $\dot u=2u$, with characteristic parameter $s$. Through the prescribed point they give

$$
\boxed{(x(s),y(s),u(s))=(x_0e^s,y_0e^s,u_0e^{2s}).}
$$

For a nonzero projected initial point, the [characteristic projections](../../../characteristic-projection.md) are rays from the origin, not trajectories crossing through the origin to the opposite ray. If $x_0=y_0=0$, a classical solution graph requires $u_0=0$, because the original equation reduces there to $0=2u$.

Parameterize the initial line by $(x,y,u)=(a,1-a,a^3)$. Along its characteristic, $x+y=e^s>0$, $a=x/(x+y)$ and $u=a^3e^{2s}$. Therefore

$$
\boxed{u(x,y)=\frac{x^3}{x+y},\qquad x+y>0.}
$$

Differentiation verifies the equation, and substitution of $x+y=1$ verifies the initial data. [Characteristic reachability for radial transport](../../../characteristic-reachability-for-radial-transport.md) shows why the domain is this positive half-plane: each point there lies on precisely one characteristic from the data line. Rays in $x+y<0$ never meet that line, so their values are not determined by these data. Allowing a negative scaling factor would incorrectly join two different characteristic rays through a degenerate origin.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2005](../../2005-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
