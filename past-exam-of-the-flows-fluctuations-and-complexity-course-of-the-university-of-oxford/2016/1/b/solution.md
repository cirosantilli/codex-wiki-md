<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put the [stagnation point](../../../../stagnation-point.md) at the origin and the local tangent plane at $z=0$. A regular [Taylor expansion](../../../../taylor-expansion.md) has no linear term because $\mathbf u(0)=0$. The impermeable tangent plane imposes $\partial_z\phi=0$ at $z=0$ to leading order, excluding mixed quadratic terms $xz,yz$. For the illustrated axisymmetric approach, [rotational symmetry](../../../../rotational-symmetry.md) in the tangent plane makes the $x^2$ and $y^2$ coefficients equal and removes $xy$. Finally the [Laplace equation](../../../../laplace-equation.md) fixes the normal coefficient to minus twice the tangential one. Up to an irrelevant additive constant,

$$
\boxed{\phi=W(x^2+y^2-2z^2)+O(|\mathbf r|^3),\qquad
\mathbf u=(2Wx,2Wy,-4Wz)+O(|\mathbf r|^2).}
$$

For incoming flow from $z>0$, $W>0$. This is a local leading form under the stated symmetry, not the exact universal potential near every possible wall [stagnation point](../../../../stagnation-point.md); a generic tangential strain can have unequal principal rates.

A [streamline](../../../../streamline.md) solves $\dot x=2Wx$, $\dot y=2Wy$, $\dot z=-4Wz$, hence $x=Ae^{2Wt}$, $y=Be^{2Wt}$, $z=Ce^{-4Wt}$. Eliminating the parameter gives

$$
\boxed{\arg(x+iy)=\text{constant},\qquad z(x^2+y^2)=\text{constant}.}
$$

Each [streamline](../../../../streamline.md) lies in a meridional plane. With cylindrical radius $s=\sqrt{x^2+y^2}$, its shape is $z=C_1/s^2$. The symmetry axis and wall are limiting invariant [streamlines](../../../../streamline.md). A particle exactly on the incoming axis approaches the [stagnation point](../../../../stagnation-point.md) asymptotically.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the flows, fluctuations and complexity course of the University of Oxford](../../../split.md)
5. [Flows, fluctuations and complexity course of the University of Oxford](../../../../flows-fluctuations-and-complexity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
