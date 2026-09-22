<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [antiplane displacement](../../../../antiplane-shear.md) has the form $v(x_1,x_2,x_3)=(0,0,u(x_1,x_2))$, independent of the out-of-plane coordinate. Only $e_{13}=e_{31}=u_{x_1}/2$ and $e_{23}=e_{32}=u_{x_2}/2$ are nonzero, so its strain energy per unit out-of-plane thickness is $\mu|\nabla u|^2/2$.

The equilibrium minimizes total potential energy

$$
\boxed{\mathcal E_s(u)=\int_{\omega\setminus K_s}
\left(\frac\mu2|\nabla u|^2-fu\right)dx,\qquad
u\in H^1(\omega\setminus K_s),\quad u=u_D\text{ on }\Gamma_D.}
$$

Here $f$ is the out-of-plane body-force component; the two [crack](../../../../crack-in-a-solid.md) faces have independent [traces](../../../../matrix-trace.md). For a variation $\eta$ with zero outer-boundary [trace](../../../../matrix-trace.md), stationarity gives

$$
\mu\int\nabla u\cdot\nabla\eta=\int f\eta.
$$

Integrating by parts first for interior [test functions](../../../../test-function.md) and then for variations free on either [crack](../../../../crack-in-a-solid.md) face yields

$$
\boxed{-\mu\Delta u=f\text{ in }\omega\setminus K_s,\qquad
u=u_D\text{ on }\Gamma_D,\qquad\mu\partial_nu=0\text{ on both crack faces}.}
$$

These are the weak equilibrium equation, prescribed [displacement](../../../../displacement.md), and zero [traction](../../../../traction.md). The tip behavior is selected by finite energy; it is not an additional prescribed tip value.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
