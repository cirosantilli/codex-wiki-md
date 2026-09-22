<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a spherically symmetric [number density](../../../../number-density.md), the radial [Laplacian](../../../../laplacian.md) is $r^{-2}\partial_r(r^2\partial_rn)$. Applying [separation of variables](../../../../separation-of-variables.md) and choosing the separation constant $-k^2$ gives

$$
\frac{R''+2R'/r}{R}=\frac{T'}T-\lambda=-k^2,
$$

so the [ordinary differential equations](../../../../ordinary-differential-equation.md) are

$$
\boxed{R''+\frac2rR'+k^2R=0,\qquad T'=(\lambda-k^2)T.}
$$

The radial problem is an [eigenvalue problem](../../../../eigenvalue-problem.md) for $-\Delta$ with [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md), hence $k^2>0$: multiplying the radial equation by $r^2\overline R$ and integrating gives $k^2\int_0^ar^2|R|^2dr=\int_0^ar^2|R'|^2dr>0$ for a nonzero regular mode vanishing at $a$.

To solve it explicitly, set $R=f/r$, corresponding to the suggested power $p=-1$. The equation reduces to $f''+k^2f=0$, so

$$
R(r)=\frac{A\sin(kr)+B\cos(kr)}r.
$$

Finiteness at the origin forces $B=0$, and the [Dirichlet boundary condition](../../../../dirichlet-boundary-condition.md) at $r=a$ requires $k=m\pi/a$ for an integer $m\geq1$. The absence of interior zeros excludes $m\geq2$, selecting the fundamental [normal mode](../../../../normal-mode.md). If $n_c>0$ denotes the initial central density, the result is

$$
\boxed{n(r,t)=n_c\frac{\sin(\pi r/a)}{\pi r/a}\exp\left[\left(\lambda-\frac{\pi^2}{a^2}\right)t\right],\qquad 0\leq r\leq a,}
$$

where the sine ratio is defined as $1$ at the origin. It is strictly positive in the interior for every finite time. The arbitrary positive scale $n_c$ cannot be fixed without additional initial data.

The spatial factor is time independent, so the density and the total [neutron](../../../../neutron-split.md) population have the same exponential growth rate. Thus the [spherical reaction-diffusion growth threshold](../../../../spherical-reaction-diffusion-growth-threshold.md) is

$$
\boxed{\lambda>\frac{\pi^2}{a^2}.}
$$

At equality the fundamental mode is stationary; below it the mode decays. For fixed $\lambda>0$, the equivalent critical-radius condition is $a>\pi/\sqrt\lambda$. This is the competition between multiplication in the bulk and [diffusion](../../../../diffusion.md) loss at the surface in the stated dimensionless model.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
