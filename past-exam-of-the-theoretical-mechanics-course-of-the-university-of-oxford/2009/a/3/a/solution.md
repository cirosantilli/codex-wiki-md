<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Scale $x,y$ by $L$, $z$ by $\delta L$, tangential velocities by $U$, normal [velocity](../../../../../velocity.md) by $\delta U$, and time by $L/U$. Continuity balances all three derivatives. Tangential viscous forces scale as $\mu U/(\delta^2L^2)$, hence their [pressure](../../../../../pressure-split.md) balance requires

$$
\boxed{p\sim\frac{\mu U}{\delta^2L},\qquad t\sim L/U.}
$$

The inertial/normal-viscous ratio is $\delta^2\rho LU/\mu$, so it is negligible under the given smallness condition. Tangential viscous derivatives are smaller by $\delta^2$; the normal [pressure](../../../../../pressure-split.md) balance gives $p_z=0$ at leading order. In dimensional variables the remaining equations are continuity, $\mu u_{zz}=p_x$, $\mu v_{zz}=p_y$, $p_z=0$.

[No-slip boundary condition](../../../../../no-slip-boundary-condition.md) at each plate imposes $u=v=0$, while their normal velocities are $w(0)=0$ and $w(h)=\dot h$. Integrating the two tangential equations twice gives

$$
(u,v)=\frac{z(z-h)}{2\mu}\nabla p,\qquad
\boxed{\overline{\mathbf u}=\frac1h\int_0^h(u,v)\,dz=-\frac{h^2}{12\mu}\nabla p.}
$$

Integrate continuity through the gap. Since $h$ is independent of in-plane position and the tangential [velocity](../../../../../velocity.md) vanishes at the upper wall, the flux divergence is $\nabla\cdot(h\overline{\mathbf u})$ and the normal contribution is $\dot h$. Therefore

$$
\boxed{\dot h+\nabla\cdot(h\overline{\mathbf u})=0.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
