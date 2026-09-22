<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [hydrostatic approximation](../../../../../../hydrostatic-approximation.md) gives $p=\rho g(h-z)$ above the horizontal floor, up to atmospheric pressure. The horizontal [Stokes flow](../../../../../../stokes-flow-split.md) equation is $\mu\mathbf u_{zz}=\rho g\nabla h$, with the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) at $z=0$ and zero tangential stress on the [free surface](../../../../../../free-surface.md). Integrating twice gives $\mathbf u=(\rho g/\mu)\nabla h\,(z^2/2-hz)$ and the [lubrication gravity-current flux](../../../../../../lubrication-gravity-current-flux.md)

$$
\mathbf q_{\rm lab}=-\frac{\rho g}{3\mu}h^3\nabla h.
$$

For the [squeegee lubrication model](../../../../../../squeegee-lubrication-model.md), use $h_0$ vertically, $\ell=\rho gh_0^3/(\mu U)$ horizontally, and $\ell/U$ in time. If $X$ is the laboratory coordinate in the direction of travel, set $x=(X-Ut)/\ell$, $y=Y/\ell$, $t=Ut_{\rm lab}/\ell$, and $h=h_{\rm lab}/h_0$. The blade half-length is $\alpha=L/\ell$. The moving-frame flux is $\mathbf q=-h\mathbf e_x-h^3\nabla h/3$. Conservation of volume gives **the dimensionless lubrication equation**

$$
\boxed{h_t-h_x=\frac13\nabla\cdot(h^3\nabla h),\qquad h\to1\quad(x\to\infty).}
$$

Using these scales as representative of the actual flow, [lubrication theory](../../../../../../lubrication-theory.md) requires a small aspect ratio and negligible inertia relative to vertical viscous resistance:

$$
\boxed{\frac{h_0}{\ell}=\frac{\mu U}{\rho gh_0^2}\ll1,\qquad\frac{\rho Uh_0^2}{\mu\ell}=\frac{U^2}{gh_0}\ll1.}
$$

The second is the [Reynolds number](../../../../../../reynolds-number.md) based on $h_0$, multiplied by $h_0/\ell$. Surface tension is neglected as assumed. Large piles, rounded gaps, and narrow end regions need their own local slope and inertia checks if these representative scales cease to describe them.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
