# Slowly opening Stokes wedge

↑ **Parent:** [Biharmonic stream function for planar Stokes flow](biharmonic-stream-function-for-planar-stokes-flow.md)

For a fixed wall at $\theta=0$ and a wall rotating at $\dot\alpha$ at $\theta=\alpha$, the [quasi-steady Stokes approximation](quasi-steady-stokes-approximation.md) with the [no-slip boundary condition](no-slip-boundary-condition.md) gives

$$
G(\theta)=\frac{\sin\alpha(1-\cos2\theta)+\cos\alpha(\sin2\theta-2\theta)}{2(\sin\alpha-\alpha\cos\alpha)}.
$$

Indeed the [biharmonic equation](biharmonic-equation.md) for $r^2G$ is $G^{(4)}+4G''=0$; the angular basis is $1,\theta,\sin2\theta,\cos2\theta$. The four wall conditions are $G(0)=G'(0)=G'(\alpha)=0$, $G(\alpha)=1$. The outward radial [volume flux per unit width](volume-flux-per-unit-width.md) is $-r^2\dot\alpha/2$, precisely the negative rate of increase of wedge [area](surface-area.md). The associated local [pressure](pressure-split.md) is $p=\mu\dot\alpha[2\cos\alpha/(\sin\alpha-\alpha\cos\alpha)]\log(r/r_*)+C$. Its logarithmic singularity is integrable, although the ideal hinge requires a microscopic regularization.

## ↑ Ancestors (7)

1. [Biharmonic stream function for planar Stokes flow](biharmonic-stream-function-for-planar-stokes-flow.md)
2. [Stokes flow](stokes-flow-split.md)
3. [Viscous fluid flow](viscous-fluid-flow-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-fluids-course-of-the-university-of-oxford/2021/1/c/solution.md)
