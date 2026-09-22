<h1 id="36b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Independence of $x$ and [incompressibility](../../../../../../incompressible-flow.md) give $v_y=0$ for the secondary velocity $(u,v,0)$. No penetration at the upper and lower walls then forces $v=0$. The radial momentum equation, retaining the given centrifugal acceleration, is $-w^2/R=-p_x/\rho+\nu u''$. The transverse pressure gradient is constant in $y$ at this order. Integrating twice and absorbing the resulting quadratic coefficient into $C$ gives

$$
\boxed{u(y)=K(5a^2y^4-y^6)+\tfrac12Cy^2+D,\qquad
K=\frac{G^2}{120\rho^2\nu^3R}.}
$$

The odd integration term vanishes because both no-slip conditions are equal. The remaining no-slip and zero-flux conditions are

$$
\boxed{4Ka^6+\tfrac12Ca^2+D=0,\qquad
\tfrac67Ka^7+\tfrac16Ca^3+Da=0.}
$$

The second equation is half of $\int_{-a}^au(y)dy=0$. Optionally solving gives $C=-66Ka^4/7$ and $D=5Ka^6/7$. With $s=y/a$ the velocity is $Ka^6(1-s^2)(s^4-4s^2+5/7)$, so the ratio to the primary velocity is bounded, including its limiting value at the walls, by a constant times $Ga^4/(\rho\nu^2R)$. A sufficient parameter ordering is

$$
\boxed{a\ll b\ll R,\qquad\frac{Ga^4}{\rho\nu^2R}\ll1.}
$$

Equivalently the last condition is $\mathrm{Re}\,a/R\ll1$ for $\mathrm{Re}=Ga^3/(\rho\nu^2)$. It keeps the secondary circulation weak; the neglected radial return flow and side-wall structure supply closure outside this central wide-channel approximation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [36B](../../36b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
