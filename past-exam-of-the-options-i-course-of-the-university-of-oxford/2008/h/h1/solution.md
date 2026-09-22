<h1 id="h/h1/solution">Solution</h1>

↑ **Parent:** [H1](../h1.md)

Put $A(r)=r^2/(r-2m)^2$ and $B(r)=r^3/(r-2m)$, so $L=A\dot r^2+B\dot\varphi^2$. Direct differentiation gives $A'=-4mr/(r-2m)^3$ and $B'=2r^2(r-3m)/(r-2m)^2$. The [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are $2A\ddot r+A'\dot r^2-B'\dot\varphi^2=0$ and $(d/dt)(2B\dot\varphi)=0$, equivalently

$$
\boxed{\ddot r-\frac{2m}{r(r-2m)}\dot r^2-(r-3m)\dot\varphi^2=0},
$$



$$
\boxed{\ddot\varphi+\frac{2(r-3m)}{r(r-2m)}\dot r\dot\varphi=0}.
$$

The cyclic angular coordinate and time [independence](../../../../independent-random-variables.md) give the two conserved quantities

$$
\boxed{J=\frac{2r^3}{r-2m}\dot\varphi,\qquad E=\frac{r^2}{(r-2m)^2}\dot r^2+\frac{r^3}{r-2m}\dot\varphi^2}.
$$

The expression for $E$ equals $L$ here because $L$ is homogeneous quadratic in the velocities.

For a constant radius and nonzero angular motion, the radial equation requires $(r_*-3m)\dot\varphi^2=0$, so $\boxed{r_*=3m}$. This lies outside $2m$, and the angular equation then gives $\varphi=\Omega t+\varphi_0$, with any nonzero constant $\Omega$. This is the [photon sphere](../../../../photon-sphere.md) radius in the stated coordinates. If both velocities are zero, the displayed variational equations also admit a stationary configuration at any radius; the moving circular photon solution is the nonzero-speed case just found.

## ↑ Ancestors (12)

1. [H1](../h1.md)
2. [H](../../h.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
