<h1 id="a/2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the tangential length and [velocity](../../../../../../velocity.md) scales as order one. In the [boundary layer](../../../../../../boundary-layer.md), continuity reads $u_x+(\delta_2/\delta_1)V_Y=0$, so a nontrivial balance requires $\delta_2\sim\delta_1$. Tangential inertia is order one, and the normal viscous term has size $\mathrm{Re}^{-1}\delta_1^{-2}$. Balancing them gives

$$
\boxed{\delta_1=\delta_2=\mathrm{Re}^{-1/2}}
$$

up to constants absorbable in the scaled variables. Streamwise diffusion is then smaller by $\mathrm{Re}^{-1}$. The normal [momentum](../../../../../../momentum-split.md) equation has a [pressure](../../../../../../pressure-split.md) term of size $\delta_1^{-1}p_Y$ and inertial/viscous terms of size $\delta_1$, hence $p_Y=0$ at leading order. The remaining [Prandtl boundary-layer equations](../../../../../../prandtl-boundary-layer-equation.md) are

$$
\boxed{uu_x+Vu_Y=-p_x+u_{YY},\qquad p_Y=0,\qquad u_x+V_Y=0.}
$$

The [boundary conditions](../../../../../../boundary-condition.md) are **no slip and no penetration at the plate, and matching to the outer tangential [velocity](../../../../../../velocity.md)**:

$$
\boxed{u(x,0)=0,\qquad V(x,0)=0,\qquad u(x,Y)\longrightarrow U_s(x)\quad(Y\to\infty).}
$$

The outer inviscid tangential [momentum](../../../../../../momentum-split.md) equation supplies $p_x=-U_sU_s'$; [pressure](../../../../../../pressure-split.md) is shared between the [boundary layer](../../../../../../boundary-layer.md) and outer flow because it has no leading normal variation.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../../split.md)
7. [Theoretical mechanics course of the University of Oxford](../../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
