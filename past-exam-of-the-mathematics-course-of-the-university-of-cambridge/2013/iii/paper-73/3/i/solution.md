<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take a [beta-plane approximation](../../../../../../beta-plane.md), $f=f_0+\beta y$ with $\beta>0$, and define the depth transport $\mathbf T=(U,V)=\int_{-H}^0\mathbf u_h\,dz$. For steady flow with no net flux through surface and bed, depth-integrated continuity gives $U_x+V_y=0$. Vertical integration of momentum gives

$$
f\hat{\mathbf k}\times\mathbf T=-\frac1{\rho_0}\nabla_h\int_{-H}^0p\,dz
+\frac{\boldsymbol\tau_w-\boldsymbol\tau_b}{\rho_0}+\nu\nabla_h^2\mathbf T.
$$

In the interior, small depth-to-horizontal aspect ratio makes vertical stress divergence the leading viscous contribution; horizontal viscous terms are neglected there. Taking the vertical component of curl eliminates pressure. Since

$$
\nabla_h\times(f\hat{\mathbf k}\times\mathbf T)=f(U_x+V_y)+\beta V=\beta V,
$$

neglecting bottom stress gives the [Sverdrup balance](../../../../../../sverdrup-balance.md),

$$
\boxed{\beta V=\frac1{\rho_0}\left(\partial_x\tau_{wy}-\partial_y\tau_{wx}\right)=\frac W{\rho_0}.}
$$

Thus the wind-stress curl sets the interior meridional depth transport, not the local surface meridional velocity. A constant-$f$ plane would have no $\beta V$ term; the use of $\beta$ in this question requires latitude-dependent $f$. For a transport [streamfunction](../../../../../../stream-function.md) with $(U,V)=(-\bar\psi_y,\bar\psi_x)$, the interior relation is $\beta\bar\psi_x=W/\rho_0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
