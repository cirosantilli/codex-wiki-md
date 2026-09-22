<h1 id="38b/solution">Solution</h1>

↑ **Parent:** [38B](../38b.md)

The outer fluid is at rest, so its pressure is independent of $x$ and $dP/dx=0$. Using [incompressibility](../../../../../incompressible-flow.md), the longitudinal [boundary-layer equation](../../../../../boundary-layer-equation.md) becomes the conservative momentum equation

$$
\partial_x(\rho u^2)+\partial_y(\rho uv-\mu u_y)=0.
$$

Integrating across the jet and using $u,u_y\to0$ and $uv\to0$ at both transverse infinities gives

$$
\boxed{\frac{dF}{dx}=0,\qquad F=\rho\int_{-\infty}^{\infty}u^2\,dy.}
$$

Put $\nu=\mu/\rho$. The momentum-flux scaling gives $U^2\delta\sim F/\rho$, while balancing longitudinal convection with transverse viscous diffusion gives $U^2/x\sim\nu U/\delta^2$. Eliminating $U$ or $\delta$ yields

$$
\boxed{\delta\propto x^{2/3},\qquad U\propto x^{-1/3}.}
$$

Choose the precise width convention $U\delta^2=\nu x$ and take $U$ to be the centre-line velocity. For the [self-similar solution](../../../../../similarity-solution.md) with streamfunction $\psi=U\delta f(\eta)$, $\eta=y/\delta$,

$$
u=U f',\qquad v=\frac{U\delta}{3x}(2\eta f'-f),\qquad u_x=\frac Ux\left(-\frac{f'}3-\frac{2\eta f''}3\right).
$$

The $\eta f'f''$ terms cancel in $uu_x+vu_y$, leaving $-U^2[(f')^2+ff'']/(3x)$. Since $u_{yy}=Uf'''/\delta^2$, the dimensionless profile equation is

$$
\boxed{f'''+\frac13\left(ff''+(f')^2\right)=0.}
$$

For a symmetric jet choose its streamfunction zero at the axis. The boundary and amplitude conditions are $f(0)=0$, $f''(0)=0$, $f'(0)=1$, and $f'(\eta)\to0$ as $\eta\to\pm\infty$, with $f$ bounded and $f''\to0$. The momentum normalization is

$$
\boxed{F=\rho U^2\delta J,\qquad J=\int_{-\infty}^{\infty}[f'(\eta)]^2\,d\eta.}
$$

It determines the dimensional constants in $U,\delta$; one should not independently impose $J=1$ after fixing both the centre-line and width conventions.

Indeed integrating the profile equation once and using its far-field conditions gives $f''+ff'/3=0$. With the axis conditions, $f'=1-f^2/6$, and therefore

$$
\boxed{f(\eta)=\sqrt6\tanh(\eta/\sqrt6),\qquad f'(\eta)=\operatorname{sech}^2(\eta/\sqrt6),\qquad J=\frac{4\sqrt6}{3}.}
$$

Consequently $\delta=(\rho J\nu^2/F)^{1/3}x^{2/3}$ and $U=[F^2/(\rho^2J^2\nu)]^{1/3}x^{-1/3}$. The transverse velocity describes entrainment; the profile need not have $f(\infty)=0$ when its axial velocity vanishes there.

## ↑ Ancestors (11)

1. [38B](../38b.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
